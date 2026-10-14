# Franklin Street — Capital Markets Deck System (2026)

Scroll-and-clicker landing-page decks for Franklin Street investment sales, built on the same design
system as the Leasing decks.

**Start here:** [START-HERE.md](START-HERE.md)

| Folder | What it is |
|---|---|
| `00_Guide/` | Build guide, Capital Markets intake questions, Claude prompts, section reference, QC, publishing, asset specs |
| `01_Templates/Capital-Markets/` | Capital Markets template (v0.1 draft, built from Leasing v2.2) |
| `02_Brand-Library/` | Logo, fonts, colors, client-logo panel, awards & stats |
| `03_Team-Library/` | Atlanta Retail Investment Sales headshots, roster and bios |
| `04_Decks/` | One folder per deck; `2026-10_atl-retail-investment-sales/05_Site` is the Atlanta deck (draft) |
| `05_Archive/` | Template snapshots |
| `tools/` | `new-deck.sh`, `preview.sh`, `check-deck.py`, `unbundle.py` |

## Atlanta deck status

Draft with highlighted placeholders — see
[`04_Decks/2026-10_atl-retail-investment-sales/00_Intake/PLACEHOLDERS.md`](04_Decks/2026-10_atl-retail-investment-sales/00_Intake/PLACEHOLDERS.md).

## Preview locally

```bash
bash tools/preview.sh 04_Decks/2026-10_atl-retail-investment-sales/05_Site 8082
```

Then open http://localhost:8082.
