# The quality gate

Burke, 4 September: "They have to be perfect. That's our goal, to make sure this is completely
reproducible without any degradation whatsoever. We could do any city in North America."

That only holds if quality is enforced by something that does not get tired. This is that thing.

## The rule

```
node automations/scripts/validate-market.mjs <slug>
node automations/scripts/validate-market.mjs --all
```

Exit 0, it ships. Exit 1, it does not. No handoff sheet, no repo push, no page render, no deploy,
no email citing its numbers. This is Hard Rule 8 in RS Gonzales/CLAUDE.md.

## What it checks, and why each rule exists

Every rule was written because something actually went wrong. None of them is theoretical.

**Method proof**
- `method.location_id` - the first four markets were collected by querying city-qualified terms at
  national scope. Abilene read 510 and measures 970. A file with no location_id was collected the
  wrong way and its headline is understated.
- `method.read_stability` - the keyword API reports SUCCESS before the values populate. Waco moved
  590 to 670 and Tyler moved 1,040 to 510 between two reads of the same research. A single read
  silently undercounts.

**Arithmetic**
- `math.market_size` - market size must equal households times $800. The published Waco page says
  $50M while its own household count gives $48M.
- `math.searches_derivation` - the headline must equal the sum of its own per-term volumes. Waco
  published 3,470 with every term volume null, and no method has ever reproduced it.

**Scorecard integrity**
- `scorecard.tracked_count` - Waco declared 20 companies tracked while carrying 10 rows. Every
  "N of the nine" footnote on the page rests on that number.
- `scorecard.sort_order` - strict descending by review count. An out-of-order table is the first
  thing a contractor notices.
- `scorecard.rounded_reviews` - Waco shipped 1600, 800, 400, 350, 300, 250, 150. Sarah's live-Google
  figures differed on all ten companies. Counts rounded to the nearest 50 are estimates wearing a
  measurement's clothes.
- `scorecard.too_few` / `scorecard.thin` - the table needs ten, and a real market holds 21 to 27
  after filtering. Too few means the email audience below the top ten is missing.

**Claims and copy**
- `claims.roas` - return on ad spend is never stated as fact. The Local Services Ads block is
  labelled illustrative on the live page and stays that way.
- `claims.revenue` - the scaled-past-$5M sentence is gone. RSG has no revenue data.
- `claims.case_study` - Skyline, never Breeze. Sarah, 2 September.
- `claims.competitor` - no competitor is ever named.
- `prose.dashes` - no em dashes, en dashes or double hyphens.
- `prose.denominator` - denominators must match what was actually tracked or crawled. The 18 August
  fact-check retired "of 20".

**Honesty**
- `ai.engines_unrecorded` - copy names only the engines that actually returned an answer. The live
  Waco page claims three were queried at a time when only one could be reached.
- `flags.none` - every null carries a flag saying what was tried and why it is empty. A silent null
  becomes an invented number the next time someone fills it in.

## Adding a rule

When something goes wrong, add the rule and write the incident into its comment. That is why the
script reads like a history. A rule with no story behind it is a guess, and guesses produce false
failures that teach people to ignore the gate.

## Standing state

Run `--all` to see where every market stands. As of 4 September all five files fail on
`method.location_id`, which is correct: they were collected before the geo-target fix and are being
re-run now. Waco additionally fails on three counts that are all known and all documented above.
