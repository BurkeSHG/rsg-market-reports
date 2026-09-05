# RS Gonzales city market reports

Everything needed to build a city HVAC market report page, one folder per market.

The Waco page is the template. Every other market is that same page with different numbers.
Nothing new gets designed.

**Live template:** https://waco-market-report.vercel.app/market-report/waco-tx/

## Start here

| File | What it is |
|---|---|
| `template/waco-reference.html` | The live Waco page, saved in full. Open it locally to see exactly what you are matching. |
| `template/waco-fullpage.png` | Full-page screenshot of the same page. |
| `template/VISUAL-INVENTORY.md` | Section-by-section layout teardown: the grid, the light and dark alternation, the background photographs, the image inventory, and the 28 things that change per market. |
| `template/DATA-CONTRACT.md` | Every field the page consumes, where each one comes from, and the static blocks that never change. |
| `FORMULA.md` | The whole report on one page: six inputs, the arithmetic, the constants. |

## Building a market

Each market gets a folder under `markets/` containing three spreadsheets.

**`handoff.csv`** is the build sheet. About 125 rows, in the page's own section order, so you can read
down it as you work. Columns: Section, Field, Value, Unit, Source, Status, Note.

The Status column is the important one:

| Status | Meaning |
|---|---|
| `FILLED` | Final. Use it. |
| `CONSTANT` | Identical in every market. Copy it from Waco. |
| `PENDING` | Not supplied yet. The Note says what is missing and who supplies it. |

**`companies.csv`** is the scorecard table, one row per contractor, sorted by review count. Columns
match the table on the Waco page: Rank, Company, Reviews, Rating, Top3Map, NamedByAI,
RecommendedByAI, RunningAds, AIQuotableContent, Website.

**`assets.csv`** is what we need from you: five to eight local photographs with a shot description,
alt text and caption for each, plus one dated screenshot of the Google results page for
"emergency ac repair <city>". These are the only PENDING rows that are genuinely yours to fill.

## The copy

Most of the page is identical in every market with only the city name changed: Sarah's Take, the One
System section, all eight call-to-action banners, the pricing table, and the Method and Sources
footer. Lift those from the Waco reference and swap the city name.

Only two narrative paragraphs are genuinely per-market, and they arrive written in the handoff sheet.

## Page rules

- URL pattern `/market-report/<city>-<state>/`, for example `/market-report/plano-tx/`
- `noindex, nofollow`. These are outreach collateral, not SEO pages, and they name ten third-party
  companies.
- Never state a return on ad spend as fact. The Local Services Ads economics block is labelled
  illustrative on the Waco page and must stay that way.
- Pricing is Grow $2,200, Accelerate $3,500, Dominate $5,000, plus a $3,000 minimum ad budget.
- Phone (202) 400-2644. Case studies at rsgonzales.com/case-studies/.
- A blank in the data is a blank. If a value is PENDING and no fallback is given, drop that sentence
  or block rather than inventing a number. Every figure on these pages is checkable by the
  contractor reading it.

## What is not in this repo

Prospect email addresses, contractor owner names, and anything else from the outreach side. This
repo is for building pages.
