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
