# City Report: the whole thing on one page

Plug in six inputs per city. Everything else is arithmetic or the same in every city. The web team does the design.

## 1. INPUTS you collect per city (six calls, one script run)

| # | What | Where it comes from |
|---|---|---|
| 1 | Households | `data/texas-markets.json`, already built for all 82 Texas markets |
| 2 | Geo target ID | Google's geotargets CSV, matched on full canonical name. Waco 1026867, Abilene 1026170, Plano 1026695, Tyler 1026855, The Woodlands 9052976 |
| 3 | Monthly searches + cost per click | Search Atlas keyword research: GENERIC terms, `location_id` = the geo ID. De-duplicate close variants. |
| 4 | Keyword lanes | Same call. Sort the terms by paid competition, split into thirds: winnable, contested, locked. |
| 5 | Top 10 companies + their scores | Google Places (name, reviews, rating), Maps check (top 3 yes/no), Ads Transparency (running ads yes/no), site crawl (AI-quotable content yes/no) |
| 6 | AI answers | Search Atlas prompt simulation, five engines. Match returned domains to the 10 companies to set mentioned and recommended. |

Assets the web team needs on top: five to eight city landmark photos with captions, and one dated screenshot of the Google results page.

## 2. ARITHMETIC (no research, just math)

```
households            = population / 2.8
market size $         = homes x $800/year
share decided online  = 40% of market size
reviews rank          = sort companies by review count, descending, strictly
tiers                 = Leaders / Rising / Established / Under the Radar, by review count
lanes                 = 12 terms sorted by paid competition, split 4 / 4 / 4
```

**RESOLVED Sep 4.** Two bases existed. The legacy Waco file used 60,000 homes, which is city-level, and rounded $48M up to the published "$50M+". `data/texas-markets.json` uses 75,700 households, which is the whole market footprint including the alias towns, and gives $60.6M.

**Use the market footprint.** It matches how a market is defined everywhere else in this campaign, and it is reproducible from Census figures without judgement. Waco therefore computes to $60.6M, and the published "$50M+" is still true at that number, so the live page needs no correction on this figure. State the basis in the Method footer: households in the market footprint, Census 2024, times $800.

## 3. CONSTANTS (identical in every report, never researched again)

| Constant | Value |
|---|---|
| Annual residential HVAC spend per home | $800 |
| Share of clicks to the top 3 map results | 44% |
| Searches ending with no click | 68% |
| Pricing | Grow $2,200, Accelerate $3,500, Dominate $5,000, plus $3,000 minimum ad budget |
| Guarantee | 30 days |
| Phone | (202) 400-2644 |
| Case studies | rsgonzales.com/case-studies/, use Skyline |

Static copy blocks, written once and reused with only the city name swapped: Sarah's Take, One System, all calls to action, Method and Sources.

## 4. Worked, batch 1

| Market | Homes | Market size | Monthly searches | Cost per click |
|---|---|---|---|---|
| Waco | 75,700 | $60.6M | 660 | $31.67 |
| Plano | 107,000 | $85.6M | 2,300 old method | in file |
| Tyler | 49,300 | $39.4M | 510 old method | in file |
| Abilene | 49,400 | $39.5M | 510 old method / 970 measured | $34.09 |
| The Woodlands | 45,400 | $36.3M | 900 old method | in file |

Only Waco and Abilene have been measured with the geo-target method. The four collected market files still hold old-method numbers, taken from city-qualified terms at national scope. Abilene is the proof of the difference: 510 in the file against 970 measured correctly. All four need one re-run before any page ships.

## 5. Throughput

Report production is not the constraint. Sending is.

```
1 market  = ~20 companies x 5 emails = ~100 emails
send rate = 25 to 30 per day
so        = ~4 days of sending per market
           = ~7 markets per month
80 markets = about 11 months of Texas
```

Build four to eight markets ahead of the send queue and no further. The other constraint is how fast the web team can turn a package into a page, which is an open question for Sarah.
