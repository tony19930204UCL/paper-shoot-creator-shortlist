# Paper Shoot Creator Shortlist — design brief

## Product goal
Build a private, responsive research dashboard for reviewing Instagram creators for Paper Shoot partnerships in the US and Canada. It should help a marketer compare leads, assess evidence quality, and decide who to verify next. It is not an influencer marketplace or outreach automation tool.

## Primary user task
Filter the discovered creator leads, open a candidate, verify the source and recent Instagram activity, then add or reject the creator for a campaign shortlist.

## Information architecture
1. **Shortlist workspace** — campaign title, retrieval date, counts by verification state, search, filters, sortable list/grid, export.
2. **Creator card/row** — handle, location, niche tags, follower count, engagement rate, source/date labels, activity status, fit rationale, verification status, actions.
3. **Creator detail drawer** — profile link, source-backed bio/location, recent post evidence with dates and visible engagement, measured-vs-reported ER, brand-fit notes, public contact and evidence source, UGC/collaboration signal, suggested activation, flags and reviewer notes.
4. **Compare view** — compare up to four selected creators across location, audience-location evidence, followers, ER method, activity, visual fit, contact, and unresolved checks.
5. **Pipeline statuses** — Lead → Needs verification → Shortlisted → Contacted → Negotiating → Confirmed; also Rejected. Allow notes and tags; do not send outreach from the first version.

## Filters
- Creator location: United States / Canada / unknown.
- Audience location: US / Canada / unknown; never infer it from creator location.
- Follower count: preferred 10k–80k; expandable 5k–150k.
- Niche: film/analog/digicam, everyday lifestyle/photo dump, travel/event/wedding, mindful/digital detox, sustainable.
- Engagement: verified measured ER vs provider-reported ER; allow minimum threshold but show the method.
- Activity: last post date and posting cadence, with unknown kept separate.
- Verification state, brand-fit confidence, and flags.

## Data integrity rules
- Make current/platform-measured values visually distinct from directory estimates.
- Every important metric shows its source and observed date; unknown or stale data never look verified.
- ER must show its calculation method/sample when independently measured.
- Do not show a single dominant fit score while activity, metrics, or visual review are unknown. Prefer “Potential fit” plus “Evidence completeness.” If scoring is later enabled, show a dimension breakdown and mark provisional scores.
- Use only public contact details and record where they came from.
- No scraping, login bypass, private Instagram data, or invented recent-post summaries.

## Visual direction
Warm paper-white canvas, charcoal text, muted cobalt/sepia accents, restrained borders, generous spacing, and editorial creator photography. The interface should feel like a thoughtful photography brand but remain a practical B2B review tool. Use readable status chips and clear labels, not film-themed decoration that obscures evidence.

## First viewport priorities
- Header: “Creator shortlist / North America” + retrieval date + export.
- Four count cards: Total leads, Verified, Needs review, Shortlisted.
- Filter bar with country, follower range, niche, ER type, activity and verification state.
- Main area toggle: Evidence table (default) / Photo grid.
- Candidate entries sorted by fit evidence or verification readiness, never ER alone.
- Persistent notice that directory-reported metrics are not live Instagram verification.

## First version scope
- Static, client-side prototype using local sample/mock data only until the owner explicitly approves adding prospect records to this repository.
- Responsive desktop and mobile layouts.
- Search, filters, sort, compare selection, detail drawer, notes/status interactions, and CSV export.
- No account login, email sending, payments, analytics tracking, or publishing of creator personal data.

## Acceptance checks
- At a glance, users can distinguish verified vs provisional candidates and see unknown data.
- Filters work together and can be reset.
- Creator location and audience location are distinct fields.
- Detail view shows source attribution and verification date beside each metric.
- Layout is usable at desktop and mobile widths, keyboard accessible, and has adequate text contrast.
- Sample data is clearly labeled as demo data until approved real data is added.
