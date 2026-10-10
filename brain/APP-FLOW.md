# NEXOVAS ERP — App Flow & User Journey Map
## Complete Navigation & Workflow Specification
### Version: FINAL v3.0

---

## 1. SITE MAP / PAGE STRUCTURE

### 1.1 Unauthenticated Pages
- `/` (Landing page)
- `/auth/login` (Login)
- `/auth/signup` (Sign up)
- `/auth/reset-password` (Password reset)
- `/pricing` (Pricing page)
- `/blog` (Blog/resources)

### 1.2 Authenticated Pages (Dashboard)
- `/dashboard` (Main dashboard + God View)
- `/invoices` (Invoice list)
- `/invoices/create` (Create invoice)
- `/invoices/[id]` (Invoice detail + evidence)
- `/invoices/[id]/edit` (Edit invoice)
- `/ledger` (Trial balance)
- `/ledger/accounts/[id]` (Account detail)
- `/ledger/entries` (GL entries log)
- `/compliance/gst` (GST summary + GSTR filings)
- `/compliance/tds` (TDS summary + Form 26Q)
- `/compliance/calendar` (Compliance calendar)
- `/reports/p-and-l` (P&L report)
- `/reports/balance-sheet` (Balance sheet)
- `/reports/cash-flow` (Cash flow)
- `/reports/variance-analysis` (Cost variance)
- `/inventory/count` (Inventory counting via camera)
- `/inventory/stock-balance` (Stock balance report)
- `/payroll/salary-slips` (Salary slip list)
- `/payroll/salary-slips/[id]` (Salary slip detail)
- `/payroll/attendance` (Attendance marking)
- `/settings/company` (Company setup)
- `/settings/users` (User management)
- `/settings/integrations` (Third-party integrations)

---

## 2. AUTHENTICATION FLOW

**Login Journey:**
1. User lands on `/auth/login`
2. Enters email + password
3. API call: `POST /api/v1/auth/login`
4. Server validates, returns JWT token + refresh token
5. Tokens stored in HTTP-only cookies
6. Redirect to `/dashboard`

**Sign-up Journey:**
1. User lands on `/auth/signup`
2. Fills: email, password, company name, GST number, PAN
3. API call: `POST /api/v1/auth/signup`
4. Server creates user + company record
5. Auto-login (return JWT)
6. Redirect to `/dashboard/settings/company` (complete setup)

**OAuth (Google) Flow:**
1. User clicks "Sign in with Google"
2. Redirects to `https://accounts.google.com/o/oauth2/v2/auth?...`
3. User grants permission
4. Callback to `/auth/google/callback`
5. Server creates/updates user + Google Drive link
6. Redirect to `/dashboard`

---

## 3. CORE USER JOURNEYS

### Journey 1: Create & Post Invoice (Retail Kirana)

**Entry Point:** `/dashboard` (God View)

**Steps:**
1. User clicks "New Invoice" button
2. Redirect to `/invoices/create`
3. **Option A: Manual Entry**
   - Select vendor/customer (dropdown with search)
   - Enter invoice date, number
   - Add line items (item, quantity, rate, HSN, GST rate)
   - System auto-calculates: amount, GST, total
   - Click "Save as Draft"
   - Redirect to `/invoices/[id]` (invoice detail)
   - Review invoice
   - Click "Post to Ledger"
   - System auto-generates GL entries:
     - Dr Inventory (or Expense), Cr Vendor
     - Dr GST Receivable, Cr Vendor
   - GL entries posted with blockchain hash
   - Invoice status: "Posted"
   - Evidence (images) saved to Google Drive

4. **Option B: Camera Scan**
   - User clicks "Scan Invoice"
   - Camera opens in modal
   - User photographs invoice
   - TensorFlow Lite OCR processes image (on-device, <2 seconds)
   - Extracted fields displayed: vendor name, amount, HSN, GST rate, date
   - User confirms extracted data
   - Image saved to Google Drive (NEXOVAS_ERP_Data/invoices/2026-10/INV-001.jpg)
   - File ID stored in DB
   - Auto-fill form with extracted data
   - User adjusts if needed
   - Click "Save as Draft"
   - Rest of flow same as manual entry

5. **Option C: Barcode Scan**
   - User clicks "Scan Barcode"
   - Camera opens with barcode overlay
   - User photographs barcode (EAN-13, UPC-A, Code-128)
   - Barcode decoded
   - Product lookup: barcode → SKU → price → HSN → GST rate
   - Line item auto-populated
   - User can scan multiple barcodes for multi-item invoice
   - After all items scanned, click "Create Invoice"
   - Rest of flow same as manual entry

**Approval Gates:**
- <₹1K: Auto-post (no approval needed)
- ₹1K–₹10K: Notify business owner (email) + auto-post in 24 hours (or owner clicks "Approve Now")
- >₹10K: Require explicit approval from business owner (email + in-app notification)

**Result:**
- Invoice posted to GL
- GL entries appended to audit trail
- Daily P&L updated (next day)
- Evidence stored in user's Google Drive
- Blockchain hash generated + stored

---

### Journey 2: File GST Return (Every MSME)

**Entry Point:** `/compliance/gst`

**Steps:**
1. User sees "GST Filing" dashboard
2. Display shows:
   - Current month: October 2026
   - GSTR-1 status: "Ready to File" (if invoices exist)
   - GSTR-2B status: "Reconciliation Pending" (if purchase invoices differ from GSTPortal's GSTR-2B)
   - GSTR-3B status: "Ready to File" (if both 1 and 2B reconciled)
   - Filing deadline: November 11 (3 days remaining)

3. **Reconcile GSTR-2B:**
   - Click "Download GSTR-2B from GST Portal" (manual step, or auto-import if API available)
   - Upload GSTR-2B file
   - System compares: Purchase invoices in NEXOVAS vs. GSTR-2B from portal
   - Differences highlighted (e.g., invoice INV-POA-101 in NEXOVAS but not in portal)
   - User can adjust NEXOVAS data or explain discrepancy
   - Click "Mark as Reconciled"

4. **Generate GSTR-3B:**
   - System auto-calculates:
     - Total ITC from GSTR-2B
     - Total tax payable from GSTR-1
     - Payable = Tax - ITC
   - Display calculation breakdown
   - User reviews + clicks "Confirm"

5. **Generate GSTR-1 (if not already auto-generated):**
   - System pulls all sales invoices from DB
   - Filters by invoice type = "sales"
   - Groups by vendor/customer
   - Auto-fills GSTR-1 format
   - User can edit if needed (e.g., remove cancelled invoices)

6. **File Return:**
   - Click "Download JSON for GST Portal"
   - File downloaded (GSTR-3B-Oct2026.json)
   - User logs into GST portal (gov.in)
   - Uploads JSON file
   - Portal processes, confirms filing
   - Notification sent: "GSTR-3B filed successfully"

**Alternative: Auto-Filing (Future)**
- If GST Portal API available, NEXOVAS files automatically
- Notification: "GSTR-3B filed on your behalf (blockchain-anchored receipt)"

**Result:**
- GSTR-3B filed (compliance obligation met)
- All evidence (invoices, images) organized in Google Drive
- Audit trail complete + hash-chained
- Tax liability calculated + scheduled for payment
- Next month's filing automatically prepared

---

### Journey 3: Process Payroll (HR Manager)

**Entry Point:** `/payroll/attendance`

**Steps:**
1. HR Manager clicks "Mark Attendance"
2. Redirect to `/payroll/attendance`
3. Display calendar for current month (October 2026)
4. For each employee:
   - Select from employee list dropdown
   - Mark attendance: Present (P), Absent (A), Half-day (H), Leave (L)
   - Save
   - System updates: days_worked, days_absent, days_leave
5. After all employees marked, click "Process Payroll"
6. System calculates (for each employee):
   - Gross salary = Base + HRA + DA - Absent deduction
   - PF = 12% of gross (capped at ₹15K/month)
   - ESI = 0.75% of gross (if gross <₹21,000)
   - PT = State-wise amount (e.g., ₹200/month in Maharashtra)
   - TDS = Based on annual salary (progressive calculation, Section 192)
   - Net salary = Gross - PF - ESI - PT - TDS

7. **Approval Gate (HR-Agent vs CA-Agent):**
   - HR-Agent calculates payroll
   - CA-Agent reviews for consistency + fraud
   - If TDS calculation seems off, CA-Agent flags
   - HR-Manager approves (after reviewing CA-Agent's feedback)

8. **Generate Salary Slips:**
   - Click "Generate Salary Slips"
   - System creates PDF for each employee
   - PDF contains: salary head, amount, deductions, net, employee signature line
   - PDFs downloaded to user's computer (or emailed to employees)

9. **Post to Ledger:**
   - Click "Post to Ledger"
   - System auto-generates GL entries:
     - Dr Salary Expense (gross amount)
     - Cr Bank (net amount)
     - Cr PF Liability (PF amount)
     - Cr ESI Liability (ESI amount)
     - Cr PT Payable (PT amount)
     - Cr TDS Payable (TDS amount)
   - GL entries posted + blockchain-hashed

10. **Generate Payment File:**
    - Click "Download Bank File"
    - System generates NEFT/RTGS format (or CSV for bank upload)
    - File contains: employee bank account, net salary, remarks
    - User uploads to bank's online portal
    - Salary transferred to employees' accounts

**Result:**
- Payroll processed for the month
- Salary slips generated + delivered
- GL entries posted (immutable)
- PF/ESI payments due in next 15 days (reminder email)
- TDS payable amount tracked for quarterly filing (Form 26Q)
- Compliance with PF, ESI, PT, TDS automated

---

### Journey 4: Audit Verification (CA Professional)

**Entry Point:** Verification Portal (dedicated login)

**Steps:**
1. CA logs into `/audit/portal`
2. Biometric login (fingerprint/face ID)
3. Email OTP verification
4. CA sees list of clients (e.g., Rajesh Kumar's Kirana Store)
5. Click on client → redirect to `/audit/portal/[client_id]`
6. Display: Trial Balance, GST Reconciliation, Bank Reconciliation, Audit Evidence

7. **Trial Balance Review:**
   - System displays all accounts + balances
   - Dr = Cr validation (should match 100%)
   - CA can drill-down: click on account → see GL entries for that account
   - GL entries display: date, narration, amount, blockchain hash
   - Verify hashes match (no tampering)

8. **GST Reconciliation:**
   - GSTR-1 vs GSTR-2B comparison
   - Highlighted variances explained
   - CA reviews explanations + adjustments
   - Approval checkbox

9. **Bank Reconciliation:**
   - Bank statement (imported) vs. GL entries
   - Unmatched items listed (e.g., outstanding cheques, deposits in transit)
   - CA verifies + approves

10. **Evidence Review:**
    - Scroll through list of all evidence (invoices, images)
    - Click on invoice → opens image from Google Drive
    - Verify: invoice matches GL entry amount, vendor, date
    - Sample 5–10 invoices for verification

11. **Digital Signature:**
    - CA reviews audit summary
    - Clicks "I approve this audit"
    - Verbal oath prompt: "I certify this audit is accurate and complete"
    - Biometric signature (fingerprint/face ID)
    - Signature blockchain-anchored (Ethereum mainnet, optional)
    - Digital certificate generated + sent to client

**Result:**
- Audit complete in 2 hours (vs. 20+ hours traditional)
- All evidence verified + blockchain-anchored
- Digital certificate issued + immutable
- CA firm revenue: ₹2,499 (service charge)
- Client trust: Audit evidence in their own Google Drive
- Compliance obligation met

---

## 4. NAVIGATION PATTERNS

### Pattern 1: Sidebar Navigation (Desktop)
NEXOVAS ├── Dashboard (home icon) ├── Invoices │ ├── All Invoices │ ├── Create Invoice │ └── Pending Approval ├── Ledger │ ├── Trial Balance │ ├── GL Entries │ └── Bank Reconciliation ├── Compliance │ ├── GST (GSTR-1/2B/3B) │ ├── TDS (Form 26Q) │ ├── Labor (PF/ESI) │ └── Calendar ├── Payroll │ ├── Attendance │ ├── Salary Slips │ └── Compliance ├── Inventory │ ├── Count (Camera) │ └── Stock Balance ├── Reports │ ├── P&L │ ├── Balance Sheet │ ├── Cash Flow │ └── Variance Analysis ├── Settings │ ├── Company │ ├── Users │ └── Integrations └── Help ├── Tutorials ├── FAQ └── Support


### Pattern 2: Mobile Bottom Tab Navigation (iOS/Android)
Home (dashboard) Scan (camera) Invoices (history) Reports (quick access) Menu (settings + more)


---

## 5. EMPTY STATES & ERROR STATES

**Empty State: No Invoices Yet**
- Display: "No invoices yet. Create your first invoice!"
- Button: "Scan Invoice" or "Create Manually"
- Illustration: Friendly graphic of invoice

**Empty State: No Compliance Filings**
- Display: "Next filing due on Nov 11. Start preparing now!"
- Button: "Prepare GSTR-3B"

**Error State: Invoice Posting Failed**
- Display: "Failed to post invoice. Reason: GL account not found."
- Suggestion: "Select a valid GL account"
- Button: "Try Again"

**Error State: GST Rate Mismatch**
- Display: "⚠️ HSN Code XYZ should have 18% GST, but invoice shows 12%. Confirm to proceed?"
- Options: "Confirm" or "Edit Invoice"

---

## 6. SUCCESS CRITERIA FOR USER JOURNEYS

**Invoice Journey:**
✅ Scan → Extract → Post to Ledger in <5 minutes (vs. 10 minutes manual entry)
✅ Accuracy >99.5% (matches manual invoice)
✅ Evidence auto-saved to Drive

**GST Filing:**
✅ Prepare GSTR-3B in <30 minutes (vs. 8 hours manual extraction)
✅ 100% accuracy vs. manual audit

**Payroll:**
✅ Process payroll for 50 employees in <10 minutes (vs. 2 hours manual)
✅ Compliance checked automatically

**Audit:**
✅ Complete audit in 2 hours (vs. 20+ hours traditional)
✅ 100% evidence organized + blockchain-anchored
