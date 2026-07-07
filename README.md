# 🏡 Dream House Construction Planner

A single-file, fully offline dashboard for planning and tracking a house build from land purchase through handover — checklists, budget, loan EMI, phase tracker, materials, and reports, all in one `index.html`.

**Powered by Sethu.**

---

## What it is

- One file: `index.html`. No build step, no server, no accounts.
- Pure HTML + CSS + vanilla JavaScript — no external frameworks or CDN dependencies.
- All data is stored in your browser's **LocalStorage**. Nothing is ever sent to a server.
- Works fully offline — open the file directly in any modern browser.

## How to use it

1. Download `index.html`.
2. Open it in Chrome, Edge, Firefox, or Safari (double-click, or drag into a browser tab).
3. Start filling in checklists — everything saves automatically as you type.
4. Bookmark the file or keep it on your desktop; reopening it reloads your saved data from that browser's LocalStorage.

> ⚠️ LocalStorage is tied to the browser + file location you open it from. If you move the file, or open it in a different browser/profile, your data won't follow automatically — use **Export JSON** (Settings or Reports page) to back up, and **Import JSON** to restore or transfer.

## Pages

| Sheet | Page | What it covers |
|---|---|---|
| — | Dashboard | Overall progress ring, budget snapshot, task counts, Risk Analyzer, Reminders |
| A-01 | Land Purchase | Site checklist + flood/water/garbage yes-no risk questions, road & frontage width |
| A-02 | Documentation | DTCP/CMDA, Patta, EC, legal & engineer opinion, etc. + file attachments |
| A-03 | Engineering | Site engineering checks, Engineer Selection, Soil Test details |
| A-04 | Architecture | House design fields (rooms, floors, etc.), design lock warning |
| B-01 | Budget Planner | Full cost breakdown, contingency %, budget health |
| B-02 | Loan Planner | EMI, total interest, total payment calculator |
| C-01 | Construction | 20-phase timeline with status, dates, notes, and photo upload |
| C-02 | Materials | Editable price/supplier table + Excluded Items checklist |
| C-03 | Agreement | Contract terms checklist + attachments |
| C-04 | Quality Inspection | Stage-by-stage inspection checklist |
| M-01 | Rainwater Harvesting | RWH planning checklist |
| M-02 | Water | Borewell & water supply checklist |
| M-03 | Electrical | Wiring & inspection checklist |
| M-04 | Plumbing | Pipe fitting & leak test checklist |
| M-05 | Painting | Surface prep through finish |
| M-06 | Interior | Fit-out & furnishing checklist |
| F-01 | Completion | Handover checklist |
| R-01 | Reports | Generate text reports, export JSON/CSV, print |
| S-01 | Settings | Theme, project timeline, global notes, data reset, disclaimer |

## Features

- **Blueprint theme** — dark mode = cyanotype (white lines on blueprint blue), light mode = diazo print (blue lines on cream paper). Toggle from the top bar or Settings.
- **Global search** — search every checklist item at once from the top bar; results jump straight to and highlight the matching row.
- **Risk Analyzer** — automatically flags: narrow road/frontage width, flood-prone or ex-garbage-dump land, missing soil test, no registered engineer, missing legal opinion, missing DTCP/CMDA approval, no rainwater harvesting plan, and thin budget contingency.
- **Reminders panel** — surfaces pending documents, loan planning, engineer visits, approvals, unordered materials, payment schedule, and inspections.
- **Budget Planner** — itemized cost inputs, 10/15/20% contingency presets, computed grand total and budget health indicator.
- **Loan Planner** — standard reducing-balance EMI formula (monthly EMI, total interest, total payment).
- **Construction Phase Tracker** — 20 standard phases (Land Purchase → Handover), each with status, date, notes, and a photo (auto-resized before saving to keep storage small).
- **Materials table** — add/remove rows, per-row include toggle, auto-computed line and grand totals, CSV export.
- **Reports** — one-click text reports: Construction Summary, Budget Summary, Checklist Summary, Pending Items, Risk Report, Engineer Report, Loan Report.
- **Export / Import JSON** — full backup and restore of all your data.
- **Print / Save as PDF** — uses your browser's print dialog; sidebar and controls are hidden in print view.
- **File attachments** — small images/PDFs (under ~700KB) can be attached to Documentation and Agreement pages.

## Data & privacy

- Everything lives in `localStorage` under the key `dreamHouseState_v1` in the browser you're using.
- No network calls, no analytics, no third-party services.
- Use **Export JSON** regularly as a backup — clearing browser data/history can erase LocalStorage.
- **Reset All Data** (Settings page) permanently wipes everything in that browser — it cannot be undone.

## Disclaimer

This app is a **personal planning and organization tool**. It does **not** provide legal, structural, financial, or engineering advice. Budget, EMI, and risk figures are estimates based only on the numbers you enter — they may not reflect actual costs, bank terms, or real site conditions.

Always verify:
- Land and ownership documents with a **licensed advocate**
- Foundation, soil, and structural decisions with a **registered civil engineer**
- Loan terms directly with your **bank**

The creator of this app is not liable for any financial, legal, or construction outcome arising from its use.

---

*Dream House Construction Planner v1.0 — single HTML file, offline-first. Powered by Sethu.*
