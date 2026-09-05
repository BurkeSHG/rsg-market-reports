# City Report Template Contract
Source of truth: the web team's Waco page, https://waco-market-report.vercel.app/market-report/waco-tx/ (captured 2026-09-04, HTTP 200, 14,320px tall).
Burke's ruling, Sep 4: this page is THE template for every city report. Every future city supplies exactly the data below; the web team supplies the page.
Captures: packages/_template/webteam-waco.html (rendered DOM), webteam-waco.txt (all copy), webteam-waco.summary.json (headings, tables, images, links), webteam-waco-fullpage.png.

## 0. Companion document
packages/_template/VISUAL-INVENTORY.md is the visual teardown of the same page (Claude in Chrome, Sep 4): global layout system, section-by-section layout with light/dark alternation and background photos, image inventory (13 assets), CTA inventory (8 banners + 2 inline), and a 28-point variable map. Read both. This file is the data contract; that file is the look. Where the two differ, the page itself wins.

Items the visual teardown adds to the collect list below, so Session 2 gathers them too:
- Report month/year stamp (eyebrow and footer).
- SERP screenshot for "emergency ac repair <city>": capture date, whether an AI Overview appeared, and the sponsored listing's review count.
- Slow-month vs peak-month lead counts and the peak month name (LSA block).
- Housing-stock inputs behind the market-size math.
- 5-6 local landmark photos with captions AND alt text (the page uses landmark photography as section backgrounds, alternating dark photo sections with light ones).
- Bar-pair pick: one high-review company not in the top 3 and one low-review company in the top 3.

Structural rule from the teardown: every channel section follows eyebrow, headline, lead paragraph, one signature data visual, footnote, CTA banner. Swapping a market refills the visuals; it never rearranges the page.

## 1. Section inventory (page order)

| # | Section label / heading | What it shows | Level |
|---|---|---|---|
| 0 | Eyebrow: HVAC MARKET INTELLIGENCE / WACO, TEXAS · MARKET REPORT · JULY 2026 | City, state, report month | market |
| 1 | H1 "3,470 Homeowners Search for HVAC in Waco Every Month. Where Do You Show Up?" | Hero. Subhead, channel strip (GOOGLE MAPS · PAID SEARCH · AI ANSWERS), "Prepared by Sarah Gonzales", tagline. Hero photo (city landmark). | market + static |
| 2 | Four stat tiles | $50M+ residential spend, ~$20M decided online, 3,470 searches/mo, 44% of clicks to top-3 map | market (3) + static stat (44%) |
| 3 | CTA card "Get My Free 'HVAC in Waco' Audit" | 15-minute audit offer, city name in button | static, city merge |
| 4 | CHANNEL 1 · GOOGLE MAPS. H2 "See Exactly Where You Rank Against Every Major HVAC Company in Waco" | Intro (names core searches), 9-row scorecard table, legend (Observed / Not there / No public data), 2 narrative paragraphs naming companies, data note | per-company + market |
| 5 | "Review count against map placement" bar pair | One high-review company NOT in top 3 vs one low-review company IN top 3, bars scaled to market high | per-company (derived) |
| 6 | Source note | Reviews from GBP + month; top-3 observed for core searches; "N of the nine hold a top-three spot, so the third is held by a company outside this list" | market |
| 7 | H3 "Reviews Are Not the Whole Story" | Dimension explainer (why reviews alone do not win the map). City photo with caption. | static |
| 8 | CTA "Book a Straight-Talk Strategy Session" | | static |
| 9 | CHANNEL 2 · PAID SEARCH. H2 "Google Has Turned Into a Pay-to-Play Search Engine" | Intro paragraph | static, city merge |
| 10 | H3 "The Top of the Results Page Is Now Sold, Not Earned" | Annotated SERP screenshot with 4 numbered zones: 01 Bought at the top (55.8%, 2x), 02 Answered before the click (68%), 03 Now being sold too (3% to 22%), 04 What is left to earn. Then a plain-English description of what the screenshot shows and its date. | market (screenshot + description) + static stats |
| 11 | CHANNEL 2 · LOCAL SERVICES ADS. H3 "Local Services Ads Are the Closest Thing to Predictable HVAC Demand in Waco" | Intro, "feast or famine" framing | static, city merge |
| 12 | H4 "The Math That Makes Local Services Ads Worth It in Waco" | 3-box graphic: $60-105 per qualified lead, 80% close, 11x ROAS, labeled illustrative (Sarah's Aug 20 ask) | static |
| 13 | H4 "Why Most Waco Shops Get Feast or Famine From Local Services Ads" | 4-5 leads slow month vs 15-60 peak; "What decides your lead volume" 4 cards (review momentum, services promoted, market coverage, account management); famine/feast pair | static, city merge |
| 14 | CTA "Fix My Lead Volume" | | static |
| 15 | CHANNEL 2 · PAY-PER-CLICK. H3 "Pay-Per-Click Is What Separates the Shops That Scale From the Ones That Stall" | Intro; claim "every residential HVAC company in the greater Waco region that has scaled past $5 million runs PPC"; "more than half of Waco contractors do not run PPC"; CPC card $38; landing page vs homepage fork (5x to 8x vs Negative); source line | market (CPC, two claims) + static |
| 16 | CTA "See the Growth Programs" | | static |
| 17 | CHANNEL 3 · AI ANSWERS. H2 "AI Is Already Recommending Waco HVAC Companies by Name. Is It Recommending You?" | Intro naming engines and the mention-vs-recommend contrast (highest-reviewed not recommended vs lowest-reviewed recommended); 5-row AI table with badges; 2 narrative lines; source line | per-company + market |
| 18 | AI content gap | "Have a page built for AI to quote: NONE OF THE 5" / "Have any Q&A content: 1 OF THE 5"; 5-dot graphic; link to rsgonzales.com/llm-info/ | market (2 counts) |
| 19 | CTA "Check My AI Visibility" | | static |
| 20 | SEARCH TERMS. H2 "Which Waco Search Terms You Can Still Win, and Which Are Already Locked Up" | Intro; flywheel graphic (Sarah's Aug 20 ask: win jobs -> reviews -> organic -> ads); three lists Winnable / Contested / Locked, 4 terms each; source line | keyword + static |
| 21 | CTA "Get My Free Keyword Audit" | | static |
| 22 | SARAH'S TAKE. H2 "This Is Not a Lead Problem. It Is a System Problem." | Founder's note, Sarah photo, 3 paragraphs, "Book Free Session". City photo with caption. | static (city name merged in para 1) |
| 23 | ONE SYSTEM. H2 "Just Like HVAC Systems, Marketing Works Best When Every Component Works Together" | 2 intro paras; H3 "Here is how the pieces work together"; 4 blocks (Reviews, Website, Ad Spend, The Whole System) each with a client proof image; closing paras | static |
| 24 | CTA "Get a Plan Built for Your Niche" | | static |
| 25 | OUR PRICING. H2 "What It Costs to Work With Us" | 3 cards Grow / Accelerate / Dominate with fee, +$3,000 min ad budget, all-in; fine print (0% markup, website you own, no setup fees, 12-month lock, 30-day guarantee) | static |
| 26 | CTA "See Full Pricing" | | static |
| 27 | WHERE THIS GOES NEXT. H2 "3,470 Searches a Month. How Many End With Your Phone Ringing?" | Closing pitch; "Book My Waco Strategy Session"; audit alternative "Get My Free SEO Audit"; phone twice; 3 badges ($0 setup, 0% markup, 30-day). City photo with caption. | market (searches, city) + static |
| 28 | METHOD & SOURCES. H2 "How These Numbers Were Put Together" | H3 Method (sizing formula, volume source, reviews month, AI engines, keyword method, advertiser sources; disclaimers incl. which image is AI-generated); H3 Sources (5 citations, one per-city CPC line) | static + market (metro name, month, CPC) |
| 29 | Footer | "Marketing for HVAC and home-services contractors · rsgonzales.com · (202) 400-2644" | static |

19 headings (1 H1, 8 H2, 8 H3, 2 H4), 2 tables, 19 images (all inline base64 webp), 23 inline SVGs (bars, zone badges, flywheel, dots, icons). No external scripts, no external stylesheets: the page is fully self-contained.

## 2. Data contract: every field the page consumes

Session 2 (collect-market.mjs) must fill every non-static row. Null is allowed only where marked; a null must be flagged in the collection log, never estimated.

### Market level
| Field | Example (Waco) | Source | Nullable |
|---|---|---|---|
| city, state, state_abbr | Waco, Texas, TX | markets file | no |
| slug | waco-tx | markets file | no |
| metro_label | "the Waco metro" | markets file | no |
| report_month | July 2026 | collection date | no |
| collected_at | 2026-07 | collection date | no |
| core_terms | ["AC repair Waco", "HVAC Waco"] | fixed pattern per city | no |
| residential_hvac_spend_usd | $50M+ | Census owner-occupied housing (metro) x industry avg annual HVAC spend per home | no |
| online_decided_share_usd | ~$20M | 40% of spend (methodology page) | no |
| monthly_searches | 3,470 | Google Keyword Planner, core HVAC term set | no |
| map_pack_click_share | 44% | static industry stat (WebFX 2026); not per-city | static |
| companies_tracked | 9 | count of scorecard rows | no |
| market_high_reviews | 2,772 | max review_count in scorecard | derived |
| top3_holders_in_list | 2 | count of top3_map = Yes | derived |
| top3_outside_note | "the third is held by a company outside this list" | derived when top3_holders_in_list < 3 | derived |
| maps_narrative (2 paragraphs) | "Lochridge Priest dominates map visibility... Oasis proves that even 1,100+ reviews..." | written per city from scorecard | no |
| serp_query | emergency ac repair waco | fixed pattern | no |
| serp_screenshot | image | live Google search, logged-out, city geo | no |
| serp_screenshot_date | August 21, 2026 | capture | no |
| serp_description | sponsored listing with 6 reviews above locals with hundreds/thousands, then map, then first organic | written from screenshot | no |
| serp_ai_overview_present | false ("zone 02 is empty") | observed | no |
| paid_stats (55.8%, 2x, 68%, 3%->22%) | static | WebFX, ALM, SparkToro, Places Scout | static |
| ppc_cpc_ac_repair | $38 | live Google Ads / Keyword Planner CPC for "AC repair <city>" | no |
| ppc_scaled_claim | "every residential HVAC company in the greater Waco region past $5M runs PPC" | Ads Transparency Center check against known large shops | yes; drop sentence if unverified |
| ppc_share_not_running | "More than half of Waco HVAC contractors do not run Google PPC" | Ads Transparency Center across scorecard | yes; drop if unverified |
| lsa_economics ($60-105, 80%, 11x) | static, labeled illustrative | RSG account experience | static |
| lsa_lead_ranges (4-5 slow, 15-60 peak) | static | RSG | static |
| ai_engines_run | ChatGPT, Google AI Overviews, Perplexity | must be the engines actually queried | no |
| ai_prompt_set | "best HVAC company in Waco" family | fixed | no |
| ai_top5_quotable_page_count | 0 of 5 | website crawl of 5 highest-reviewed sites | no |
| ai_top5_qa_content_count | 1 of 5 | website crawl | no |
| ai_narrative_contrast | Lochridge-Priest 2,700+ not recommended; Polansky recommended with 467 | derived from AI table | derived |
| keywords_winnable[4] | furnace repair Waco, HVAC maintenance Waco, heating repair Waco, air duct cleaning Waco | live results-page analysis | no |
| keywords_contested[4] | HVAC installation Waco, best HVAC Waco, AC installation Waco, HVAC companies Waco TX | same | no |
| keywords_locked[4] | AC repair Waco, emergency HVAC Waco, AC repair near me, HVAC contractor Waco | same | no |
| photos[6-8] with alt text and caption | Suspension Bridge, Washington Ave Bridge, Waco home, ALICO x3, aerial x2 | licensed or original city photography; alt text written | no |
| sources_cpc_line | "Waco 'AC repair' cost per click about $38, live Google Ads data, July 2026" | derived | derived |

### Company level (scorecard: the N highest-reviewed HVAC companies serving the market; Waco shows 9)
| Field | Example | Source | Nullable |
|---|---|---|---|
| rank | 1..9 | order by review_count desc, except the page keeps Oasis at 4 below Clark; follow review_count strictly for new cities | derived |
| name | Lochridge Priest Home Services | Google Business Profile | no |
| review_count | 2,772 | GBP, live, unrounded | no |
| rating | 4.9 | GBP | no |
| top3_map | Yes / No | observed map pack for core_terms, logged-out, city geo | no |
| ai_named | Yes / No | engine responses mention the name | no |
| ai_recommended | Yes / No | engine responses recommend it | no |
| running_google_ads | Yes / No / No public data | Ads Transparency Center + live LSA unit; "No public data" when the advertiser cannot be resolved | third state allowed |

### AI table (top 5 by review_count from the scorecard)
| Field | Example | Source |
|---|---|---|
| name, review_count | as scorecard | scorecard |
| mentioned, recommended | YES/NO | scorecard ai_named / ai_recommended |
| badge | MOST REVIEWS, NEVER RECOMMENDED / IN BOTH / RECOMMENDED, NEVER MENTIONED | derived: top reviews with recommended=NO; both YES; recommended YES with mentioned NO |

### Bar-pair graphic
| Field | Example | Rule |
|---|---|---|
| not_top3_high | Danco 1,306 | highest review_count with top3_map = No |
| top3_low | Polansky 467 | lowest review_count with top3_map = Yes |

Field count: 34 market-level (27 collected or written, 7 static or derived), 8 per company x N companies, 3 derived per AI row, 2 derived for the bar pair. Session 2 must collect 27 market fields plus 8 fields for each of roughly 9 to 10 companies per city.

## 3. Per-company table as shown

| # | Company | Reviews | Rating | Top 3 on the map | Named by AI | Recommended by AI | Running Google ads |
|---|---|---|---|---|---|---|---|
| 1 | Lochridge Priest Home Services | 2,772 | 4.9 | Yes | Yes | No | No |
| 2 | Danco Heating, Cooling & Plumbing | 1,306 | 4.9 | No | Yes | Yes | Yes |
| 3 | Clark Heating and Air Conditioning, LLC | 584 | 5.0 | No | Yes | Yes | No |
| 4 | Oasis Heating & Cooling | 1,121 | 4.9 | No | Yes | No | No |
| 5 | Polansky Heating & Air | 467 | 4.9 | Yes | No | Yes | No |
| 6 | Comfort Plus Heating and Cooling LLC | 213 | 4.9 | No | No | No | Yes |
| 7 | Falcon 5 Plumbing & HVAC | 172 | 4.9 | No | No | No | Yes |
| 8 | Hobson AC | 97 | 4.8 | No | No | No | No public data |
| 9 | Zip Air | 72 | 4.8 | No | No | No | No public data |

AI table (top 5): Lochridge Priest 2,772 YES/NO (MOST REVIEWS, NEVER RECOMMENDED); Danco 1,306 YES/YES (IN BOTH); Oasis 1,121 YES/NO; Clark 584 YES/YES (IN BOTH); Polansky 467 NO/YES (RECOMMENDED, NEVER MENTIONED).

Note: Legacy Home Services (in both Sarah's Aug 21 rewrite at 2,828 and our render at 300) is absent from the web team page. Row 4 (Oasis 1,121) sits below row 3 (Clark 584), so the table is not strictly sorted; new cities should sort strictly by review_count.

## 4. Static copy blocks (unchanged across cities, city name merged where noted)

| Block | Heading | Length | City merge |
|---|---|---|---|
| Tagline | "We do marketing for HVAC and home-services contractors. Nothing else." | 1 line | none |
| Audit CTA card | "Get My Free 'HVAC in Waco' Audit" | 3 lines | city in button and body |
| Reviews explainer | "Reviews Are Not the Whole Story" | 2 paras | none |
| Pay-to-play intro | under "Google Has Turned Into a Pay-to-Play Search Engine" | 1 para | "Most Waco shops" |
| SERP zone stats | 55.8%, 2x, 68%, 3% to 22% | 4 badges | none |
| LSA intro + math + feast/famine + 4 cards | 3 headings | ~330 words | city in 2 headings |
| PPC intro + landing-page fork | 1 heading | ~180 words | city in 3 sentences, 2 of them factual claims (see contract) |
| AI content-gap explainer | "That gap is not a reputation gap..." | 2 paras | none |
| Keyword intro + flywheel | 1 para + graphic | ~110 words | none |
| Sarah's Take | "This Is Not a Lead Problem. It Is a System Problem." | 3 paras, ~170 words | "Waco has no shortage..." para 1 |
| One System | H2 + H3 + 4 blocks + 2 closing paras | ~330 words | none |
| Pricing | 3 cards + fine print | ~150 words | none |
| Closing | "3,470 Searches a Month. How Many End With Your Phone Ringing?" | 2 CTAs, 3 badges | searches + city |
| Method | 1 para + disclaimers | ~120 words | metro, month, engines |
| Sources | 5 citations | 5 lines | CPC line per city |
| Footer | rsgonzales.com · (202) 400-2644 | 1 line | none |

CTA targets (7 distinct): rsgonzales.com/seo-audit-for-hvac/, /book-strategy-session/ (x6 buttons), /hvac-seo-packages/, /llm-info/, /pricing/, tel:+12024002644. Phone appears 3 times.
Static images: RSG logo (x2), Sarah photo (x2), 4 client proof images (review carousel, GA report, Google Ads account, rank grid), kitchen illustration (AI-generated, disclosed).

## 5. Diff against our render (market-reports-navy.vercel.app/waco-tx/, render-report.mjs 3.0.0)

Sections only in the web team page: Hero stat tiles with "Prepared by Sarah Gonzales"; annotated SERP screenshot with 4 zones; the whole LSA block (math graphic, feast/famine, what decides lead volume); PPC landing-page fork; AI content-gap dots; keyword flywheel; Method & Sources; per-city photography with captions (8 city photos); "Reviews Are Not the Whole Story" explainer.

Sections only in ours: "$50 Million. That's What's on the Table" hero; "Three Companies Own the Map Pack"; "Ads Inside the Map Pack"; "What a Click Is Actually Worth"; "AI Visibility Scorecard"; "How a 100-Review Shop Can Beat a 2,000-Review Competitor"; "The Competitive Landscape at a Glance"; "The Big Money Is Already Here" (private equity); "How the Market Breaks Down" with Leaders / Rising / Established / Under the Radar tiers; "How Do I Catch Up?" (5 steps). None of these exist on the template.

Numbers that differ:
| Company | Ours | Web team |
|---|---|---|
| Lochridge Priest | 2,742 / 4.7 | 2,772 / 4.9 |
| Danco | 1,600 / 4.9 | 1,306 / 4.9 |
| Clark | 800 / 4.8 | 584 / 5.0 |
| Oasis | 461 / 4.8 | 1,121 / 4.9 |
| Polansky | 400 / 4.8 | 467 / 4.9 |
| Comfort Plus | 350 / 4.6 | 213 / 4.9 |
| Legacy Home Services | 300 / 4.7 | not on page |
| Falcon 5 | 250 / 4.5 | 172 / 4.9 |
| Hobson AC | 150 / 4.6 | 97 / 4.8 |
| Zip Air | 49 / 4.3 | 72 / 4.8 |
Market-level numbers only in ours: 64% concentration, $48M, 60,000 homes, $800/home, $2.5M, 40%, 733%, 78%, 10x, $200, 300K. None are on the template. Numbers only on the template: 55.8%, 68%, 3% to 22%, 2x, $60-105, 80%, 11x, 15-60, 4-5, $38, 5x to 8x.

What render-report.mjs would need to change to mirror the template: replace the section list wholesale with the 29 rows in section 1; drop tiers, catch-up, competitive landscape, PE, scorecard-of-AI; add hero tiles, SERP zone module (needs a screenshot asset per city), LSA block, PPC fork, AI dots, flywheel SVG, Method & Sources; switch the pricing table to three cards; add 8 photo slots with alt and caption fields; add the 9-row scorecard with a third "No public data" state; consume the field names in section 2. Not changed in this pass.

## 6. Diff against Sarah's Notion rewrite (Aug 21, 12 sections in STATUS.md)

The web team page IS Sarah's rewrite, built. Section order matches her page: hero + 4 tiles, Channel 1 table, Channel 2 (pay-to-play, LSA, PPC), Channel 3 AI, keyword lanes, Sarah's Take, One System, pricing, closing CTAs, Method & Sources. Her three Aug 20 comment asks are all built: the 3-box LSA graphic, the flywheel, and the "system problem for individual contractors" reframing appears in the AI/closing copy. The garbled pricing paragraph from her page is fixed on the site.

Review counts: the web team used Sarah's Aug 21 live-Google set (2,772 / 1,306 / 584 / 1,121 / 467 / 213 / 172 / 97 / 72), not the v3 rounded set. Differences from her page: Legacy Home Services (2,828 on her page) was dropped, so the table is 9 rows not 10; the AI table is trimmed to the top 5 by reviews. Everything else carries her numbers.

Our render carries none of her numbers and carries a company she listed. On the template, Waco's collected data problem is already solved: the numbers on the live web team page are the ones to treat as current.

## 7. Build notes

- URL pattern: /market-report/<slug>/ on the waco-market-report Vercel project (production alias waco-market-report.vercel.app). Expect the final home to be rsgonzales.com/market-report/<slug>/ per Sarah's build reference; confirm with the web team.
- Meta title: "Where <City> HVAC Companies Rank Online in 2026". Meta description: "See where every major HVAC company in <City> stands on Google Maps, paid ads, and AI answers, and which lanes are still open. Book a strategy session."
- Robots: meta robots "noindex, nofollow" AND response header X-Robots-Tag: noindex, nofollow, noarchive, nosnippet, noimageindex.
- Images: all 19 are inline base64 webp. No external assets, scripts, or stylesheets. Page is one self-contained HTML document (3.06 MB rendered).
- Per-city assets the web team needs supplied: 6 to 8 city photographs with alt text and caption (landmarks, a typical home, aerials); one annotated SERP screenshot for "emergency ac repair <city>" with capture date and a plain-English description; the scorecard, AI table, bar-pair, keyword lanes, and all market numbers from section 2; the two narrative paragraphs for Channel 1; the AI contrast sentence; the CPC. Everything else is static copy they already hold.
- Charts are inline SVG generated from the numbers (bars, dots, flywheel); no chart images need supplying.
