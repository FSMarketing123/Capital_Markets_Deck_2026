# Franklin Street Capital Markets Decks — instructions for Claude

Capital markets (investment sales, debt & equity) decks: single-page, scroll-and-clicker websites on the
Leasing design system, published on Netlify. The Leasing side lives in `../Leasing/`; don't edit it from here.

## Layout
- `01_Templates/Capital-Markets/` — template (v0.1 draft). Only edit when the user says the change is for all
  future Capital Markets decks; log it in `CHANGELOG.md`.
- `04_Decks/<YYYY-MM_slug>/` — one deck. Edit only its `05_Site/`. Sources: `00_Intake/` (intake.md, `source/` PDFs,
  `PLACEHOLDERS.md`), `03_Data/` (financials, sales-comps), `03_Team-Library/team-roster.md`, `02_Brand-Library/awards/awards-list.md`.
- Capital Markets additions live in each site's `css/capital-markets.css` (placeholders, round headshots, text marquees,
  client logo panel, transactions grid).
- `00_Guide/04_Section-Reference.md` describes the shared section structure (written for Leasing; names differ).

## Rules
- Never invent numbers, cap rates, buyers, awards or contacts. Put unknowns in `<span class="todo">What to add</span>`
  and list them in the deck's `00_Intake/PLACEHOLDERS.md`.
- Data from source PDFs: copy exactly; flag inconsistencies in PLACEHOLDERS.md instead of guessing.
- Run `python3 tools/check-deck.py <site>` after every edit. `todo` placeholders show as errors until filled.
- Same structural rules as Leasing: tabs/panels numbered from 0, carousel `data-i` + one dot per card,
  marquee items listed twice, `tl-count` matches items, new sections go in `var CH` in `js/motion.js`.
- Preview: `python3 -m http.server 8082 --directory <site>` in the background, then http://localhost:8082.
- Don't publish without the user's go-ahead.
