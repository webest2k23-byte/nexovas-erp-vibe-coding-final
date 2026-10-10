DOCUMENT 01: PRD.md — PRODUCT REQUIREMENTS DOCUMENT
# NEXOVAS ERP — Product Requirements Document (PRD)
## Enterprise-Grade Autonomous Intelligence Platform for MSME Commerce
### Classification: BOARD APPROVAL REQUIRED | ANTIGRAVITY-READY | Version: FINAL v3.0
### Date: October 7, 2026 | Owner: Chief Product Officer + CTO

---

## 1. EXECUTIVE SUMMARY

**NEXOVAS ERP** is a **civilization-scale commerce intelligence platform** that combines:
- **VisionCount AI** (camera-based inventory scanning with 99.9% accuracy)
- **Autoclaw Prime** (1.2 trillion-parameter autonomous decision engine)
- **Biological Firewall™** (human-consent-first quantum particle tracking)
- **Zero Storage Cost Model** (user-owned Google Drive integration)
- **21 Complete ERPNext Modules** (500+ DocTypes, 150+ Reports)

**Core Thesis:** *The camera is the enterprise. The AI is the professional. The phone is the accountant.*

---

## 2. APP NAME & TAGLINE

**App Name:** NEXOVAS ERP

**Primary Tagline:**
> "Zero Storage Cost. Infinite Scale. Autonomous Professional Management."

**Alternate Taglines:**
- "Every business deserves Big-4 accounting. Now on your phone."
- "VisionCount Intelligence meets Autoclaw Prime. Your ERP just became conscious."
- "GST, TDS, Payroll, Inventory — all handled by AI. You focus on growth."

---

## 3. THE PROBLEM STATEMENT

### 3.1 Market Pain (Who Feels It?)

Indian MSMEs (₹20L–₹50Cr annual turnover) face an **impossible trilemma:**

#### **Choice 1: Manual Management (Spreadsheets + WhatsApp)**
- **Time Cost:** 40+ hours/month on accounting alone
- **Financial Cost:** ₹500–₹1,000/month on accountant visits
- **Compliance Risk:** 60% compliance gaps, 30% invoice errors
- **Result:** Tax penalties (₹5L–₹20L annually), director liability

**Key Pain Points:**
- No audit trail → GST/TDS penalties
- No data backup → business disruption on device loss
- No compliance automation → constant regulatory anxiety
- Employees unmotivated by manual, error-prone processes
- Customers frustrated by billing delays
- Bank reconciliation takes 4–6 hours monthly

#### **Choice 2: Traditional ERP Systems (Tally, SAP, Zoho)**
- **Setup Cost:** ₹50K–₹2L implementation + training
- **Monthly Fee:** ₹2K–₹10K licensing (scales with users/transactions)
- **Hardware:** Requires desktop/server (not mobile-native)
- **Learning Curve:** 2–4 weeks per employee
- **Scalability:** Pricing explodes at scale
- **Data Ownership:** Vendor lock-in (provider controls data)
- **Result:** 70% of Indian MSMEs stuck with manual processes

**Key Pains:**
- Can't afford per-user licensing
- Employees resist desktop-only software
- No real-time inventory visibility
- Bank reconciliation is manual
- Compliance reports require manual extraction
- Audit costs remain ₹10K–₹50K/month

#### **Choice 3: Compliance Burden (GST/TDS/Labor/Corporate)**

**GST Complexity:**
- GSTR-1/3B/9 filings require manual invoice extraction (40+ hours)
- HSN code validation (wrong code = ₹5K–₹50K penalty)
- ITC eligibility calculation (common errors = tax liability)
- E-way bill generation (for goods >₹50K)
- E-invoice generation (mandatory for B2B >₹5Cr turnover)

**TDS/Income Tax:**
- 8+ sections (**194C** contractors, **194J** professionals, **194LA** rent, **194D** commission)
- Threshold complexity (e.g., 194C: >₹30K to single contractor/month)
- Quarterly **26Q** filing + annual **24Q** filing
- Advance tax scheduling (15% June 15, 50% Sept 15, 75% Dec 15, 100% March 15)
- **ITR** preparation with Schedule NA/DA/CFL
- Tax-saving recommendations (Section 80C/D/E/G)

**Corporate/Labor Compliance:**
- **ROC** e-form filings (annual requirements)
- **AGM** schedules + director KYC renewals
- **PF** contribution (12% employee + 1.61% employer)
- **ESI** (if applicable, state-specific)
- **Professional tax** (state variations)
- **Minimum wage** tracking (state updates every quarter)
- **Bonus** calculation (Payment of Bonus Act)
- **Gratuity** at exit (statutory calculation)
- Leave encashment limits

**Penalty Exposure:**
- **GST:** ₹100–₹1,000 per return, late filing = 2% interest/month
- **TDS:** 10% of tax amount if not deducted + 30% interest
- **MCA:** ₹10K–₹5L per delayed filing
- **Labor:** ₹5K–₹50K per violation
- **Total Annual Penalty Risk:** ₹5L–₹50L for MSMEs

**CA Visit Reality:**
- ₹2K–₹5K per audit hour
- 50–100 hours/year required (₹1L–₹5L annually)
- Slow turnaround (2–4 weeks for audit sign-off)
- No real-time visibility into compliance gaps

---

## 4. NEXOVAS SOLUTION — CORE VALUE PROPOSITION

### 4.1 Three-Layer Consciousness Stack

#### **LAYER 1: PHYSICAL CONSCIOUSNESS (VisionCount AI + Quantum Dust Infinity™)**

**What It Does:**
Transforms smartphone camera into **enterprise-grade document processor** + **inventory scanner**.

**Core Capabilities:**

1. **Document Scanning & OCR**
   - Photograph invoice → Auto-extract fields (vendor, amount, date, **HSN**, **GST**, **TDS**)
   - Multi-language support (Hindi, Tamil, Telugu, Marathi, Gujarati, English)
   - Confidence scoring: >90% = auto-process, <90% = user confirmation
   - Extract fields: vendor name, invoice number, date, item details, tax rate, HSN, quantity, rate, amount, TDS section
   - Save image to user's Google Drive (linked via file ID in DB)
   - Evidence metadata (session ID, timestamp, user, optional geolocation)

2. **Inventory Counting (Scale-Adaptive)**
   - **Micro Mode** (0.1–10mm items): Pharmaceutical pills, grains, fasteners → 99.2% accuracy
   - **Small Mode** (10–100mm items): Bolts, tools, boxes → 99.7% accuracy
   - **Medium Mode** (shelf audit, visible products) → 99.9% accuracy
   - **Macro Mode** (equipment/vehicles, barcode-required) → 100% with confirmation
   - Variance detection (physical vs. system stock)
   - Auto-suggest reorder quantities (based on consumption history)
   - Quality flagging (rust, damage, expiry detected)
   - Real-time location tagging with THz particles

3. **Barcode/QR Scanning**
   - EAN-13, UPC-A, Code-128 decoding
   - QR code URL parsing (link to product, delivery note, supplier)
   - Product master lookup (match barcode → SKU → price → GST rate)
   - IMEI scanning (for electronics, warranty activation)
   - Auto-fill invoice line items (barcode → product → rate → tax → line total)

4. **Evidence Capture & Storage**
   - Session ID generated (unique per scanning action)
   - Images saved to **user's Google Drive** (folder: NEXOVAS_ERP_Data/[DocType]/[Date]/)
   - Metadata logged (device, GPS location optional, user ID, timestamp)
   - Linked in database (file ID stored, not actual file)
   - Evidence accessible from ledger entries (one-click view)
   - Audit-ready (hash-chained, immutable, linked to transactions)

**Technical Architecture (CPU-Only, Zero Hardware Cost):**
- **TensorFlow Lite** models (runs on-device, no GPU required)
- **MLKit Vision** (Google's free vision API)
- **ONNX Runtime** (optimized inference)
- **Edge processing** (device-side, sync on connection)
- **Offline-first** (works without internet connection)
- **Quantum Dust Particle (QDI) Simulation:** Blockchain-anchored particle tracking without physical particles (MVP phase)

---

#### **LAYER 2: QUANTUM INTELLIGENCE (Autoclaw Prime™ Orchestration)**

**What It Does:**
Routes every business document to the **correct AI agent**, executes deterministic financial engines, maintains immutable audit trail.

**Architecture:**

1. **Autoclaw Prime™ CEO Brain**
   - **Role:** Document classifier, agent orchestrator, decision arbiter
   - **Processing:** 4.7M decisions/second (distributed across 2,847 global nodes)
   - **Training Data:** 100M audit reports, 10B inventory transactions
   - **Confidence Scoring:** 0.0 to 1.0 (fraud probability 0.0000001% or lower)
   - **Decision Protocol:** Observation → Pattern Recognition → Hypothesis → Evidence → Alternative Analysis → Judgment → Blockchain Anchor

2. **Document Classification & Routing**
   - Input: Image, PDF, voice, or API call
   - AI classifier identifies doc type (purchase invoice, sales invoice, journal entry, expense claim, payroll, etc.)
   - Confidence threshold: >90% auto-route, <90% ask user
   - Output: Task graph (sequence of agent calls)
   - Ambiguity handling (if unclear, present multiple options)

3. **Six Specialized Agents (Complete Disclosure)**

**AGENT 1: CA-Agent (Chartered Accountant Prime)**
- **Role:** Ledger posting, GST computation, TDS calculation, fraud detection, bank reconciliation
- **Core Functions:**
  - Journal entry generation (auto Dr/Cr account selection)
  - Double-entry validation (Dr = Cr balance check)
  - GST computation (HSN validation, rate verification, ITC eligibility check)
  - TDS calculation (Section 194C/J/LA/D, threshold checking)
  - Fraud detection (anomaly scoring 0–100, duplicate detection, unusual patterns)
  - Bank reconciliation (auto-match bank statement with ledger)
  - Audit trail (immutable logging, hash-chained entries)
  - Approval gates (risk-based: auto-approve <₹1K, notify CA ₹1K–₹10K, explicit >₹10K)
  - Posted ledger (append-only, no edits, immutable)
- **AI Capabilities:**
  - Detects anomalies (e.g., invoice posted twice)
  - Flags potential fraud (e.g., vendor invoice at 3 AM from unusual location)
  - Suggests account mapping for ambiguous vendors
  - Validates GST-to-HSN matching
  - Checks TDS thresholds against cumulative supplier payments

**AGENT 2: CMA-Agent (Cost & Management Accountant Omega)**
- **Role:** Costing, variance analysis, budget tracking, depreciation, quality cost
- **Core Functions:**
  - Unit cost calculation (standard costing, FIFO/LIFO/Weighted Average)
  - Cost sheet maintenance (per product, per batch)
  - Variance analysis (material, labor, overhead vs. actual)
  - Budget vs. actual tracking (monthly, quarterly, annual)
  - Asset depreciation (straight-line, diminishing value)
  - Quality cost tracking (defects, rework, waste)
  - Inventory valuation (automatic on purchase/production/sale)
  - Cost center allocation (split costs across departments)
- **AI Capabilities:**
  - Detects cost overruns before they happen (predictive variance)
  - Suggests process improvements based on historical data
  - Flags unusual cost patterns (e.g., raw material cost spike)
  - Auto-calculates depreciation schedule
  - Allocates shared costs intelligently across cost centers

**AGENT 3: HR-Agent (Human Resources Intelligence)**
- **Role:** Payroll, PF/ESI, leave, attendance, compliance, gratuity
- **Core Functions:**
  - Salary calculation (gross – deductions = net)
  - PF computation (12% employee + 1.61% employer contribution)
  - ESI calculation (if applicable, threshold-based)
  - Professional tax (state-wise rates, monthly/quarterly)
  - TDS on salary (Section 192, auto-deduction)
  - Leave accrual (EL, SL, CL per employee, per month)
  - Attendance integration (biometric, manual, camera-based)
  - Form 16 generation (tax certificate for employees)
  - Gratuity valuation (exit calculation, payment to employee)
  - Exit processing (FNF, statutory compliance, archival)
  - Compliance calendar (PF submission, ESI return, PT payment due dates)
- **AI Capabilities:**
  - Predicts payroll anomalies (e.g., overpayment due to coding error)
  - Tracks leave encashment limits automatically
  - Calculates gratuity entitlement in real-time
  - Flags minimum wage violations
  - Schedules compliance submissions before deadlines

**AGENT 4: CRM-Agent (Customer Relations Management)**
- **Role:** Lead capture, opportunity tracking, sales order processing, customer segmentation
- **Core Functions:**
  - Lead capture (web form, email, WhatsApp, API)
  - Lead scoring (RFM, industry, company size, engagement)
  - Opportunity tracking (status: Qualified, Proposal, Negotiation, Won/Lost)
  - Quotation generation (auto-pricing, terms, validity)
  - Sales order processing (validate stock, create delivery note)
  - Customer segmentation (RFM, behavioral, geographic)
  - Churn prediction (risk score, engagement alerts)
  - Marketing automation (email, SMS, WhatsApp campaigns)
  - Customer portal (self-service: view invoices, make payments, track orders)
  - Retention analysis (lifetime value, repeat purchase rate)
- **AI Capabilities:**
  - Predicts which customers will churn (next 30 days)
  - Suggests best follow-up timing for leads
  - Auto-pricing based on market rates + customer segment
  - Detects fraudulent leads (competitor honeypots)
  - Optimizes quotation validity dates based on sales cycle

**AGENT 5: PM-Agent (Project Management)**
- **Role:** Project planning, resource allocation, milestone tracking, profitability
- **Core Functions:**
  - Project planning (WBS, milestones, deliverables)
  - Resource allocation (skill-based, availability-based)
  - Gantt chart generation (critical path calculation)
  - Timesheet management (billable hours, project allocation)
  - Budget tracking (cost vs. actual, forecast final cost)
  - Milestone completion (on-time, at-risk, delayed flags)
  - Resource utilization (% billable, idle time alerts)
  - Project profitability (P&L by project, margin analysis)
  - Delivery schedule (customer timeline tracking)
- **AI Capabilities:**
  - Predicts project cost overruns (burn rate analysis)
  - Suggests resource reallocation to prevent delays
  - Flags scope creep (hours vs. planned)
  - Optimizes project profitability per team member
  - Forecasts delivery date based on historical velocity

**AGENT 6: CS-Agent (Customer Service Intelligence)**
- **Role:** Ticket management, SLA monitoring, warranty, returns, escalation
- **Core Functions:**
  - Ticket management (auto-categorization, priority routing)
  - SLA monitoring (breach alerts, escalation rules)
  - Knowledge base (FAQ, self-service resolution)
  - Returns management (approval workflow, refund processing)
  - Warranty validation (serial number lookup, entitlement check)
  - Complaint analysis (root cause, preventive action)
  - Customer feedback (survey post-resolution, satisfaction scoring)
  - Escalation management (time-bound reviews, management visibility)
- **AI Capabilities:**
  - Routes tickets to best-qualified agent (skill-based)
  - Predicts ticket resolution time (helps SLA planning)
  - Auto-suggests solutions from knowledge base
  - Detects fraud in warranty claims
  - Flags repeat complaints (systemic issue)

**Agent Coordination & Conflict Resolution:**
- **CA-Agent vs. CMA-Agent:** If both agents suggest different cost allocations, CEO Brain arbitrates based on audit trail
- **HR-Agent vs. CA-Agent:** HR calculates deductions, CA posts to GL (no double-posting)
- **CRM-Agent vs. CA-Agent:** CRM generates sales order, CA posts revenue when delivery confirmed
- **PM-Agent vs. CA-Agent:** PM tracks project costs, CA posts to ledger monthly
- **CS-Agent vs. CRM-Agent:** CS handles complaints, CRM manages retention (no overlap)

---

#### **LAYER 3: CONSCIOUSNESS INTERFACE (VisionCount Mobile SaaS + CA Portal)**

**What It Does:**
Provides **mobile-first interface** for business users + **professional verification** for CA/CMA.

**1. VisionCount Mobile App (iOS, Android, PWA)**

**Core Modules:**

a) **Omni-Scan™ Module**
   - **THz Quantum Scan** (simulated on CPU, blockchain-anchored)
   - **Neural Vision** (camera-based object detection)
   - **Acoustic Fingerprint** (sound-based authentication)
   - **Gravimetric Sense** (weight-based verification)
   - **Spectral Analysis** (light-spectrum identification)
   - Offline capability (local processing, sync when connected)
   - Evidence saved to user's Google Drive

b) **God View Dashboard**
   - Global inventory real-time visibility
   - P&L dashboard (updated daily)
   - Autoclaw status (current decisions, pending approvals)
   - Compliance calendar (next filing deadline)
   - Cash flow forecast (next 30 days)
   - Top 10 risks (fraud probability, payment defaults, inventory variances)

c) **Autoclaw Chat**
   - Natural language queries ("Show me margin by product")
   - Root cause analysis (why did profit drop?)
   - What-if scenarios ("If we raise prices 5%, impact on margin?")
   - Compliance queries ("Am I GST-compliant?")
   - AI-powered explanations (not just numbers)

d) **Audit Portal**
   - CA/CMA login (biometric + email verify)
   - Trial balance (all accounts, balances)
   - GST reconciliation (GSTR-1 vs GSTR-2B, highlighted variances)
   - Bank reconciliation (statement vs ledger)
   - Evidence access (one-click to Drive images, PDFs)
   - Digital signature workflow (blockchain-anchored)
   - Audit report generation (forms, certificates, compliance checklist)

**2. CA/CMA Professional Portal**

**Features:**
- **Consciousness Authentication** (biometric + knowledge + optional EEG)
- **Quantum Verification** (THz array activation, particle response validation)
- **Consciousness-Locked Digital Signatures** (verbal oath + truthfulness analysis)
- **Digital Certificate Generation** (immutable blockchain anchoring)
- Bulk client management (audit 50–100 clients vs. current 10–20)
- Pre-filled GST/TDS data (reduce manual entry by 80%)
- Audit evidence auto-organized
- Blockchain-anchored sign-offs

---

### 4.2 Bring Your Own Storage (BYOS) Model

**Why It Matters:**

| Aspect | Traditional SaaS | NEXOVAS BYOS |
|--------|------------------|--------------|
| **Storage Cost per User** | ₹50–₹200/month | ₹0 (user's Google Drive) |
| **Data Ownership** | Provider controls | User controls (in Drive) |
| **GDPR Compliance** | Cloud hosting in US | India-only compute, files in user's account |
| **Scalability Cost** | Grows linearly | Zero marginal cost per user |
| **Trust** | Provider may sell data | Data stays with user |
| **Backup** | Dependent on provider | User owns backups |

**Business Impact:**
- **10,000 users = 150GB storage cost:** Traditional SaaS = ₹5L–₹10L/month, NEXOVAS = ₹0
- **Gross Margin:** 90%+ per user (vs. 60–70% traditional SaaS)
- **Marketing Message:** *"Your data is in your Google Drive, not our servers."*
- **Revenue Model:** Pure software licensing (no storage arbitrage)

**Implementation:**
- Files stored in: User's Google Drive (15GB free per user forever)
- NEXOVAS stores: Only metadata + Drive file IDs
- Database size: 1MB per company (just references)
- Infinite scalability: 10,000 users = zero storage cost to NEXOVAS

---

## 5. TARGET USER PERSONAS

### 5.1 Primary: MSME Business Owner

**Name:** Rajesh Kumar (age 35–55)

**Business:** Kirana store / manufacturing unit / trading house (₹20L–₹50Cr turnover)

**Current Situation:**
- Spends 30–40 hours/month on manual accounting
- Can't afford ₹5K+/month for Tally/Zoho
- Fears GST/tax penalties → hires accountant for ₹2K/month (partial coverage)
- No visibility into real-time P&L, inventory, payroll
- Employees struggle with manual processes
- Bank reconciliation takes 4–6 hours
- Audit costs ₹10K–₹50K/month

**Pain Points:**
1. **Time:** Accounting consumes 40+ hours/month
2. **Compliance:** GST/TDS deadlines missed regularly
3. **Cost:** CA visits expensive + partial coverage
4. **Visibility:** Can't answer "What's my profit today?"
5. **Trust:** Employees prone to errors/embezzlement

**What He Needs:**
✅ One-touch billing (camera scan → invoice → payment)
✅ Automatic GST/TDS calculation
✅ Real-time P&L visibility
✅ Compliance automation (GST filing, TDS payments scheduled)
✅ Affordable (₹999–₹4,999/month, not ₹10K+)
✅ Mobile-first (he uses phone for everything)
✅ Data ownership (his files in his Drive)

**User Journey (First 30 Days):**
- Day 0: Signs up on mobile, takes 10 minutes onboarding
- Day 1: Scans first invoice, sees auto-generated journal entry, posts to ledger
- Week 1: 50 invoices processed, GST-ready report auto-generated
- Month 1: Submits GSTR-3B using pre-filled data (CA signs off in 1 hour)
- Year 1: All compliance done via AI, CA audit is 2-hour review (saves ₹5L+ vs. traditional)

---

### 5.2 Secondary: CA/CMA Professional Firm

**Name:** Patel & Associates (10–20 client base)

**Current Workflow:**
- Clients send invoices via email/WhatsApp (chaotic)
- Manual data entry into Excel/Tally (10+ hours per client/month)
- Monthly reconciliation calls (2–3 hours each)
- Year-end audit (50–100 hours per client)

**Pain Points:**
1. **Efficiency:** Manual data entry is 70% of audit time
2. **Scalability:** Can't serve more than 20 clients profitably
3. **Evidence:** Documents scattered across email/WhatsApp
4. **Compliance:** Audit evidence not organized
5. **Revenue:** Capped at 20 clients × 50 hours × ₹500/hour = ₹5L/year

**What They Need:**
✅ Client portal with pre-filled GST/TDS data (reduce manual entry by 80%)
✅ Audit evidence auto-organized (images, ledger, hash-chained proof)
✅ Digital signature workflow (blockchain-anchored, immutable)
✅ Bulk client management (serve 50–100 clients)
✅ Revenue per client: ₹2,499/audit (vs. ₹5K+ traditional)

**Use Case:**
- Client uses NEXOVAS → auto-generated evidence in Drive
- CA logs into Verification Portal → reviews all documents, ledgers, reconciliations
- CA clicks *Approve* → digital signature applied, blockchain-anchored
- Audit complete in 2 hours (vs. 20+ hours traditional)
- CA firm revenue: ₹2,499 × 50 clients = ₹1.25Cr annual (repeat business)

---

### 5.3 Tertiary: Enterprise/Large MSME

**Name:** Bhatnagar Manufacturing (₹50Cr+ turnover, 100+ employees)

**Current:** Uses SAP/Tally + 3 accountants + 1 CA firm

**What NEXOVAS Adds:**
✅ VisionCount for warehouse/production audits (real-time inventory)
✅ Multi-location support (10 warehouses, different GST jurisdictions)
✅ Advanced reporting (analytics, profitability by cost center, product line)
✅ Integration with existing ERP (NEXOVAS as audit layer on top)

**Use Case:**
- Warehouse manager scans stock → variance detected → auto-alert to management
- Production line uses VisionCount → WIP tracking, quality checks
- Monthly P&L auto-generated → management dashboard updated real-time

---

## 6. CORE FEATURES (MUST HAVE — v1.0)

### 6.1 Tier 1: Camera Intelligence (VisionCount)

#### Feature 1: Document Scanning & OCR
✅ Photograph invoice → Auto-extract fields (vendor, amount, date, HSN, GST, TDS)
✅ Confidence scoring (if <90%, ask user to confirm)
✅ Save image to user's Google Drive (linked via file ID in DB)
✅ Multi-language support (Hindi, Tamil, Telugu, Marathi, Gujarati)
✅ Evidence metadata (session ID, timestamp, user, geolocation optional)
✅ Barcode scanning (**EAN**-13, **UPC**-A, Code-**128**)

#### Feature 2: Inventory Counting (Scale-Adaptive)
✅ Micro Mode: Count pills/grains/fasteners (0.1–10mm items, 99.2% accuracy)
✅ Small Mode: Count bolts/tools/boxes (10–100mm items, 99.7% accuracy)
✅ Medium Mode: Shelf audit (products visible, 99.9% accuracy)
✅ Macro Mode: Equipment/vehicles (barcode-required, 100% with confirmation)
✅ Variance detection (physical vs. system stock)
✅ Auto-suggest reorder quantities (based on consumption history)
✅ Quality flagging (rust, damage, expiry detected)

#### Feature 3: Barcode/QR Scanning
✅ Auto-fill invoice line items (barcode → product → rate → tax → line total)
✅ IMEI scanning (for electronics, warranty activation)
✅ Product master lookup (match barcode → SKU → price → GST rate)

#### Feature 4: Evidence Capture & Storage
✅ Session ID generated (unique per scanning action)
✅ Images saved to user's Google Drive
✅ Metadata logged (device, GPS location optional, user ID, timestamp)
✅ Linked in database (file ID stored, not actual file)
✅ Evidence accessible from ledger entries (one-click view)

---

### 6.2 Tier 2: Autoclaw Prime Orchestration

#### Feature 5: Document Classification & Routing
✅ Input: Image, PDF, voice, or API call
✅ AI classifier: Identifies doc type (purchase invoice, sales invoice, journal entry, etc.)
✅ Confidence threshold: >90% auto-route, <90% ask user
✅ Output: Task graph (sequence of agent calls)
✅ Ambiguity handling (if unclear, present multiple options)

#### Feature 6: CA-Agent (Complete Disclosure)
✅ Journal entry generation (auto Dr/Cr account selection)
✅ Double-entry validation (Dr = Cr balance check)
✅ GST computation (HSN validation, rate verification, ITC eligibility)
✅ TDS calculation (Section 194C/J/LA/D, threshold checking)
✅ Fraud detection (anomaly scoring 0–100, duplicate detection)
✅ Bank reconciliation (auto-match bank statement with ledger)
✅ Audit trail (immutable logging, hash-chained)
✅ Approval gates (risk-based: auto-approve <₹1K, notify CA ₹1K–₹10K, explicit >₹10K)
✅ Posted ledger (append-only, no edits, immutable)

#### Feature 7: CMA-Agent (Complete Disclosure)
✅ Unit cost calculation (standard costing, FIFO/LIFO/Weighted Avg)
✅ Cost sheet maintenance (per product, per batch)
✅ Variance analysis (material, labor, overhead vs. actual)
✅ Budget vs. actual tracking (monthly, quarterly, annual)
✅ Asset depreciation (straight-line, diminishing value)
✅ Quality cost tracking (defects, rework, waste)
✅ Inventory valuation (automatic on purchase/production/sale)
✅ Cost center allocation (split costs across departments)

#### Feature 8: HR-Agent (Complete Disclosure)
✅ Salary calculation (gross – deductions = net)
✅ PF computation (12% + 1.61%, with caps)
✅ ESI calculation (if applicable)
✅ Professional tax (state-wise rates)
✅ TDS on salary (Section 192)
✅ Leave accrual (EL, SL, CL per employee, per month)
✅ Attendance integration (biometric, manual, camera-based)
✅ Form 16 generation (tax certificate)
✅ Gratuity valuation (exit calculation)
✅ Exit processing (FNF, statutory compliance)

#### Feature 9: CRM-Agent (Complete Disclosure)
✅ Lead capture (web form, email, WhatsApp, API)
✅ Lead scoring (RFM, industry, company size, engagement)
✅ Opportunity tracking (Qualified → Proposal → Negotiation → Won/Lost)
✅ Quotation generation (auto-pricing, terms, validity)
✅ Sales order processing (validate stock, create delivery note)
✅ Customer segmentation (RFM, behavioral, geographic)
✅ Churn prediction (risk score, engagement alerts)
✅ Marketing automation (email, SMS, WhatsApp)
✅ Customer portal (self-service invoices, payments, orders)
✅ Retention analysis (lifetime value, repeat rate)

#### Feature 10: PM-Agent (Complete Disclosure)
✅ Project planning (WBS, milestones, deliverables)
✅ Resource allocation (skill-based, availability-based)
✅ Gantt chart generation (critical path)
✅ Timesheet management (billable hours)
✅ Budget tracking (cost vs. actual, forecast)
✅ Milestone completion (on-time, at-risk, delayed)
✅ Resource utilization (% billable, idle alerts)
✅ Project profitability (P&L by project)
✅ Delivery schedule tracking

#### Feature 11: CS-Agent (Complete Disclosure)
✅ Ticket management (auto-categorization, priority routing)
✅ SLA monitoring (breach alerts, escalation)
✅ Knowledge base (FAQ, self-service)
✅ Returns management (approval, refund processing)
✅ Warranty validation (serial number, entitlement)
✅ Complaint analysis (root cause, preventive action)
✅ Customer feedback (survey, satisfaction scoring)
✅ Escalation management (time-bound, visibility)

---

### 6.3 Tier 3: Indian Compliance Automation

#### Feature 12: GST Compliance
✅ HSN code validation (correct per item type)
✅ GST rate application (0%, 5%, 12%, 18%, 28%, exempted)
✅ Tax computation (per-line + aggregation)
✅ GSTR-1 generation (outward supplies, auto-populated)
✅ GSTR-2B reconciliation (match inputs to purchases)
✅ GSTR-3B filing (compute ITC, payable, file ready)
✅ GSTR-9 annual return (auto-summary)
✅ E-way bill generation (goods movement documentation)
✅ E-invoice generation (for B2B, >₹5Cr turnover)
✅ Input tax credit tracking (eligible vs ineligible)

#### Feature 13: Income Tax Automation
✅ TDS calculation (194C, 194J, 194LA, 194D)
✅ TDS payment scheduling (13th, 26th, 31st monthly)
✅ Form 26Q generation (quarterly summary)
✅ Form 24Q generation (annual TDS)
✅ Advance tax scheduling (15%, 50%, 75%, 100% dates)
✅ ITR preparation (Schedule NA/DA/CFL, auto-fill)
✅ Tax saving recommendations (80C/D/E/G)
✅ Presumptive taxation (Section 44AD, 8% auto-calculation)

#### Feature 14: Corporate Compliance (MCA/ROC)
✅ ROC filing tracking (e-form due dates)
✅ AGM compliance (meeting schedule, notice, minutes)
✅ Director KYC management (updates, renewals)
✅ Charge registration (property/asset mortgage)
✅ Compliance calendar (ROC, AGM, board meetings)
✅ Document management (certificates, resolutions)

#### Feature 15: Labor Law Compliance
✅ PF contribution (computation, payment deadlines)
✅ ESI contribution (if applicable)
✅ Professional tax (state-wise rates, monthly)
✅ Minimum wage validation (state updates, breach alerts)
✅ Bonus calculation (Payment of Bonus Act, %)
✅ Gratuity valuation (at exit, statutory)
✅ Leave compliance (encashment limits, carry-forward)
✅ Compliance calendar (PF/ESI/PT submission, updates)

#### Feature 16: Banking & Payment Compliance
✅ RBI UPI 2.0 integration (personal UPI accounts, merchants)
✅ Payment splitting (₹2,000/transaction limit enforcement)
✅ Cash reporting (Section 269ST, >₹2L/day alerts)
✅ TDS on cash withdrawal (Section 194N, >₹1Cr annual)
✅ Digital payment tracking (% digital, compliance reporting)
✅ Bank reconciliation (auto-matching, statement import)

---

### 6.4 Tier 4: Industry-Specific Suites

#### Module 17: Retail & Kirana
✅ Camera billing (scan 5 items → auto-invoice in 3 seconds)
✅ Inventory management (500+ SKUs, expiry tracking)
✅ GST composition scheme support (1% tax cap)
✅ Personal UPI integration (merchant's own account)
✅ Daily P&L auto-generated
✅ Reorder automation (below-threshold alerts)

#### Module 18: Manufacturing
✅ BOM (Bill of Materials) management
✅ Job costing (per-product cost tracking)
✅ Production planning (MRP-style suggestions)
✅ Maintenance scheduling (preventive)
✅ Work order management (production orders)
✅ Quality inspection (defect tracking, cost of poor quality)

#### Module 19: Pharmacy
✅ Pill counting (through bottles, 99.2% accuracy)
✅ Batch & expiry tracking (cold-chain compliance)
✅ Drug license management (renewals)
✅ Narcotics register (Schedule H/X tracking)
✅ Prescription scanning (auto-billing)
✅ GST 5%/12% auto-application (per drug type)

#### Module 20: Agriculture
✅ Seed/produce counting (density estimation)
✅ Produce grading (AI by size, color, defects)
✅ Mandi integration (live prices, auto-invoicing)
✅ PM-KISAN documentation (automated)
✅ Crop insurance tracking
✅ Soil health card management

#### Module 21: Construction
✅ Material counting (bricks, bags, steel)
✅ Progress monitoring (photo-based % completion)
✅ Labor attendance (facial recognition)
✅ TDS 1% auto-deduction (contractor payments)
✅ Retention money tracking
✅ Safety compliance (PPE detection)

#### Additional Modules (22–28):
22. **Hospitality** (table billing, inventory, recipe costing)
23. **Electronics & Mobile** (IMEI scanning, warranty, exchange valuation)
24. **Jewelry** (piece counting, hallmark OCR, making charges)
25. **Waste Management** (material identification, segregation, scrap invoicing)
26. **FMCG/Distribution** (multi-warehouse, route optimization, dealer management)
27. **Services/Consulting** (timesheet billing, project costing, resource planning)
28. **Healthcare** (clinic management, prescription management, inventory)

---

## 7. NICE-TO-HAVE FEATURES (v1.5+)

- Multi-currency support (USD, EUR, GBP, AED, SGD)
- Advanced analytics (predictive revenue, churn forecasting)
- AI chat assistant (GPT-4 for instant ERP queries)
- Marketplace integrations (Amazon, Flipkart, Shopify seller sync)
- Tally import (bulk data migration)
- Custom reports builder (drag-drop UI)
- Native mobile app (iOS/Android, in addition to PWA)
- Voice commands ("Show me today's P&L")
- Multi-tenant agency portal (CA firms managing 100+ clients)
- Blockchain integration (public verification of audit reports)
- Video tutorials for all features
- Mobile-first reporting (PDF generation on device)

---

## 8. OUT OF SCOPE (v1.0 — NOT INCLUDED)

❌ Artificial autonomous ledger posting (all entries require approval gate)
❌ Guaranteed *infinite free storage* (marketing claim, must be realistic)
❌ Full ERP replacement for enterprises >₹100Cr (NEXOVAS is for MSMEs)
❌ Offline-only mode (limited offline capture, sync on connection)
❌ Real-time 3D warehouse mapping
❌ Blockchain integration (hash-chaining is internal, not public)
❌ BI/analytics suite (basic dashboards only in v1)
❌ Customs/export documentation (India-focused, other countries in v2+)
❌ AI-to-AI direct transactions (all require human approval)

---

## 9. USER STORIES (MUST HAVE FUNCTIONALITY)

### Story 1: Invoice-to-Posting (Retail Kirana)
As a Kirana shop owner, I want to scan 5 customer items with my phone camera, So that I get an auto-generated invoice with GST calculated, accept UPI payment, and see the transaction posted to my ledger in real-time, Because currently I manually enter each item (10 minutes per bill) and manually track sales.

Acceptance Criteria: ✅ Scan 5 items in <5 seconds ✅ Invoice generated with customer name, date, HSN, GST rates, total ✅ UPI QR displayed on screen (auto-split if >₹2,000) ✅ Payment confirmation received in <30 seconds ✅ Ledger entry posted automatically (Dr Bank, Cr Sales, Cr GST) ✅ Evidence images saved to my Google Drive ✅ Daily P&L available next morning (auto-generated)


### Story 2: GST Filing (Every MSME)
As a business owner, I want NEXOVAS to automatically prepare my GSTR-1/3B using invoices I've entered, So that I can file GST returns without manual extraction, Because currently my accountant spends 8 hours extracting data per return.

Acceptance Criteria: ✅ GSTR-1 auto-populated from all sales invoices ✅ GSTR-2B reconciliation with purchase invoices highlighted ✅ GSTR-3B inputs pre-calculated (ITC, payable, etc.) ✅ One-click file export (JSON format for GST portal) ✅ 100% accurate (matches manual calculation when reviewed) ✅ Due date reminder (email 3 days before deadline)


### Story 3: Payroll Processing (HR Manager)
As an HR manager, I want to enter employee attendance once, and have NEXOVAS auto-calculate salary, PF, ESI, PT, TDS, and generate salary slips, So that I don't have to manually compute 5+ deductions per employee per month.

Acceptance Criteria: ✅ Mark attendance (biometric or manual) ✅ Auto-calculate gross pay (base + HRA + special allowance) ✅ Auto-deduct PF (12% employee + 1.61% employer) ✅ Auto-deduct ESI (if applicable) ✅ Auto-deduct PT (state-wise rate) ✅ Auto-compute TDS (Section 192) ✅ Generate salary slip (employee-ready PDF) ✅ Post to ledger (Dr Salary Expense, Cr Bank, Cr PF Liability, Cr TDS Payable) ✅ Payment file generated (ready for bank upload)


### Story 4: Stock Audit (Warehouse Manager)
As a warehouse manager, I want to photograph a bin of fasteners and get an instant count + variance report, So that I don't spend 2 hours manually counting with a clipboard.

Acceptance Criteria: ✅ Photograph bin of 847 fasteners ✅ AI counts and classifies by type (423 M8 nuts, 298 bolts, 126 washers) ✅ Detect quality issues (12 rusted items flagged) ✅ Compare vs system stock (847 physical vs 1,000 system = -15.3% variance) ✅ Auto-generate variance journal entry (Dr Expense, Cr Inventory) ✅ Generate reorder suggestion (M8 bolts below reorder level) ✅ All evidence (images, report) saved to Drive


### Story 5: Audit Prep (CA/CMA Reviewer)
As a CA professional, I want to log into NEXOVAS Verification Portal and see audit-ready data (trial balance, reconciliations, evidence images, hash-chained ledger), So that I can complete the annual audit in 2 hours instead of 20 hours.

Acceptance Criteria: ✅ Portal login (biometric + email verify) ✅ Trial balance auto-generated (all accounts, balances) ✅ GST reconciliation (GSTR-1 vs GSTR-2B, highlighted variances) ✅ Bank reconciliation (statement vs ledger, unmatched items noted) ✅ All evidence accessible (one-click to Drive images, PDFs) ✅ Digital signature workflow (click Approve → blockchain-anchored) ✅ Audit report generated (forms, certificates, compliance checklist) ✅ Audit complete marker (client status updated)


### Story 6: Payment Splitting (₹2,000+ RBI Compliance)
As a customer buying a ₹5,500 LED TV, I want to scan one QR code and make 3 UPI payments (₹2,000 + ₹2,000 + ₹1,500), without manually initiating separate transactions, So that I don't violate RBI per-transaction limits and the merchant gets paid instantly.

Acceptance Criteria: ✅ Invoice total: ₹5,500 ✅ Display: "Will be split into 3 UPI transactions" ✅ Customer scans single QR code ✅ 3 transactions processed sequentially (RRN-001, RRN-002, RRN-003) ✅ All 3 transactions complete in <20 seconds ✅ Real-time display of transaction status (1/3, 2/3, 3/3 complete) ✅ All 3 journal entries posted (Dr Bank ₹2K, ₹2K, ₹2K, ₹1.5K) ✅ Invoice marked as "Fully Paid"

---

## 10. SUCCESS METRICS (HOW WE KNOW IT'S WORKING)

### 10.1 User Adoption Metrics

- ✅ **Signups:** 100 in week 1, 1,000 in month 1, 10,000 by month 6
- ✅ **DAU (Daily Active Users):** >30% of signups
- ✅ **Retention Rate:** >70% month-over-month
- ✅ **Feature Usage:** >80% of users use VisionCount within first week
- ✅ **Time to First Invoice:** <24 hours from signup
- ✅ **Onboarding Completion:** >80% complete within 7 days

### 10.2 Transaction Volume

- ✅ **Daily Transactions:** 100,000+ invoices/day by month 3
- ✅ **Invoice Accuracy:** >99.5% (matching manual review)
- ✅ **Error Rate:** <0.1% (auto-corrected or flagged)
- ✅ **Compliance Filings:** 100% GSTR-3B filings from NEXOVAS data (zero manual re-entry)
- ✅ **Average Processing Time:** <2 seconds per invoice

### 10.3 Business Metrics

- ✅ **Revenue:** ₹999/month × 10,000 users = ₹10Cr ARR (year 2)
- ✅ **Gross Margin:** >85% (BYOS model eliminates storage costs)
- ✅ **CAC (Customer Acquisition Cost):** <₹200 (organic, affiliate, content)
- ✅ **LTV (Lifetime Value):** >₹20,000 (36+ month average customer life)
- ✅ **LTV/CAC Ratio:** >100:1 (highly profitable)

### 10.4 Product Quality

- ✅ **VisionCount Accuracy:**
  - Micro-mode: 99.2%+ (vs 95% manual counting)
  - Small-mode: 99.7%+
  - Medium-mode: 99.9%+
  - Macro-mode: 100% (with barcode confirmation)
- ✅ **Ledger Posting Accuracy:** 100% (Dr = Cr, no imbalances posted)
- ✅ **Audit Trail Integrity:** 100% (no entries deleted, hash-chain verified)
- ✅ **AI Decision Confidence:** >95% average (fraud probability <0.0000001%)

### 10.5 Compliance Metrics

- ✅ **GST Filing Accuracy:** 100% match with manual audit
- ✅ **TDS Calculation Accuracy:** 100% (matches official tables)
- ✅ **Audit Turnaround Time:** 2 hours (vs 20+ traditional)
- ✅ **Penalty/Audit Issues:** <1% of users (vs 30–50% traditional MSMEs)
- ✅ **Compliance Calendar Hit Rate:** 100% (no missed deadlines)

### 10.6 Customer Satisfaction

- ✅ **NPS Score:** >50 (benchmark: 30–40 for SaaS)
- ✅ **CSAT:** >85% (customer satisfaction rating)
- ✅ **Support Ticket Resolution:** >95% in <24 hours
- ✅ **Churn Rate:** <5% per month
- ✅ **Net Promoter Referrals:** >40% of new users from referrals

---

## 11. PRICING & PACKAGES (NEXOVAS v1.0)

### 11.1 Free Tier (Forever Free for Micro-Businesses)

- **Price:** ₹0
- **Limit:** Up to 100 invoices/month
- **Features:**
  - VisionCount basic scanning
  - Manual journal entry creation
  - Basic reports (P&L, balance sheet)
  - No GST filing assistance
  - No compliance automation
  - No support (community forum only)
- **Target:** Freelancers, micro-traders testing platform

### 11.2 Starter Tier (Small Kirana/Retail)

- **Price:** ₹999/month (auto-renew, cancel anytime)
- **Limit:** Up to 500 invoices/month, 1 user
- **Features:**
  - VisionCount (all modes)
  - CA-Agent (journal entry auto-posting, GST draft prep)
  - Basic reports + daily P&L
  - GST composition scheme support
  - Personal UPI integration
  - Evidence storage (user's Google Drive, unlimited)
  - Email support (48-hour response)
- **Target:** Small kirana stores, freelancers, traders
- **Margin:** ₹999 revenue – ₹50 DB cost = ₹949 margin (95%)

### 11.3 Professional Tier (Growing Business)

- **Price:** ₹4,999/month
- **Limit:** Unlimited invoices, 5 users, 50 employees (HR)
- **Features:**
  - All Starter features
  - All 6 Agents (CA, CMA, HR, CRM, PM, CS)
  - Payroll processing (auto-calculation, statutory deductions)
  - GST GSTR-1/3B auto-filing prep
  - TDS calculation + Form 26Q prep
  - Multi-location support (3 locations)
  - Advanced reports (cost analysis, variance, profitability)
  - CA Verification Portal (1 annual audit included)
  - Priority email support (24-hour response)
  - Dedicated onboarding (2 hours)
- **Target:** Growing MSMEs, manufacturing units, trading houses
- **Margin:** ₹4,999 – ₹500 cost = ₹4,499 margin (90%)

### 11.4 Enterprise Tier (Large MSME/Manufacturing)

- **Price:** ₹24,999/month
- **Limit:** Unlimited everything
- **Features:**
  - All Professional features
  - Unlimited locations
  - Unlimited users
  - Custom integrations (Tally, QuickBooks, ERPNext)
  - Advanced analytics + BI dashboards
  - CA Verification Portal (unlimited audits/year)
  - API access (REST + GraphQL)
  - White-label option (for CA firms reselling)
  - Dedicated account manager
  - Phone + email support (4-hour response)
  - Custom training (4 hours/month)
- **Target:** Large MSMEs (₹50Cr+ turnover), manufacturing, enterprises
- **Margin:** ₹24,999 – ₹3,000 cost = ₹21,999 margin (88%)

### 11.5 À La Carte Services (Additional Charges)

- **CA/CMA Audit Verification:** ₹2,499/audit (digital signature + blockchain-anchored)
- **Custom Report Development:** ₹5,000 per report
- **Data Migration (from Tally/Zoho):** ₹10,000–₹50,000 (depends on volume)
- **Integration Setup:** ₹2,000 per integration
- **Compliance Calendar Setup:** ₹5,000 (configure all GST/Tax/Labor deadlines)
- **Advanced Training Session:** ₹1,000/hour (per team member)

### 11.6 Pricing Strategy

- **Freemium Model:** Free tier converts to Starter (30% conversion rate target)
- **Stickiness:** Monthly subscriptions (auto-renew), no long-term contracts
- **Land & Expand:** Start Starter (₹999) → upgrade to Professional (₹4,999) as business grows
- **CAC Payback:** <2 months (LTV/CAC >100:1)
- **Gross Margin:** 85–95% across all tiers (BYOS model advantage)

---

## 12. NEXOVAS TARGET: 10,000 USERS BY END OF YEAR 1

### 12.1 Growth Milestones

| Month | Signups | Total Users | Revenue (Monthly) | Status |
|-------|---------|-------------|-------------------|--------|
| Month 1 | 100 | 100 | ₹50K | MVP launch |
| Month 2 | 300 | 400 | ₹2L | Word-of-mouth |
| Month 3 | 500 | 900 | ₹4.5L | Product review features |
| Month 6 | 1,000 | 3,500 | ₹15L | CA firm partnerships |
| Month 9 | 2,000 | 6,500 | ₹30L | Industry-specific suites launch |
| Month 12 | 3,500 | 10,000 | ₹50L | Scale phase complete |

### 12.2 ARR Projection (Year 1 Close)

- **10,000 users avg mix:**
  - 40% Free (0 revenue)
  - 40% Starter (₹999/month)
  - 15% Professional (₹4,999/month)
  - 5% Enterprise (₹24,999/month)

- **Revenue breakdown:**
  - Starter: 4,000 × ₹999 × 12 = ₹4.8Cr
  - Professional: 1,500 × ₹4,999 × 12 = ₹9Cr
  - Enterprise: 500 × ₹24,999 × 12 = ₹1.5Cr
  - Audit services: 500 audits × ₹2,499 = ₹1.25Cr
  - **Total Year 1 ARR: ₹16.55Cr** (conservative estimate)

### 12.3 Year 2 Projections

- **Users:** 25,000–30,000 (3x growth)
- **ARR:** ₹50Cr+ (3x growth)
- **Gross Margin:** 85%+ (₹42.5Cr+ profit)
- **Expansion:** International (Southeast Asia, UK, US)
- **New Modules:** Advanced analytics, blockchain, IoT integrations

---

## 13. INVESTMENT & RUNWAY

### 13.1 Seed Funding Required (₹1.25Cr / $150K USD)

| Category | Amount | Justification |
|----------|--------|---------------|
| Engineering (3 FTE) | ₹50L | Backend (FastAPI), Frontend (Next.js), DevOps |
| AI/ML (VisionCount training) | ₹20L | TensorFlow Lite models, dataset curation, edge deployment |
| Product & Design | ₹15l | PRD refinement, UI/UX design, prototyping |
| Compliance & Legal | ₹10l | GST/TDS/Labor law expertise, regulatory review |
| Marketing & Sales | ₹15l | Content marketing, affiliate, Google Ads, CA partnerships |
| Infrastructure & Cloud | ₹5l | AWS, Supabase, Google Cloud, monitoring |
| Legal & Admin | ₹10l | Incorporation, contracts, insurance, hiring |
| Contingency | ₹5l | Unexpected costs, buffer |
| **Total (12-month runway)** | **₹1.25Cr** | **MRR breakeven by month 8–9** |

### 13.2 Profitability Path

- **Month 1–3:** Negative (engineering, setup, product refinement)
- **Month 4–6:** Approaching break-even (first revenues, 100–300 users)
- **Month 7–9:** Break-even achieved (revenue offsets operating costs)
- **Month 10–12:** Positive cash flow (revenue > costs, compound growth)
- **Year 2:** Highly profitable (ARR ₹50Cr > operating costs ₹1.5Cr/year)

---

## 14. COMPETITIVE ADVANTAGES

### 14.1 vs Tally (Market Leader in India)

| Feature | Tally | NEXOVAS | Winner |
|---------|-------|---------|--------|
| **Mobile-first** | ❌ Desktop-only | ✅ Mobile + Web | NEXOVAS |
| **Camera scanning** | ❌ No | ✅ VisionCount AI | NEXOVAS |
| **Cloud sync** | ❌ Local only | ✅ Google Drive + Supabase | NEXOVAS |
| **AI automation** | ❌ None | ✅ Autoclaw Prime (6 agents) | NEXOVAS |
| **Compliance automation** | Partial | ✅ Complete (GST/TDS/Labor) | NEXOVAS |
| **Cost** | ₹25K setup | ₹999/month | NEXOVAS (flexible pay) |
| **Data ownership** | Vendor lock-in | ✅ User's Google Drive | NEXOVAS |
| **Per-user scalability** | ₹1K/user | ₹999/month flat | NEXOVAS |

### 14.2 vs Zoho Books (Cloud Competitor)

| Feature | Zoho | NEXOVAS | Winner |
|---------|-----|---------|--------|
| **Per-user cost** | ₹4K+/month | ₹999/month Starter | NEXOVAS (4–10x cheaper) |
| **Storage cost** | Extra charge | ₹0 (BYOS) | NEXOVAS |
| **Indian compliance** | Basic | ✅ Complete (21 modules) | NEXOVAS |
| **AI automation** | Limited | ✅ Complete (Autoclaw Prime) | NEXOVAS |
| **Mobile camera** | ❌ No | ✅ VisionCount | NEXOVAS |
| **Offline capability** | Limited | ✅ Full offline mode | NEXOVAS |
| **Multi-location** | ₹2K/location | Included | NEXOVAS |
| **Audit trail** | Basic | ✅ Blockchain-anchored | NEXOVAS |

### 14.3 Why NEXOVAS Wins

1. **Price:** ₹999 vs ₹4K–₹10K alternatives (4–10x cheaper)
2. **Mobile-First:** Camera as interface (vs manual data entry)
3. **Data Ownership:** User's Google Drive, not NEXOVAS servers (GDPR compliant)
4. **Compliance:** 21 modules, 500+ DocTypes (complete India coverage)
5. **AI Orchestration:** Autoclaw Prime (6 professional agents, not generic AI)
6. **Audit Ready:** Hash-chained ledger, CA portal, 2-hour audit (vs 20+ hours)
7. **Zero Storage Cost:** BYOS model = 90% gross margin (vs 60–70% traditional SaaS)
8. **Industry Coverage:** 28+ industry-specific modules (Retail, Manufacturing, Pharmacy, etc.)

---

## 15. GO-TO-MARKET STRATEGY

### 15.1 Phase 1: Foundation (Months 1–3)
- **Launch:** Closed beta with 50 kirana store owners
- **Focus:** Product-market fit validation, bug fixes
- **Target:** NPS >40, retention >70%
- **CAC:** Organic only (founder network)

### 15.2 Phase 2: Expansion (Months 4–6)
- **Launch:** Public beta on App Store + Google Play
- **Marketing:** Content (blog posts on GST, TDS, payroll automation)
- **Partnerships:** CA firm partnerships, kirana aggregators
- **Target:** 3,000 users, ₹15L MRR

### 15.3 Phase 3: Scale (Months 7–12)
- **Expansion:** Enterprise sales (direct)
- **Product:** Industry-specific templates (Pharmacy, Manufacturing, etc.)
- **Partnerships:** CRM tools, payment gateways, banking integrations
- **Target:** 10,000 users, ₹50L MRR

### 15.4 Phase 4: Internationalization (Year 2)
- **Expansion:** Southeast Asia (Thailand, Vietnam), UK, US
- **Localization:** Local compliance, local payment methods
- **Target:** 30,000 users, ₹1.5Cr+ MRR

---

## 16. BOARD APPROVAL CHECKLIST

- ✅ Problem statement validated (surveys: 500+ MSME owners)
- ✅ Product-market fit confirmed (early users showing 50+ NPS)
- ✅ Technical feasibility proven (MVP built, VisionCount accuracy validated)
- ✅ Compliance framework designed (CA review pending)
- ✅ Funding strategy defined (Seed ₹1.25Cr, Series A ₹5Cr target)
- ✅ Team identified (CEO, CTO, Product Lead, CA, Compliance Officer)
- ✅ GO-TO-MARKET plan refined (3-phase approach, CA partnerships)
- ✅ Legal structure ready (Private Limited Company registered)
- ✅ Intellectual property protected (Patents filed for VisionCount, Autoclaw)

---

## FINAL STATEMENT

**NEXOVAS ERP** is not just software. It's a **movement** to democratize professional-grade accounting and compliance for every Indian MSME.

*"The camera is the enterprise. The AI is the professional. The phone is the accountant."*

**Status:** AUTHORIZED FOR IMMEDIATE DEVELOPMENT

**Target Launch:** Week 1, 2027

**Expected Impact:** 10,000 MSMEs with professional accounting within 12 months
DOCUMENT 02: TRD.md — TECHNICAL REQUIREMENTS DOCUMENT
# NEXOVAS ERP — Technical Requirements Document (TRD)
## Complete Technology Stack & Architecture Blueprint
### Version: FINAL v3.0 | Date: October 7, 2026

---

## 1. TECHNOLOGY STACK OVERVIEW

### 1.1 Frontend

**Platform:** Next.js 14 + TypeScript + Tailwind CSS

**Justification:**
- Mobile-responsive PWA (works iOS, Android, Web)
- Server-side rendering (fast page loads, SEO)
- API routes (can run backend on same service)
- Vercel hosting (zero-config deployment)
- Edge functions (low-latency compliance checks)

**Key Libraries:**
- **React 18:** Component library, hooks, state management
- **TanStack Query:** Server state management, real-time updates
- **Zod:** Schema validation (request/response contracts)
- **Zustand:** Client state (UI state, temporary form data)
- **Lucide Icons:** Icon library (35+ financial/inventory icons)
- **Shadcn/ui:** Component library (tables, modals, forms)
- **Recharts:** Charts & graphs (P&L, trends, variance analysis)
- **Expo:** React Native (for iOS/Android native apps)

**Mobile App Stack:**
- **Expo:** Cross-platform mobile development
- **React Native Vision Camera:** TensorFlow Lite integration for scanning
- **SQLite:** Local offline database on device
- **Realm:** Offline-first sync engine

---

### 1.2 Backend

**Framework:** FastAPI (Python) + Supabase Edge Functions

**Justification:**
- CPU-only (no GPU required, free tier viable)
- Zero infrastructure management (Edge Functions)
- REST + GraphQL support
- Built-in async/await (high concurrency)
- Swagger documentation (auto-generated API docs)
- CORS, rate limiting, authentication built-in

**Key Libraries:**
- **FastAPI:** Web framework
- **Pydantic:** Data validation (ZOD equivalent)
- **SQLAlchemy:** ORM (database queries)
- **python-jose:** JWT token generation/validation
- **passlib:** Password hashing (bcrypt)
- **celery:** Background job processing
- **redis:** Job queue + caching
- **python-multipart:** File uploads
- **httpx:** External API calls (synchronous)

**Deployment:**
- **Vercel:** Frontend + API routes (Next.js)
- **Railway/Fly.io:** Backend services (FastAPI)
- **Supabase:** PostgreSQL + Edge Functions
- **Redis Cloud:** Session/queue management

---

### 1.3 Database

**Primary:** PostgreSQL via Supabase

**Justification:**
- ACID compliance (financial data integrity)
- Row-Level Security (RLS) policies (per-tenant isolation)
- JSON support (flexible schema)
- Full-text search (invoice search, customer lookup)
- Realtime subscriptions (live P&L updates)
- Automatic backups (Supabase-managed)

**Database Features:**
- **Tables:** 500+ DocTypes (Accounts, Stock, Selling, Buying, HR, etc.)
- **Relationships:** Foreign keys with cascading deletes
- **Indexes:** B-tree on frequently queried columns (user_id, company_id, date)
- **Partitioning:** By month (transactions, GL entries, stock ledger)
- **Search:** Full-text indexes on vendor name, customer name, invoice number

**Backup Strategy:**
- Automatic daily backups (Supabase handles)
- User can export to their Google Drive
- Point-in-time recovery (30-day retention)

---

### 1.4 Authentication & Authorization

**Authentication Method:** Supabase Auth (JWT tokens + OAuth)

**Supported Providers:**
- Email + Password (basic login)
- Google OAuth (social sign-in)
- Apple ID (for iOS)

**JWT Token Structure:**
```json
{
  "sub": "user_id",
  "email": "user@example.com",
  "role": "user|admin|ca",
  "company_id": "company_id",
  "permissions": ["create_invoice", "view_ledger"],
  "exp": 3600
}
Authorization Model:

Row-Level Security (RLS): Users can only see their own company data
Roles: user (basic), admin (company setup), ca (auditor)
Permissions: Granular (create_invoice, approve_invoice, view_ledger, etc.)
Session Management:

Access Token: 1-hour expiry (short-lived)
Refresh Token: 30-day expiry (long-lived)
Cookie Storage: Secure HTTP-only cookies (CSRF protected)
1.5 File Storage
Provider: Google Drive (Bring Your Own Storage - BYOS)

Justification:

₹0 cost to NEXOVAS (15GB free per user)
User owns data (not vendor lock-in)
Automatic backup + versioning
Shareable (share audit evidence with CA)
File Organization:

My Drive/
└── NEXOVAS_ERP_Data/
    ├── invoices/
    │   ├── 2026-10/
    │   │   ├── INV-001.pdf
    │   │   ├── INV-001.jpg (camera scan)
    │   │   └── INV-001.json (extracted data)
    │   └── 2026-11/
    ├── ledger/
    │   ├── 2026-10.csv (exported ledger)
    │   └── 2026-11.csv
    ├── reports/
    │   ├── GST-GSTR-1-Oct2026.json
    │   ├── GSTR-3B-Oct2026.json
    │   ├── TDS-26Q-Q2-2026.json
    │   └── P&L-Oct2026.pdf
    └── backups/
        ├── full-backup-2026-10-01.zip
        └── incremental-2026-10-15.zip
API Integration:

OAuth 2.0: User grants NEXOVAS permission to access Drive
Google Drive API v3: Upload files, list files, download files
File IDs: Store file ID in DB (not actual file content)
Access Control: User can revoke access anytime (uninstall app from Drive)
1.6 Email & Notifications
Email Service: SendGrid or Resend

Use Cases:

Invoice delivery (customer receives invoice PDF)
GST filing deadline (email 3 days before)
TDS payment due (email 3 days before)
PF/ESI submission due (email 3 days before)
Monthly P&L summary (auto-sent on 1st of month)
Bank reconciliation variance alert (if >5% difference)
Fraud alert (if transaction confidence < 90%)
SMS: Twilio (for urgent alerts)

WhatsApp: WhatsApp Business API (for customer invoices)

In-App Notifications: WebSockets (real-time alerts)

1.7 Payment Gateway Integration
Primary: Razorpay (for subscription billing + UPI)

Secondary: Stripe (for international expansion)

Capabilities:

Subscription billing (auto-renew monthly)
UPI QR code generation (for retail customers)
Payment splitting (₹2,000 limit enforcement)
Invoice tracking (payment status)
Refund processing
Reconciliation (match payments to subscriptions)
Webhooks:

payment.authorized → activate subscription
payment.failed → send retry email
invoice.paid → send receipt email
invoice.expired → send renewal notice
1.8 Third-Party Integrations
Banking:

Razorpay API (payments, UPI, settlement)
NEFT/RTGS (via bank APIs, if available)
Bank statement import (Plaid API for statement aggregation)
Government:

GST Portal API (filing GSTR-1/3B, if available)
MCA e-filing API (company compliance)
TDS Portal API (Form 26Q submission, if available)
ERP Integration:

ERPNext API (import/export data)
Tally export format (CSV, XML)
QuickBooks API (for international expansion)
Communication:

Slack integration (compliance alerts)
Email (SendGrid, Resend)
SMS (Twilio)
WhatsApp (Twilio WhatsApp Business)
1.9 AI/ML Models
VisionCount - Document Scanning:

Model: Google MLKit Vision (free, on-device)
Accuracy: 95%+ OCR accuracy (tested on 10K invoices)
Deployment: TensorFlow Lite (on-device inference)
Languages: Hindi, Tamil, Telugu, Marathi, Gujarati, English
Latency: <2 seconds per page (on mobile device)
VisionCount - Inventory Counting:

Model: Custom YOLOv8 (trained on item images)
Accuracy: 99.2%+ (micro-mode), 99.9%+ (macro-mode)
Deployment: ONNX Runtime (on-device inference)
Training Data: 100K+ images (various lighting, angles)
Latency: <1 second per count
Autoclaw Prime - AI Decision Engine:

Architecture: Distributed decision tree + heuristics (no neural networks)
Processing: 4.7M decisions/second (CPU-only)
Confidence Scoring: 0.0 to 1.0 (fraud probability <0.0000001%)
Decision Protocol: Observation → Pattern Recognition → Hypothesis → Evidence → Alternative Analysis → Judgment → Confidence Scoring → Blockchain Anchor
Agents: 6 specialized agents (CA, CMA, HR, CRM, PM, CS)
Autoclaw Prime - Fraud Detection:

Algorithm: Anomaly scoring using statistical models
Features: Transaction amount, vendor history, time-of-day, day-of-week, user location, invoice patterns
Accuracy: 99.5%+ (tested on 1M transactions)
Latency: <100ms per transaction
1.10 API Specification
REST API Base URL:

Production: https://api.nexovas.com/v1
Staging: https://staging-api.nexovas.com/v1
Local: http://localhost:8000/v1
Core Endpoints:

Authentication:

POST /auth/signup (email, password)
POST /auth/login (email, password)
POST /auth/refresh (refresh token)
POST /auth/logout
POST /auth/reset-password (email)
Invoices:

GET /invoices (list all invoices, paginated)
POST /invoices (create invoice)
GET /invoices/{id} (get single invoice)
PUT /invoices/{id} (update invoice)
DELETE /invoices/{id} (soft delete)
POST /invoices/{id}/post (post to ledger)
POST /invoices/{id}/unpost (remove from ledger)
GET /invoices/{id}/evidence (get attached images)
POST /invoices/scan (camera scan OCR)
Ledger:

GET /ledger (trial balance)
GET /ledger/accounts/{account_id} (ledger for account)
GET /ledger/entries (all GL entries)
POST /ledger/entries (manual journal entry)
DELETE /ledger/entries/{id} (soft delete, if in draft)
Compliance:

GET /compliance/gst/gstr1 (GSTR-1 data)
GET /compliance/gst/gstr2b (GSTR-2B data)
GET /compliance/gst/gstr3b (GSTR-3B data)
GET /compliance/tds/26q (Form 26Q data)
GET /compliance/calendar (upcoming deadlines)
POST /compliance/validate (validate GST/TDS)
Payroll:

GET /payroll/salary-slips (list salary slips)
POST /payroll/salary-slips (generate salary slip)
GET /payroll/attendance (attendance records)
POST /payroll/attendance (mark attendance)
GET /payroll/compliance/pf (PF calculation)
GET /payroll/compliance/esi (ESI calculation)
Reports:

GET /reports/p-and-l (Profit & Loss)
GET /reports/balance-sheet (Balance Sheet)
GET /reports/cash-flow (Cash Flow)
GET /reports/trial-balance (Trial Balance)
GET /reports/gst-summary (GST Summary)
GET /reports/variance-analysis (Cost Variance)
GraphQL Schema (alternative to REST):

type Query {
  invoices(filter: InvoiceFilter!): [Invoice!]!
  invoice(id: ID!): Invoice
  ledger(account_id: ID!): [GLEntry!]!
  gstrData(month: Int!): GSTRData
  salarySlips(employee_id: ID!): [SalarySlip!]!
  reports(type: ReportType!): Report
}

type Mutation {
  createInvoice(input: CreateInvoiceInput!): Invoice
  postInvoice(id: ID!): Invoice
  generateSalarySlip(input: SalarySlipInput!): SalarySlip
  validateCompliance(type: ComplianceType!): ComplianceStatus
}

type Subscription {
  invoiceCreated: Invoice
  ledgerUpdated: GLEntry
  complianceAlert: Alert
  payrollUpdated: PayrollStatus
}
2. ENVIRONMENT VARIABLES
Required (Production):

# Database
DATABASE_URL=postgresql://user:password@host:port/nexovas
DATABASE_SSL=true

# Authentication
JWT_SECRET=your-jwt-secret-key-min-32-chars
SUPABASE_URL=https://your-project.supabase.co
SUPABASE_KEY=your-anon-key
SUPABASE_SERVICE_ROLE_KEY=your-service-role-key

# Google Drive (OAuth)
GOOGLE_CLIENT_ID=your-client-id
GOOGLE_CLIENT_SECRET=your-client-secret
GOOGLE_REDIRECT_URI=https://nexovas.com/auth/google/callback

# Email
SENDGRID_API_KEY=your-sendgrid-key
SENDER_EMAIL=noreply@nexovas.com

# Payments
RAZORPAY_KEY_ID=your-razorpay-key
RAZORPAY_SECRET=your-razorpay-secret

# AI/ML
TENSORFLOW_LITE_PATH=/models/invoice-ocr.tflite
YOLO_MODEL_PATH=/models/inventory-count.onnx

# Redis
REDIS_URL=redis://user:password@host:port

# Monitoring
SENTRY_DSN=your-sentry-dsn
LOG_LEVEL=info

# Feature Flags
ENABLE_GST_FILING=true
ENABLE_PAYROLL=true
ENABLE_INVENTORY_COUNTING=true
3. DEPLOYMENT ARCHITECTURE
3.1 Development Environment
Frontend: npm run dev (localhost:3000)
Backend: python -m uvicorn main:app --reload (localhost:8000)
Database: Docker PostgreSQL (localhost:5432)
Redis: Docker Redis (localhost:6379)
3.2 Staging Environment
Frontend: Vercel preview deployment
Backend: Railway staging environment
Database: Supabase staging database
CI/CD: GitHub Actions (test → staging → production)
3.3 Production Environment
┌─────────────────────────────────────────┐
│         Vercel CDN / Load Balancer      │
└────────────────┬────────────────────────┘
                 │
     ┌───────────┼───────────┐
     │           │           │
┌────▼────┐ ┌────▼────┐ ┌────▼────┐
│Next.js   │ │FastAPI  │ │Supabase │
│App       │ │Backend  │ │Edge Fn  │
│(Vercel)  │ │Railway  │ │         │
└────┬────┘ └────┬────┘ └────┬────┘
     │           │           │
     └───────────┼───────────┘
                 │
        ┌────────▼────────┐
        │ PostgreSQL DB   │
        │ (Supabase)      │
        └────────┬────────┘
                 │
    ┌────────────┼────────────┐
    │            │            │
┌───▼───┐  ┌─────▼─────┐  ┌──▼──┐
│Redis  │  │Google     │  │S3   │
│Cache  │  │Drive API  │  │Logs │
└───────┘  └───────────┘  └─────┘
4. FOLDER STRUCTURE
4.1 Frontend (Next.js)
frontend/
├── app/
│   ├── layout.tsx (root layout)
│   ├── page.tsx (home page)
│   ├── auth/
│   │   ├── layout.tsx
│   │   ├── login/page.tsx
│   │   ├── signup/page.tsx
│   │   └── reset-password/page.tsx
│   ├── dashboard/
│   │   ├── layout.tsx
│   │   ├── page.tsx (main dashboard)
│   │   ├── invoices/
│   │   │   ├── page.tsx
│   │   │   ├── [id]/page.tsx (invoice detail)
│   │   │   └── create/page.tsx
│   │   ├── ledger/
│   │   │   ├── page.tsx
│   │   │   └── entries/page.tsx
│   │   ├── reports/
│   │   │   ├── page.tsx
│   │   │   ├── p-and-l/page.tsx
│   │   │   ├── balance-sheet/page.tsx
│   │   │   └── gst-summary/page.tsx
│   │   ├── compliance/
│   │   │   ├── page.tsx
│   │   │   ├── gst/page.tsx
│   │   │   ├── tds/page.tsx
│   │   │   └── calendar/page.tsx
│   │   ├── payroll/
│   │   │   ├── page.tsx
│   │   │   ├── salary-slips/page.tsx
│   │   │   └── attendance/page.tsx
│   │   ├── inventory/
│   │   │   ├── page.tsx
│   │   │   └── count/page.tsx
│   │   └── settings/
│   │       ├── page.tsx
│   │       ├── company/page.tsx
│   │       └── users/page.tsx
│   └── api/
│       ├── auth/[...auth].ts
│       ├── invoices/route.ts
│       ├── ledger/route.ts
│       ├── compliance/route.ts
│       └── reports/route.ts
├── components/
│   ├── common/
│   │   ├── Header.tsx
│   │   ├── Sidebar.tsx
│   │   ├── Footer.tsx
│   │   └── Breadcrumb.tsx
│   ├── forms/
│   │   ├── InvoiceForm.tsx
│   │   ├── LoginForm.tsx
│   │   ├── SignupForm.tsx
│   │   └── CompanySetupForm.tsx
│   ├── tables/
│   │   ├── InvoiceTable.tsx
│   │   ├── LedgerTable.tsx
│   │   └── PayrollTable.tsx
│   ├── charts/
│   │   ├── PAndLChart.tsx
│   │   ├── CashFlowChart.tsx
│   │   └── VarianceChart.tsx
│   └── camera/
│       ├── InvoiceScanner.tsx
│       ├── InventoryCounter.tsx
│       └── BarcodeScanner.tsx
├── lib/
│   ├── api.ts (API client)
│   ├── auth.ts (auth utilities)
│   ├── validation.ts (Zod schemas)
│   ├── utils.ts (helper functions)
│   └── constants.ts (app constants)
├── hooks/
│   ├── useAuth.ts
│   ├── useInvoices.ts
│   ├── useReports.ts
│   └── useCamera.ts
├── store/
│   ├── authStore.ts (Zustand)
│   ├── uiStore.ts
│   └── formStore.ts
├── styles/
│   ├── globals.css
│   └── tailwind.config.ts
├── public/
│   ├── images/
│   ├── icons/
│   └── fonts/
├── package.json
├── tsconfig.json
├── tailwind.config.js
└── next.config.js
4.2 Backend (FastAPI)
backend/
├── app/
│   ├── main.py (app entry point)
│   ├── config.py (settings, environment)
│   ├── middleware/
│   │   ├── auth.py (JWT validation)
│   │   ├── error_handler.py
│   │   └── rate_limit.py
│   ├── api/
│   │   ├── v1/
│   │   │   ├── auth/
│   │   │   │   └── routes.py
│   │   │   ├── invoices/
│   │   │   │   ├── routes.py
│   │   │   │   └── schemas.py
│   │   │   ├── ledger/
│   │   │   │   ├── routes.py
│   │   │   │   └── schemas.py
│   │   │   ├── compliance/
│   │   │   │   ├── routes.py
│   │   │   │   ├── gst.py
│   │   │   │   ├── tds.py
│   │   │   │   └── labor.py
│   │   │   ├── payroll/
│   │   │   │   ├── routes.py
│   │   │   │   └── calculator.py
│   │   │   ├── reports/
│   │   │   │   ├── routes.py
│   │   │   │   ├── p_and_l.py
│   │   │   │   ├── balance_sheet.py
│   │   │   │   └── gst_summary.py
│   │   │   ├── inventory/
│   │   │   │   ├── routes.py
│   │   │   │   └── counter.py
│   │   │   └── camera/
│   │   │       ├── routes.py
│   │   │       ├── ocr.py
│   │   │       └── barcode.py
│   │   └── deps.py (dependencies)
│   ├── db/
│   │   ├── models.py (SQLAlchemy models)
│   │   ├── schemas.py (Pydantic schemas)
│   │   ├── session.py (DB connection)
│   │   └── migrations/ (Alembic migrations)
│   ├── core/
│   │   ├── security.py (JWT, password hashing)
│   │   ├── config.py (app config)
│   │   └── constants.py
│   ├── services/
│   │   ├── auth_service.py
│   │   ├── invoice_service.py
│   │   ├── ledger_service.py
│   │   ├── gst_service.py
│   │   ├── payroll_service.py
│   │   ├── report_service.py
│   │   └── autoclaw_service.py
│   ├── agents/
│   │   ├── ca_agent.py (Chartered Accountant)
│   │   ├── cma_agent.py (Cost & Management)
│   │   ├── hr_agent.py (Human Resources)
│   │   ├── crm_agent.py (Customer Relations)
│   │   ├── pm_agent.py (Project Management)
│   │   └── cs_agent.py (Customer Service)
│   ├── ml/
│   │   ├── ocr.py (TensorFlow Lite OCR)
│   │   ├── inventory.py (YOLO inventory counting)
│   │   ├── fraud_detection.py (anomaly scoring)
│   │   └── models/ (pre-trained models)
│   ├── integrations/
│   │   ├── google_drive.py
│   │   ├── razorpay.py
│   │   ├── sendgrid.py
│   │   ├── gst_portal.py
│   │   ├── mca_efiling.py
│   │   └── tds_portal.py
│   ├── tasks/
│   │   ├── celery_app.py (Celery setup)
│   │   ├── invoice_tasks.py
│   │   ├── compliance_tasks.py
│   │   ├── payroll_tasks.py
│   │   └── scheduled_tasks.py (cron jobs)
│   ├── utils/
│   │   ├── validators.py
│   │   ├── formatters.py
│   │   ├── calculations.py
│   │   └── helpers.py
│   └── logging/
│       ├── logger.py
│       └── audit.py (audit trail)
├── tests/
│   ├── test_auth.py
│   ├── test_invoices.py
│   ├── test_ledger.py
│   ├── test_compliance.py
│   ├── test_payroll.py
│   └── test_agents.py
├── requirements.txt
├── Dockerfile
├── docker-compose.yml
├── .env.example
└── README.md
5. DATABASE SCHEMA HIGHLIGHTS
5.1 Core Tables
users

CREATE TABLE users (
  id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
  email VARCHAR(255) UNIQUE NOT NULL,
  full_name VARCHAR(255),
  password_hash VARCHAR(255),
  phone VARCHAR(20),
  company_id UUID REFERENCES companies(id),
  role VARCHAR(50) DEFAULT 'user',
  permissions JSONB,
  is_active BOOLEAN DEFAULT TRUE,
  created_at TIMESTAMP DEFAULT NOW(),
  modified_at TIMESTAMP DEFAULT NOW()
);
companies

CREATE TABLE companies (
  id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
  name VARCHAR(255) NOT NULL,
  gst_no VARCHAR(15),
  pan_no VARCHAR(10),
  industry VARCHAR(100),
  fiscal_year_start INT DEFAULT 4,
  created_at TIMESTAMP DEFAULT NOW(),
  modified_at TIMESTAMP DEFAULT NOW()
);
invoices

CREATE TABLE invoices (
  id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
  company_id UUID REFERENCES companies(id),
  invoice_no VARCHAR(50) UNIQUE,
  invoice_date DATE,
  vendor_id UUID REFERENCES vendors(id),
  customer_id UUID REFERENCES customers(id),
  amount DECIMAL(12,2),
  gst_amount DECIMAL(12,2),
  hsn_code VARCHAR(8),
  gst_rate DECIMAL(5,2),
  invoice_type VARCHAR(50), -- 'purchase', 'sales'
  status VARCHAR(50) DEFAULT 'draft', -- 'draft', 'posted', 'cancelled'
  evidence_file_id VARCHAR(255), -- Google Drive file ID
  posted_date TIMESTAMP,
  posted_by UUID REFERENCES users(id),
  autoclaw_status VARCHAR(50) DEFAULT 'pending',
  autoclaw_confidence DECIMAL(3,2),
  fraud_probability DECIMAL(10,9),
  created_at TIMESTAMP DEFAULT NOW(),
  modified_at TIMESTAMP DEFAULT NOW()
);

CREATE INDEX idx_invoices_company_date ON invoices(company_id, invoice_date);
CREATE INDEX idx_invoices_status ON invoices(status);
CREATE INDEX idx_invoices_hsn ON invoices(hsn_code);
gl_entries (General Ledger)

CREATE TABLE gl_entries (
  id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
  company_id UUID REFERENCES companies(id),
  account_id UUID REFERENCES accounts(id),
  invoice_id UUID REFERENCES invoices(id),
  debit DECIMAL(12,2) DEFAULT 0,
  credit DECIMAL(12,2) DEFAULT 0,
  narration TEXT,
  entry_type VARCHAR(50), -- 'journal', 'invoice', 'payment', 'payroll'
  posting_date DATE,
  blockchain_hash VARCHAR(255), -- SHA-256 hash
  status VARCHAR(50) DEFAULT 'posted',
  created_at TIMESTAMP DEFAULT NOW(),
  modified_at TIMESTAMP DEFAULT NOW()
);

CREATE INDEX idx_gl_company_date ON gl_entries(company_id, posting_date);
CREATE INDEX idx_gl_account ON gl_entries(account_id);
CREATE INDEX idx_gl_hash ON gl_entries(blockchain_hash);

-- Immutability: No UPDATE or DELETE allowed (only INSERT)
CREATE RULE gl_entries_no_update AS ON UPDATE TO gl_entries
  DO INSTEAD NOTHING;
CREATE RULE gl_entries_no_delete AS ON DELETE TO gl_entries
  DO INSTEAD NOTHING;
salary_slips

CREATE TABLE salary_slips (
  id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
  company_id UUID REFERENCES companies(id),
  employee_id UUID REFERENCES employees(id),
  salary_month DATE,
  gross_salary DECIMAL(12,2),
  pf_amount DECIMAL(12,2),
  esi_amount DECIMAL(12,2),
  pt_amount DECIMAL(12,2),
  tds_amount DECIMAL(12,2),
  net_salary DECIMAL(12,2),
  status VARCHAR(50) DEFAULT 'draft',
  posted_date TIMESTAMP,
  posted_by UUID REFERENCES users(id),
  created_at TIMESTAMP DEFAULT NOW(),
  modified_at TIMESTAMP DEFAULT NOW()
);
row_level_security_policies

-- Users can only see invoices from their company
CREATE POLICY users_see_own_company_invoices
  ON invoices FOR SELECT
  USING (company_id IN (
    SELECT company_id FROM users WHERE id = auth.uid()
  ));

-- Users can only create invoices for their company
CREATE POLICY users_create_own_company_invoices
  ON invoices FOR INSERT
  WITH CHECK (company_id IN (
    SELECT company_id FROM users WHERE id = auth.uid()
  ));
6. INTEGRATION REQUIREMENTS
6.1 Google Drive API
Scope: https://www.googleapis.com/auth/drive.file (app-created files only)
Endpoints:
files.create() (upload invoice image)
files.list() (list files by company)
files.download() (download evidence)
Error Handling: Retry on quota_exceeded, rateLimitExceeded
6.2 Razorpay API
Endpoints:
payments.create() (charge customer)
subscriptions.create() (recurring billing)
transfers.create() (settle to merchant account)
Webhooks: payment.authorized, payment.failed, subscription.charged
6.3 SendGrid API
Email Templates:
Invoice delivery (customer)
GST filing deadline (business owner)
TDS payment due (business owner)
Monthly P&L summary (business owner)
Support ticket response (customer)
Retry Logic: Exponential backoff on 429, 500, 502 errors
7. PERFORMANCE & SCALABILITY
7.1 Caching Strategy
Redis: Cache frequently queried data (accounts, customers, vendors)
TTL: 1 hour for reports, 24 hours for masters
Invalidation: On-update (cache bust)
Memory: 2GB Redis instance (supports 1M+ cache entries)
7.2 Database Optimization
Query Optimization:
Indexes on (company_id, date) for most queries
Partitioning by month for large tables (invoices, GL entries)
EXPLAIN ANALYZE for slow queries
Connection Pooling:
PgBouncer for connection pooling
50 connections per microservice
7.3 API Rate Limiting
Per User: 100 requests/minute
Per IP: 1000 requests/minute
Per Endpoint: 500 requests/minute (GST validation, reports)
Response: 429 Too Many Requests with Retry-After header
7.4 Backend Scaling
Auto-scaling: Railway auto-scales based on CPU/memory (2–10 instances)
Load Balancing: Nginx round-robin
Max Concurrent Users: 10,000+ with current infrastructure
8. SECURITY SPECIFICATIONS
8.1 Authentication
JWT Tokens: Signed with HS256, expiry 1 hour
Refresh Tokens: 30-day expiry, stored in HTTP-only cookies
Password Hashing: bcrypt with salt rounds 12
2FA: Optional (TOTP via authenticator app)
8.2 Data Encryption
In Transit: TLS 1.3 (HTTPS only)
At Rest: PostgreSQL native encryption (PgCrypto)
Sensitive Fields: payment_method, pan_no, aadhaar_no (if collected)
8.3 Access Control
Row-Level Security: PostgreSQL RLS policies (per-company isolation)
Role-Based: user, admin, ca roles
Permissions: Granular (create_invoice, approve_invoice, etc.)
8.4 API Security
CORS: Whitelisted domains only
CSRF Protection: Double-submit cookies
Input Validation: Pydantic models (strict type checking)
SQL Injection Prevention: Parameterized queries (SQLAlchemy ORM)
XSS Prevention: Content Security Policy (CSP) headers
8.5 Audit Trail
Logging: All transactions logged (user_id, timestamp, action, result)
Immutable Ledger: GL entries cannot be edited/deleted (PostgreSQL rules)
Blockchain Anchoring: Hash of each GL entry stored (optional: Ethereum mainnet)
9. COMPLIANCE & TESTING
9.1 Compliance
GST: HSN code validation, ITC eligibility rules
TDS: Section thresholds (194C: >₹30K, 194J: >₹30K, etc.)
Labor: PF cap (₹15K/month), ESI eligibility
Data Privacy: GDPR-compliant (users own data in Drive)
9.2 Testing
Unit Tests: 80%+ coverage (pytest)
Integration Tests: API → DB → Google Drive
End-to-End Tests: Selenium (invoice creation → posting → report generation)
Performance Tests: k6 (load testing, 10K concurrent users)
Security Tests: OWASP Top 10 validation, penetration testing
FINAL NOTES
MVP Timeline (20 weeks):

Weeks 1–4: Setup, database schema, authentication
Weeks 5–8: Core APIs (invoices, ledger, compliance)
Weeks 9–12: Autoclaw Prime agents, VisionCount integration
Weeks 13–16: UI/UX, mobile app, reporting
Weeks 17–20: Testing, deployment, documentation
Infrastructure Cost (Monthly):

Vercel: ₹2,500 (frontend)
Railway: ₹5,000 (backend)
Supabase: ₹10,000 (database, 2GB RAM)
Redis: ₹2,000 (caching)
SendGrid: ₹1,000 (email)
Razorpay: 2% + ₹3/transaction (payments)
Total: ₹20,500 + transaction fees
Profitability at 10,000 Users:

Revenue: ₹50L/month (avg ₹999/user)
Infrastructure: ₹50K/month
Gross Margin: 99%

---

# CONTINUING WITH REMAINING 8 DOCUMENTS...

[Due to character limit, I'll provide the core structure and key highlights for remaining documents. Each would be similarly detailed]

---

# DOCUMENT 03: APP-FLOW.md — Navigation & User Journey Map

```markdown
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
DOCUMENT 04: UI-UX-BRIEF.md — Design System & Visual Language
# NEXOVAS ERP — UI/UX Design Brief
## Visual Language, Components & Interaction Design
### Version: FINAL v3.0

---

## 1. DESIGN PHILOSOPHY

**Core Principles:**
1. **Speed Over Perfection** — Kirana owner can scan invoice in <5 seconds
2. **Clarity Over Complexity** — Non-technical user understands GST/TDS instantly
3. **Trust Through Transparency** — All calculations visible + explainable
4. **Mobile-First** — Desktop is secondary (90% users on phones)
5. **Accessibility** — WCAG 2.1 AA compliance (colorblind-friendly, large text)

**Aesthetic Direction:**
- Minimal, clean, dark-mode first (reduces battery drain on phone)
- Like Linear (SaaS management tool) + Vercel (developer experience)
- Financial/professional (not playful)
- Modern without being trendy (timeless design)

---

## 2. COLOR SYSTEM

### Primary Palette
- **Primary (Indigo):** #6C47FF (CTAs, highlights, active states)
- **Secondary (Green):** #10B981 (Success, positive variance)
- **Warning (Orange):** #F59E0B (Caution, pending approval)
- **Danger (Red):** #EF4444 (Error, fraud alert)
- **Neutral (Gray):** #6B7280 (Secondary text, disabled states)

### Background
- **Dark Mode (Primary):** #0F172A (near-black, reduces eye strain)
- **Surface:** #1E293B (card backgrounds)
- **Surface Alt:** #334155 (hover states)
- **Light Mode (Optional):** #FFFFFF with #F8FAFC surface

### Semantic Colors
- **GST Filing Due:** #FCA5A5 (light red)
- **GST Filed:** #86EFAC (light green)
- **TDS Pending:** #FED7AA (light orange)
- **Fraud Alert:** #DC2626 (bright red)
- **Blockchain Verified:** #8B5CF6 (purple, trustworthy)

---

## 3. TYPOGRAPHY

### Font Family
- **UI/Headers:** "Inter" (modern, clean, excellent readability)
- **Code/Data:** "Geist Mono" (monospace, for numbers + GL entries)
- **Fallback:** -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto

### Scale
Display: 48px / 57.6px line-height (hero headline) Heading 1: 36px / 43.2px (page title) Heading 2: 28px / 33.6px (section title) Heading 3: 24px / 28.8px (subsection) Body Large: 16px / 24px (primary text) Body: 14px / 21px (secondary text) Small: 12px / 18px (captions, labels) Tiny: 11px / 16.5px (timestamps, hints)


### Font Weights
- **Regular (400):** Body text, labels
- **Medium (500):** Emphasis, secondary headings
- **Semibold (600):** Primary headings, CTAs
- **Bold (700):** Display text, highlights

---

## 4. COMPONENT LIBRARY (Shadcn/ui)

### Form Components
**Input Field:**
- Dark background (#1E293B), light text
- Focus: Indigo border + glow effect
- Placeholder: Gray text (40% opacity)
- Validation: Red border + error message below

**Select Dropdown:**
- Search-enabled (filter 100+ vendors in <200ms)
- Scroll: Virtual scrolling (performance)
- Multi-select option (for batch invoices)

**Checkbox / Radio:**
- Size: 20px × 20px (touch-friendly)
- Label: 14px, gray text
- Checked state: Indigo background + checkmark

**Date Picker:**
- Calendar popup
- Default: Today's date
- Disabled: Dates before fiscal year start

### Data Display

**Table:**
- Striped rows (every other row: #1E293B vs #0F172A)
- Sortable columns (click header to sort)
- Filterable (column filter icon)
- Paginated (50 rows/page, pagination controls at bottom)
- Row actions: Edit, Delete, Post buttons on hover

**Card:**
- Shadow: Subtle (0 1px 3px 0 rgba(0,0,0,0.1))
- Border: None (shadow only)
- Padding: 16px
- Rounded: 8px

**Alert / Toast:**
- Success: Green icon + "Invoice posted successfully"
- Error: Red icon + "GST rate mismatch. Please confirm."
- Info: Blue icon + "Compliance filing due in 3 days"
- Warning: Orange icon + "Invoice pending CA approval"
- Auto-dismiss: 5 seconds (or manual close)

### Modal / Dialog
- Overlay: Dark with 50% opacity
- Width: 90% (mobile), 600px (desktop)
- Close: X button (top-right)
- Action buttons: "Cancel" (gray) + "Confirm" (indigo)

### Navigation
- **Top Bar:** Logo + company name + user menu
- **Sidebar:** Dark (#0F172A), icons + labels
- **Active State:** Indigo background on current page
- **Hover State:** #1E293B background

---

## 5. LAYOUT PATTERNS

### Dashboard (God View)
┌─────────────────────────────────────────┐ │ NEXOVAS [Company Name] [Menu] │ ├─────────────────────────────────────────┤ │ Side │ Dashboard │ │ bar │ │ │ │ ┌─────────────────┐ ┌────────┐ │ │ │ │ Today's P&L │ │ Cash │ │ │ │ │ Revenue: ₹50K │ │ Flow │ │ │ │ │ Expense: ₹20K │ │ 
You can't use 'macro parameter character #' in math mode
$###   │ │
│      │  │ Profit: ₹30K    │  └────────┘ │
│      │  └─────────────────┘              │
│      │                                   │
│      │  ┌─────────────────┐  ┌────────┐ │
│      │  │ GST Filing Due  │  │ TDS    │ │
│      │  │ in 3 days       │  │ Due    │ │
│      │  │ [Prepare Now]   │  │ $### │ │ │ │ └─────────────────┘ └────────┘ │ │ │ │ │ │ ┌─────────────────────────────┐ │ │ │ │ Recent Invoices (Last 5) │ │ │ │ │ [Table with 5 rows] │ │ │ │ └─────────────────────────────┘ │ │ │ │ └─────────────────────────────────────────┘


### Invoice Create/Edit
┌─────────────────────────────────────────┐ │ Create Invoice │ ├─────────────────────────────────────────┤ │ Invoice Type: [Purchase / Sales] │ │ Vendor/Customer: [Search dropdown] │ │ Invoice Date: [Date picker] │ │ Invoice Number: [Text input] │ │ │ │ Line Items: │ │ ┌─────────────────────────────────────┐ │ │ │ Item │ Qty │ Rate │ HSN │ GST │ Amt │ │ │ ├─────────────────────────────────────┤ │ │ │ .... │ ... │ ... │ ... │ ... │ ... │ │ │ │ [+] Add Item │ │ │ └─────────────────────────────────────┘ │ │ │ │ Total: ₹10,000 | GST: ₹1,800 | ... │ │ │ │ [Cancel] [Save as Draft] [Post] │ └─────────────────────────────────────────┘


### Reports / P&L
┌─────────────────────────────────────────┐ │ Profit & Loss (October 2026) │ ├─────────────────────────────────────────┤ │ Month: [October] Year: [2026] [Export] │ │ │ │ ┌─────────────────────────────────────┐ │ │ │ Revenue ₹1,00,000 │ │ │ │ Sales ₹1,00,000 │ │ │ │ COGS (₹40,000) │ │ │ │ Gross Profit ₹60,000 60% │ │ │ │ Expenses (₹20,000) │ │ │ │ Salary (₹15,000) │ │ │ │ Rent (₹5,000) │ │ │ │ Net Profit ₹40,000 40% │ │ │ └─────────────────────────────────────┘ │ │ │ │ [Chart: P&L Trend] │ │ ┌─────────────────────────────────────┐ │ │ │ $ │ │ │ │ • │ │ │ │ • • • │ │ │ │ • • • • │ │ │ │ Oct Nov Dec Jan │ │ │ └─────────────────────────────────────┘ │ └─────────────────────────────────────────┘


---

## 6. MOBILE-FIRST DESIGN

### Responsive Breakpoints
- **Mobile (< 640px):** Single column, full-width components
- **Tablet (640–1024px):** 2-column layout
- **Desktop (> 1024px):** 3-column + sidebar

### Mobile-Specific Features
- **Bottom Tab Navigation:** Home, Scan, Invoices, Reports, Menu
- **Floating Action Button (FAB):** "+" button (bottom-right) → New Invoice /

## @rupankard018-svg

build remaining all .md files in this chat
