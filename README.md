# Centralized Technical Debt Prioritization Process

A self-contained HTML dashboard for collecting, scoring, and prioritizing technical debt work items across four SBUs (MSS, SCIM, A&I, TPC) aligned to FY27 goals.

## Workflow Steps

### Step 1 — Roll-up
Collect ADO feature requests from all four SBUs into a single intake bucket. Each item captures:
- Source SBU, ADO ID, Title
- Requestor and business justification

### Step 2 — Triage & Prioritize
Score each item 1–5 against five weighted FY27 criteria:

| Criteria | Weight | Description |
|----------|--------|-------------|
| USD Impact | 4 | Estimated dollar savings / cost avoidance |
| Scale / Reach | 3 | Volume of cases, agents, SBUs impacted |
| Strategic Alignment | 4 | Alignment with FY27 exec priorities |
| CSAT Impact | 5 | Customer satisfaction score improvement |
| TPUT Impact | 5 | Throughput / time to resolution improvement |

### Step 3 — Prioritized Output
- Items ranked by **Adjusted Score** (base score ÷ effort days)
- Priority auto-assigned: Critical, High, Medium, Low
- Customizable capacity validation (total days + per-feature effort)
- Medium/Low items auto-tagged as **Deferred**
- CSV export available

### Step 4 — Business & Engineering Alignment
- Only Critical and High priority items surface for review
- Approve or Defer each item
- Reviewer notes field for CSS LT

### Step 5 — Final / Create
- Auto-creates SXG ADO work items for approved items
- Deferred items listed for next sprint planning
- CSV exports for both created and deferred items

## Usage
1. Open `index.html` in any modern browser
2. Click **Load Sample Data** to see 12 pre-built items, or add your own
3. Walk through Steps 1–5 using the pipeline nav at the top

## Sharing
- **GitHub Pages**: Upload `index.html` to a public repo and enable Pages
- **SharePoint**: Upload the file to a document library and share the link
- **Email / Teams**: Attach the HTML file directly — recipients open in browser

## Tech Stack
- Single-file HTML/CSS/JS — no dependencies, no build step
- Works offline once loaded
