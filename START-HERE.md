# Franklin Street Decks — Capital Markets

Investment sales and debt & equity decks, built on the same design system as the
Leasing decks (`../Leasing/`).

## What's in this folder

| Folder | What it is |
|---|---|
| `00_Guide/` | Build guide, **Capital Markets intake questions**, Claude prompts, section reference, QC, publishing, asset specs |
| `01_Templates/Capital-Markets/` | The Capital Markets template (v0.1 draft, built from Leasing v2.2). See its `TEMPLATE-INFO.md` |
| `02_Brand-Library/` | Logo, fonts, colors, client-logo panel, awards & stats list |
| `03_Team-Library/` | Atlanta Retail Investment Sales headshots and `team-roster.md` (titles, contacts, full bios) |
| `04_Decks/` | One folder per deck. `_DECK-TEMPLATE` is the blank copied for each new one |
| `05_Archive/` | Finished decks and template snapshots |
| `tools/` | Start a deck, preview, QC check, convert a design export |

## Decks

| Deck | Status | Preview |
|---|---|---|
| `04_Decks/2026-10_atl-retail-investment-sales/` | Build — draft with highlighted placeholders (`00_Intake/PLACEHOLDERS.md`) | Live: https://fsmarketing123.github.io/Capital_Markets_Deck_2026/ · local: http://localhost:8082 |

## Commands

```bash
cd ~/Desktop/Decks/"Capital Markets"
```

| Do this | Command |
|---|---|
| Start a new deck | `bash tools/new-deck.sh "Deck Name"` |
| Preview a deck | `bash tools/preview.sh 04_Decks/[deck-folder]/05_Site 8082` → http://localhost:8082 |
| QC a deck | `python3 tools/check-deck.py 04_Decks/[deck-folder]/05_Site` |

## Placeholders

Anything still to add is wrapped in `<span class="todo">…</span>` and shows on the page as a yellow,
dashed label, with a "Draft · N placeholders" badge in the corner. The QC check lists every one and
the badge disappears when none are left.
