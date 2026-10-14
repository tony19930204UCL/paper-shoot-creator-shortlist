# First build task for ChatGPT Codex

Build a responsive, single-page prototype for the Paper Shoot creator shortlist. Read `DESIGN_BRIEF.md` first and follow it.

## Scope
- Implement a polished desktop and mobile shortlist dashboard with a warm paper-white / charcoal / muted cobalt and sepia visual language.
- Use clearly labeled mock creator records only. Do not copy the real prospect CSV, public contact emails, or any other creator personal data into this repository until the owner explicitly approves.
- Include KPI cards, search, filters, sort, evidence table/photo-grid toggle, multi-select compare, creator detail drawer, status changes, reviewer notes, and CSV export of mock records.
- Label demo records and metrics as fictional/demo data. Never imply they are verified.
- Treat the verification status, source, and observed date as first-class fields. Unknown recent-post activity and audience geography must remain visibly unknown.
- Use native browser APIs and plain HTML/CSS/JavaScript unless a dependency is clearly justified. Do not add an account/login flow, third-party analytics, scraping, or network calls.
- Keep the app usable with keyboard navigation, visible focus states, responsive layouts, and readable contrast.

## Deliverables
- A runnable static prototype from `index.html` (or an equivalently simple structure).
- Short local run instructions in `README.md`.
- A small local demo fixture with at least 8 distinct example rows spanning film, everyday lifestyle, travel and outdoor niches.
- A short test/verification note describing browser sizes, tested interactions, and any remaining limitations.

## Acceptance checklist
1. Search and every filter work together and can be reset.
2. Sorting supports follower count, ER value and evidence completeness without presenting directory ER as verified ER.
3. Each creator row opens a detail panel with metric provenance, activity status, fit rationale, contact state and next verification steps.
4. Compare mode supports up to four records and distinguishes creator location from audience location.
5. Status and notes work during the session; export returns valid CSV with clear demo labeling.
6. Desktop and mobile layouts are readable, keyboard-operable and have visible focus indication.
7. No real candidate/contact data, credentials, API keys, or remote scraping code are included.
