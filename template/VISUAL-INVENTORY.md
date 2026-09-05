# Waco HVAC Market Report — Template Teardown

**Source:** `https://waco-market-report.vercel.app/market-report/waco-tx/`
**Page title:** Where Waco HVAC Companies Rank Online in 2026
**Captured:** September 4, 2026 (page data is stamped "July 2026")
**Brand:** RS Gonzales · phone (202) 400-2644 · rsgonzales.com

Two parts below: **Part A** is the layout report (structure, component types, order). **Part B** is the complete data inventory (every value, verbatim). **Part C** is the variable map for cloning to a new market.

---

# PART A — LAYOUT REPORT

## Global layout system

| Property | Value |
|---|---|
| Container | Single centered column, ~1,265px content width inside a full-bleed section wrapper. No sidebar, no sticky nav. |
| Total page length | ~22,000px (very long scroll, 13 stacked bands) |
| Section rhythm | Alternating **dark band** / **light band**. Dark bands are near-black with a dimmed photographic background at very low opacity. Light bands are white/off-white. |
| Section anchor pattern | Every band opens with a small colored **eyebrow label** (icon + ALL-CAPS letterspaced text), then an H2, then a lead paragraph. |
| Accent colors | Green `#2E7D52`-ish (primary CTA, positive), Blue (AI / paid), Red/maroon (negative / gap), Yellow-gold (review-count bars), Dark navy table headers |
| Repeating CTA component | Full-width rounded card with a **green left border stripe**, a square icon tile on the left, bold question + explanatory sentence, and a pill CTA button on the right. Appears at the end of **8** sections. |
| Footnote pattern | Small grey sentence directly under each data component, stating source + "July 2026". |
| Callout pattern | Tinted box with a green left border, holding a single bolded takeaway sentence. |
| Mobile affordance | Both tables carry a "Swipe the table sideways to see every column" hint. |
| Photo caption pattern | Full-width rounded photo with an ALL-CAPS caption overlaid bottom-left. |

## Section order and internal layout

### 0. Header bar — dark, over hero photo
- Left: RS Gonzales logo mark (upward-arrow-over-bars) + wordmark
- Right: `HVAC MARKET INTELLIGENCE` (small caps, letterspaced, grey)
- Thin horizontal divider rule below

### 1. Hero — dark, background photo (Waco Suspension Bridge at dusk)
Two-column asymmetric split (left ~55%, right ~45%), right column starts lower.

- **Left column (top to bottom):** green dot + eyebrow `WACO, TEXAS · MARKET REPORT · JULY 2026`; giant H1 with the lead number in green; 3-line lead paragraph; small caps channel line `GOOGLE MAPS · PAID SEARCH · AI ANSWERS`; horizontal rule; byline row = circular headshot + "Prepared by Sarah Gonzales" + one-line positioning sentence.
- **Right column:** one bordered card containing a **2×2 stat grid** (thin dividers between quadrants). Each cell = large number, then 2–3 line label.
- **Below both columns, full width:** CTA banner #1.

### 2. Channel 1 · Google Maps — light
- Eyebrow (map-pin icon) `CHANNEL 1 · GOOGLE MAPS`
- H2, then 4-line intro paragraph
- Callout box: reputation vs visibility definition
- **Competitor table** (the page's centerpiece):
  - Dark navy header row for the first three columns (`#`, `Company`, `Reviews`, `Rating`), then **four color-coded header cells**: red `Top 3 on the map`, blue `Named by AI`, green `Recommended by AI`, dark blue `Running Google ads`
  - 9 numbered rows. `Reviews` cell = number stacked above a **gold horizontal bar** scaled against the market high (2,772)
  - Visibility cells render as **filled dots** in the column's color = observed, hollow grey dot = not there, hatched dot = no public data
  - Legend row beneath: Observed / Not there / No public data
  - Grey takeaway panel with two bolded lead-ins
  - Footnote line
- **Two-column block:** left = bordered card "Review count against map placement" (2 horizontal bars with right-aligned status labels + bar-scale footnote); right = H3 "Reviews Are Not the Whole Story" + 2 paragraphs
- Footnote under the left card
- Full-width photo (Washington Avenue Bridge) with overlaid caption
- CTA banner #2

### 3. Channel 2 · Paid Search — dark, background photo (Waco clapboard home)
- Eyebrow (magnifier icon) `CHANNEL 2 · PAID SEARCH`
- H2, 2-line intro
- H3 "The Top of the Results Page Is Now Sold, Not Earned"
- **Two-column annotated screenshot layout:**
  - Left (~60%): a mock browser chrome (three dots + URL pill showing the query) framing a real Google SERP screenshot. **Numbered blue zone badges `01`–`04`** are pinned on the screenshot with vertical bracket lines marking regions (01 sponsored listing, 03 Businesses/map pack, 04 first organic result)
  - Right (~40%): a stacked rail of **four numbered zone stat blocks**, each = `NN` badge + ALL-CAPS zone name, a big blue statistic, a progress bar, an explanatory sentence, and (zone 01) a small inset `2×` note. Zone 03 uses a two-row before/after bar chart (Nov 2025 / Jan 2026). Zone 04 has no number, just a bold sentence.
- Below, three small grey caption paragraphs explaining the screenshot, then a disclaimer sentence
- **No CTA banner in this section**

### 4. Channel 2 · Local Services Ads — light, no background photo
- Eyebrow (shield-check icon) `CHANNEL 2 · LOCAL SERVICES ADS`
- H2, one-line italic-style prompt, then 2 paragraphs, then a bolded one-liner
- H3 with an inline ALL-CAPS subtitle to its right (`COST PER QUALIFIED LEAD · CLOSE RATE · RETURN ON AD SPEND`)
- **Three-card horizontal flow diagram**, gradient-filled, joined by gold arrows with labels between them:
  - maroon card → arrow `OF WHICH YOU CLOSE` → navy card → arrow `WHICH RETURNS` → green card
  - Each card = small caps kicker, huge figure, sub-label
- Footnote
- H3 "Why Most Waco Shops Get Feast or Famine…", 4 paragraphs
- **Dark two-column panel:** left = "WHAT DECIDES YOUR LEAD VOLUME" with 4 colored-bullet items (bold title + 2-line description, separated by rules); right = green sub-panel "THE DIFFERENCE BETWEEN FAMINE AND FEAST" holding two side-by-side tiles (hatched "THE FAMINE" tile, solid "THE OPPORTUNITY" tile). Dashed curved connector lines fan from the 4 left items into the right panel.
- Two closing lines (one plain, one bold)
- CTA banner #3

### 5. Channel 2 · Pay-Per-Click — dark, background photo (downtown ALICO street)
- Eyebrow (cursor icon) `CHANNEL 2 · PAY-PER-CLICK`
- H2, 2-line intro
- Callout box (the $5M observation)
- One paragraph
- **Branching pathway diagram**, left to right:
  - Left: small card `COST PER CLICK` / `$38` / caption
  - Middle: small bordered node "Where the click lands / You control this"
  - Right: two stacked outcome panels — top (green-tinted, solid) holds two pill labels and a right-aligned `5× to 8×` + `BACK FOR EVERY DOLLAR SPENT`; bottom (hatched, grey) holds one pill label and a right-aligned `Negative` + `THE SPEND LEAKS AWAY`
  - A solid green curve connects to the good path, a dashed grey arrow to the bad path
- Footnote
- CTA banner #4

### 6. Channel 3 · AI Answers — light
- Eyebrow (green dot) `CHANNEL 3 · AI ANSWERS`
- H2, 2-line intro
- **AI visibility table**, 5 rows, 4 columns:
  - Dark navy header for `Company` and `Google reviews`, then blue `Mentioned by AI`, green `Recommended`
  - Company cell can carry an inline **status pill** (outlined grey, solid green, or light green)
  - `Google reviews` cell = number over a gold bar
  - Yes/No rendered as blue pill / green pill / plain grey "NO"
  - Polansky's row carries a green left-edge accent stripe
  - Grey takeaway panel with bolded lead-in
- Two footnote lines
- **Two-column block:** left = 2 paragraphs (with an inline link on "AI search reference page"); right = two gradient stat cards side by side (maroon, navy). Each card = statement, a row of **5 dashes** acting as a dot-plot (filled = yes), then an ALL-CAPS result line. Shared caption under both.
- CTA banner #5

### 7. Search Terms — dark, background photo (aerial downtown Waco)
- Eyebrow (green dot) `SEARCH TERMS`
- H2, 4-line intro
- **Flywheel diagram:** a large donut/wheel split into 4 labeled segments with green triangular direction arrows between them, and a center hub reading `REINFORCING LOOP` + a 3-line bold statement. A dashed blue line from outside the wheel connects to a dotted-border side card `AD SPEND IN`.
- Footnote
- **Three-tier keyword grid:** a full-width gradient bar (green → grey) with `OPEN TO YOU NOW` at far left and `LOCKED UP` at far right, then three equal columns divided by vertical rules:
  - `Winnable` `4 TERMS` — green-outlined pills
  - `Contested` `4 TERMS` — grey-outlined pills
  - `Locked` `4 TERMS` — grey-outlined pills
- Right-aligned footnote
- CTA banner #6

### 8. Sarah's Take — light
- Eyebrow (green dot) `SARAH'S TAKE`
- Full-width H2
- **Two-column block:** left (~35%) = tall portrait photo card with a white `Founder's Note` pill badge top-left and a bottom overlay containing name, "Owner, RS Gonzales", and a green `Book Free Session ›` button. Right (~65%) = 2 paragraphs then a green-bordered callout paragraph ending in a bolded sentence.
- Full-width photo (ALICO Building) with overlaid caption

### 9. One System / How the pieces fit — light
- Eyebrow (green dot) `ONE SYSTEM. EVERY CHANNEL WORKING TOGETHER.`
- H2, 2 paragraphs (second ends in a bolded clause)
- H3 "Here is how the pieces work together"
- **2×2 card grid.** Each card = full-bleed screenshot/photo image on top, then a solid green **category pill**, then a bold card title, then a 3–4 line paragraph.
- Closing paragraph opening with a bolded sentence
- CTA banner #7

### 10. Pricing — dark, background photo (ALICO at sunset)
- Eyebrow (green dot) `OUR PRICING`
- H2, 2-line intro
- **Three pricing cards.** Middle card is filled solid green (visually promoted); outer two are dark translucent. Each card top-to-bottom: tier name, ALL-CAPS revenue band, large monthly fee in green (outer) / white (middle), `PER MONTH`, divider, `+ $3,000 MINIMUM AD BUDGET`, all-in figure, `All-in per month`, divider, one-sentence scope description.
- **Disclaimer banner:** dark card with green left stripe, tag icon, a 5-line block whose first sentence is bolded, and a `See Full Pricing` pill on the right.

### 11. Where This Goes Next — light
- Eyebrow (green dot) `WHERE THIS GOES NEXT`
- H2 (reuses the hero's search-volume number), intro paragraph ending in a bolded sentence
- **Two-column block:** left (~40%) = tall photo (woman on phone in a kitchen); right (~60%) = two stacked green-bordered CTA cards, each = icon tile, bold lead-in + copy including the phone number, and a green pill button
- **Three-up trust stat row** beneath, divided by vertical rules: big figure + ALL-CAPS label
- Full-width photo (Waco at first light, aerial) with overlaid caption

### 12. Method & Sources — dark, background photo (aerial farmland edge of Waco)
- Eyebrow (green dot) `METHOD & SOURCES`
- H2
- **Two columns:** left = flask icon + `Method` + 2 paragraphs; right = book icon + `Sources` + a 5-item **numbered list** with green numerals
- Divider rule
- **Footer row:** RS Gonzales logo left; centered/right text `Marketing for HVAC and home-services contractors · rsgonzales.com · (202) 400-2644` with the phone as a green `tel:` link

---

# PART B — DATA INVENTORY

## B1. Hero stats

| Value | Label |
|---|---|
| 3,470 | Homeowners searching for HVAC in Waco every month (headline figure) |
| $50M+ | Residential HVAC spend in the Waco metro every year |
| ~$20M | The share decided online before a homeowner calls |
| 3,470 | High-intent HVAC searches every month |
| 44% | Of local clicks go to the top three map results |

Byline: **Prepared by Sarah Gonzales** — "We do marketing for HVAC and home-services contractors. Nothing else."

## B2. Google Maps competitor table (9 rows)

| # | Company | Reviews | Rating | Top 3 map | Named by AI | Recommended by AI | Running Google ads |
|---|---|---|---|---|---|---|---|
| 1 | Lochridge Priest Home Services | 2,772 | 4.9 | Yes | Yes | — | — |
| 2 | Danco Heating, Cooling & Plumbing | 1,306 | 4.9 | — | Yes | Yes | Yes |
| 3 | Clark Heating and Air Conditioning, LLC | 584 | 5.0 | — | Yes | Yes | — |
| 4 | Oasis Heating & Cooling | 1,121 | 4.9 | — | Yes | — | — |
| 5 | Polansky Heating & Air | 467 | 4.9 | Yes | — | Yes | — |
| 6 | Comfort Plus Heating and Cooling LLC | 213 | 4.9 | — | — | — | Yes |
| 7 | Falcon 5 Plumbing & HVAC | 172 | 4.9 | — | — | — | Yes |
| 8 | Hobson AC | 97 | 4.8 | — | — | — | No public data |
| 9 | Zip Air | 72 | 4.8 | — | — | — | No public data |

Bar scale: market high **2,772**. Note in footnote: only two of the nine hold a top-three spot, so the third is held by a company outside the list.

**Secondary bar chart — "Review count against map placement"**
- Danco Heating, Cooling & Plumbing — 1,306 — `NOT IN THE TOP 3`
- Polansky Heating & Air — 467 — `TOP 3 ON THE MAP`

## B3. Paid search zone stats (annotated SERP)

| Zone | Label | Figure | Meaning |
|---|---|---|---|
| 01 | BOUGHT AT THE TOP | **55.8%** | Of clicks land above the free results when Local Services Ads are running. Inset: **2×** — paid clicks have doubled in a year. |
| 02 | ANSWERED BEFORE THE CLICK | **68%** | Of Google searches end without a click to any website (Gemini / AI Overviews). Note: no AI Overview appeared on this search, so zone 02 is empty on the screenshot. |
| 03 | NOW BEING SOLD TOO | **3% → 22%** | Map-pack ads, **Nov 2025** → **Jan 2026** |
| 04 | WHAT IS LEFT TO EARN | — | "Everything you can still earn without paying sits below all of it." |

Screenshot metadata: query `emergency ac repair waco`, captured **August 21, 2026**. First result is a Sponsored Google Maps listing with only **6** reviews. Visible SERP entities include TexTech Services (5.0, 6), Evergreen Heating and Cooling (4.8, 870), Lochridge Priest (4.9, 2.8K), Clark Heating and Air (5.0, 585), and organic result P&E Mechanical.

## B4. Local Services Ads economics

| Stage | Figure | Label |
|---|---|---|
| WHAT IT COSTS | **$60–105** | per qualified lead |
| WHAT YOU CONVERT | **80%** | of qualified calls booked |
| WHAT COMES BACK | **11×** | return on ad spend |

Volume contrast: **4–5** qualified leads in a slow month vs **15–60** qualified leads during peak cooling demand (peak month cited: July).

**Four drivers of lead volume:** Your review momentum · The services you promote · Your market coverage · Your account management.

## B5. Pay-per-click

| Item | Value |
|---|---|
| Cost per click, "AC repair" in Waco | **$38** |
| Good path (keyword research + dedicated landing page with an offer) | **5× to 8×** back for every dollar spent |
| Bad path (straight to your homepage) | **Negative** — the spend leaks away |
| Market claim | Every residential HVAC company in the greater Waco region past **$5 million** in revenue runs Google PPC; more than half of Waco HVAC contractors run no PPC at all |

## B6. AI answers table (5 rows)

| Company | Status pill | Google reviews | Mentioned by AI | Recommended |
|---|---|---|---|---|
| Lochridge Priest Home Services | MOST REVIEWS, NEVER RECOMMENDED | 2,772 | Yes | No |
| Danco Heating, Cooling & Plumbing | IN BOTH | 1,306 | Yes | Yes |
| Oasis Heating & Cooling | — | 1,121 | Yes | No |
| Clark Heating and Air Conditioning, LLC | IN BOTH | 584 | Yes | Yes |
| Polansky Heating & Air | RECOMMENDED, NEVER MENTIONED | 467 | No | Yes |

**Content-gap dot cards** (each has 5 dots = the 5 highest-reviewed sites):
- "Have a page built for AI to quote" → **None of the 5** (0 filled)
- "Have any question-and-answer content" → **1 of the 5** (1 filled)

Assistants tested: ChatGPT, Google AI Overviews, Perplexity.

## B7. Flywheel (illustrative, not measured)

Segments in order: **Win more jobs** ("The calls already there") → **Earn more reviews** ("Every job earns one more") → **More organic leads** ("Reviews move them up the map") → **Fund more ads** ("Leads fund the next round") → back to Win more jobs.
Hub: `REINFORCING LOOP` — "Every turn makes the next turn easier."
External input card: `AD SPEND IN` — "New money entering the wheel from outside."

## B8. Keyword tiers (12 terms, 4 per tier)

| Winnable | Contested | Locked |
|---|---|---|
| furnace repair Waco | HVAC installation Waco | AC repair Waco |
| HVAC maintenance Waco | best HVAC Waco | emergency HVAC Waco |
| heating repair Waco | AC installation Waco | AC repair near me |
| air duct cleaning Waco | HVAC companies Waco TX | HVAC contractor Waco |

Core searches used for map/AI testing: "AC repair Waco" and "HVAC Waco".

## B9. Pricing

| Tier | Revenue band | Management fee | Min ad budget | All-in / month | Scope |
|---|---|---|---|---|---|
| Grow | Under $1M revenue | $2,200 | + $3,000 | $5,200 | First complete setup: Google Business Profile, reviews, organic search, light paid search. |
| **Accelerate** (highlighted) | $1M to $3M revenue | $3,500 | + $3,000 | $6,500 | Adds Google paid search, Local Services Ads, Meta retargeting, and the content engine. |
| Dominate | $3M to $15M revenue | $5,000 | + $3,000 | $8,000 | Full stack: Local Services, paid search, Meta, Yelp where it fits, AI search, content, CRM, email. |

Terms stated: ad spend paid directly to Google/Meta/Yelp at **0% markup**; every program includes a website you own, **no setup fees**, **locked pricing for 12 months**, **30-day money-back guarantee**.

## B10. Closing trust stats

| $0 | 0% | 30-Day |
|---|---|---|
| SETUP FEES | MARKUP ON AD SPEND | MONEY-BACK GUARANTEE ON EVERY PROGRAM |

## B11. Method

Market sizing: U.S. Census owner-occupied housing for the Waco metro × industry-average annual HVAC spend per home. Search volume: Google Keyword Planner. Reviews and ratings: Google Business Profiles, July 2026. AI testing: ChatGPT, Google AI Overviews, Perplexity. Keyword competition: live results-page analysis. Advertiser activity: live Google Local Services unit and Google Ads Transparency Center.

Disclaimers: market-size figures are directional estimates; every number is a July 2026 snapshot; industry percentages are third-party figures, not RS Gonzales client results; photographs are illustrative and do not depict any company named; the kitchen illustration is AI-generated, every other image is a real photograph or a real screen capture.

## B12. Sources (5, numbered)

1. WebFX 2026 — map pack about 44% of clicks, about 98% of local pages, 55.8% above organic with Local Services Ads.
2. SparkToro / Datos 2026 — about 68% zero-click.
3. Places Scout / PPC.land 2026 — map-pack ads under 3% to about 22%, November 2025 to January 2026.
4. ALM Corp 2026 — paid click share doubled, organic down 23%, text ads 9% to 16%.
5. Waco "AC repair" cost per click about $38, live Google Ads data, July 2026.

## B13. CTA inventory (8 banners + 2 inline buttons)

| # | Section | Question / lead-in | Button | Destination |
|---|---|---|---|---|
| 1 | Hero | Want your shop's own review, map, and AI numbers, not the market's averages? | Get My Free "HVAC in Waco" Audit | `/seo-audit-for-hvac/` |
| 2 | Google Maps | Not where you'd like to be on this list? | Book a Straight-Talk Strategy Session | `/book-strategy-session/` |
| 3 | Local Services Ads | We review your review pace, GBP, website services, and current LSA setup… | Fix My Lead Volume | `/book-strategy-session/` |
| 4 | Pay-Per-Click | Want to know what a click should cost you in Waco? | See the Growth Programs | `/hvac-seo-packages/` |
| 5 | AI Answers | Want to see what AI says about your company today? | Check My AI Visibility | `/book-strategy-session/` |
| 6 | Search Terms | Want to know which Waco terms you could own first? | Get My Free Keyword Audit | `/seo-audit-for-hvac/` |
| 7 | One System | Want to see what your complete marketing system could look like? | Get a Plan Built for Your Niche | `/book-strategy-session/` |
| 8 | Pricing | These are our monthly management fees, not your ad budget. | See Full Pricing | `/pricing/` |
| — | Sarah's Take (inline) | — | Book Free Session › | `/book-strategy-session/` |
| — | Where This Goes Next | Talk it through with us. / Or start with the audit. | Book My Waco Strategy Session · Get My Free SEO Audit | `/book-strategy-session/` · `/seo-audit-for-hvac/` |

Other links: inline "AI search reference page" → `rsgonzales.com/llm-info/`; three `tel:+12024002644` links.

## B14. Image inventory (13 assets, per alt text)

| # | Placement | Subject |
|---|---|---|
| 1 | Hero background | Waco Suspension Bridge over the Brazos at dusk, two people on a bench |
| 2 | Header + footer | RS Gonzales logo (×2 instances) |
| 3 | Hero byline + Sarah's Take | Sarah Gonzales headshot (×2 instances) |
| 4 | Google Maps section | Washington Avenue Bridge, steel truss span from a grassy bank |
| 5 | Paid Search background | Single-storey Waco home, pale clapboard siding, red brick chimney |
| 6 | Paid Search content | Google results page for "emergency ac repair waco" |
| 7 | Pay-Per-Click background | Downtown Waco street, ALICO tower over brick storefronts |
| 8 | Search Terms background | Downtown Waco from the air, ALICO above a grid of blocks |
| 9 | Sarah's Take | ALICO Building on Austin Avenue at golden hour |
| 10 | One System card 1 | Client website with Google reviews in a branded carousel |
| 11 | One System card 2 | HVAC client website beside its Google Analytics engagement report |
| 12 | One System card 3 | Client Google Ads account showing cost, phone calls, pipeline value |
| 13 | One System card 4 | Client local map-pack rank grid with keyword/backlink/traffic metrics |
| 14 | Where This Goes Next | Woman in a home kitchen on a smartphone (AI-generated, per the method note) |
| 15 | Where This Goes Next | Waco from the air at first light, river through dark farmland |
| 16 | Method & Sources background | Edge of Waco from the air, roads through wooded farmland |

---

# PART C — VARIABLE MAP FOR CLONING

## Must be re-researched per market (28 data points)

1. City / state / metro name (appears ~40+ times, including in headings, keyword strings, CTA button labels, and the URL slug)
2. Report month/year stamp
3. Monthly high-intent search volume (used twice: hero H1 and closing H2)
4. Annual residential HVAC metro spend
5. Online-decided share of that spend
6. Top-3 map click share (or reuse the 44% third-party figure)
7. Competitor table: 9 companies × (name, review count, rating, top-3 map, named by AI, recommended by AI, running ads)
8. Market-high review count (drives every bar scale)
9. Which two of nine hold top-three (footnote logic)
10. Secondary bar chart pair: one high-review company not in top 3, one low-review company in top 3
11. SERP screenshot for `emergency ac repair <city>` + capture date + the sponsored listing's review count
12. Whether an AI Overview appeared (drives zone 02 copy)
13. LSA cost per qualified lead range
14. LSA close rate and ROAS
15. Slow-month vs peak-month lead counts + peak month name
16. Cost per click for "AC repair <city>"
17. Revenue threshold observation ($5M) and the "more than half don't run PPC" claim
18. AI table: 5 companies × (review count, mentioned, recommended) + which status pill each earns
19. Content-gap counts (0 of 5, 1 of 5)
20. 12 keyword terms split across winnable / contested / locked
21. Core search terms used for map + AI testing
22. Local landmark photography (5–6 background/feature photos with captions)
23. Local landmark alt text
24. Housing-stock inputs for the market-size math

## Fixed / brand-level (reusable as-is)

- All 8 CTA banners and their destinations (only the city name inside CTA #1's label changes)
- Pricing table (3 tiers, fees, ad-budget minimum, terms)
- Closing trust stats ($0 / 0% / 30-Day)
- Sarah's Take section (all copy, headshot, badge, button)
- One System 2×2 card grid (images and copy are client-work screenshots, not market-specific)
- Method paragraph structure and the 5 numbered sources (source #5 carries the city CPC)
- Phone number, footer, logo
- Every structural component: eyebrow labels, table styling, dot legends, flow diagrams, flywheel, tier grid, callout and footnote patterns

## Structural note

The report is built as a **channel narrative**: Channel 1 (Maps) → Channel 2 (Paid: three sub-sections) → Channel 3 (AI) → Search Terms → founder POV → system pitch → price → close → method. Every channel section follows the identical five-beat rhythm: **eyebrow → headline → lead paragraph → one signature data visual → footnote → CTA banner**. That rhythm is the template; swapping a market means refilling the visuals, not rearranging the page.
