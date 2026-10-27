# Open items

The backlog the 48-hour standup pulls from. Everything identified but not yet
committed to a cycle lives here with an owner and a date.

**This is not the commitment list.** `/standup` takes **one** item per person per
cycle from here and moves it into `company/momentum.md`. An item sitting here with a
date in the past gets raised at the next standup.

**Opened:** 2026-10-27 (founding interview) · **Dated:** 2026-10-27, first standup

---

## This week — committed

| # | Item | Owner | By | Why it matters |
|---|---|---|---|---|
| 1 | **Post-mortem on the 9,000 MXN prosthesis failure.** Outsourced digital design was wrong and nobody caught it mid-process. Write it up in `customers/`. | Alex | **2026-10-31** | Largest single revenue loss on record; the cause is a missing checkpoint, not bad luck |
| 2 | **Add a design approval checkpoint before manufacture.** Alex reviews every outsourced design before anything is printed or milled. | Alex | **2026-10-29** | Design is outsourced and currently unguarded — the failure mode we sell against |
| 3 | **Talk to Rosario's replacement at Omnidental.** Make sure the incoming dentist keeps sending printed restorations. | Alex | **2026-10-29** | 100% of revenue depends on it; a new dentist forms lab habits in week one |
| 4 | **Decide the furnace: use it or exit it.** 12,500 MXN/month against no ceramics work being done. | Alex | **2026-11-03** | ~49% of fixed costs, possibly for an idle asset |
| 5 | **Reprice the minimum consumption above breakeven.** Current 18,000 MXN sits below the ~29,900 MXN/month needed to cover fixed costs (furnace 12,500 + lease 12,600). | Alex | **2026-11-05** | Every scanner placed at 18k locks in a loss-making clinic |
| 6 | **Decide the scanner spec for placements at scale.** Not a cost question — at 48–60mo with 30% residual a 200k TRIOS is ~4–4.5k/mo vs Runyes 3,500. Decide on *scan quality*, measured. | Alex | **2026-11-10** | A cheap scanner that scans badly causes remakes — the exact failure we sell against |

## Next — dated, not yet committed

| # | Item | Owner | By | Why it matters |
|---|---|---|---|---|
| 7 | **Scope out anterior aesthetic cases.** Written policy + a script for declining them. | Alex | **2026-11-05** | 6 botched veneers; the material's known weak spot and the least forgiving audience |
| 8 | **Set the quality tripwire threshold.** Proposed: stop signing clinics when loss rate exceeds 15% of potential monthly revenue. Currently ~37%. | Alex | **2026-10-31** | Chosen now while hypothetical, not during a crisis |
| 9 | **Start the longevity log.** Every printed unit placed: date, tooth, type, clinic, photo. Backfill the 1-year 3-unit posterior bridge. | Alex | **2026-10-31** | In 18 months this is the only clinical evidence base in the market. Nobody else is building one |
| 10 | **Ask Rosario why she actually buys** — price, case margin, or speed. | Alex | **2026-10-31** | The whole message depends on which; we are currently guessing |
| 11 | **Get the X-ray lab facts:** name, number of orthodontists served, studies/month, price per model, who signs. | Alex | **2026-10-29** | Channel that may be worth more than several direct clinics |
| 12 | **Re-approach the churned doctor** with a Runyes-based structure and a lower minimum. | Alex | **2026-11-07** | He wanted the product and bet on it; the structure failed, not the demand |
| 13 | **Reconcile the unit mix** in the 23,500 MXN month — crowns vs guards vs models vs smile design. | Alex | **2026-11-03** | We don't know which product actually earns; guards look like the best margin we have |
| 14 | ~~**Get BEGO's written answer on the TriniQ "Crown And Bridge, Temporary, Resin" FDA product code.**~~ **Resolved 2026-10-27** by reading K233596 directly: EBF is primary, EBG is secondary because TriniQ is *also* indicated for temporaries. No FDA blocker. **Replaced by:** get BEGO's written confirmation of the **maximum bridge span and pontic count** (their literature says 3 units; the IFU says only "bridge restorations"), and check COFEPRIS registration for Mexico. | Alex | **2026-11-05** | The span limit is what we show a dentist who asks; COFEPRIS is our market, FDA isn't |
| 15 | ~~**Make Rodin Sculpture 2.0 the default for posterior permanent crowns.**~~ **Dropped 2026-10-27.** No 510(k) located for Sculpture 2.0, and no permanent *bridge* indication in the category outside TriniQ. **Replaced by:** log the decision to **stay on TriniQ** and the reason (only resin whose IFU names permanent bridges). See `materials.md` revision. | Alex | **2026-11-03** | Our case mix has pontics; every higher-filler candidate is single-unit by indication |
| 16 | **Controlled anterior test with Laura.** ~~Rodin Titan~~ — Titan is a *denture* resin (21 CFR 872.3760), not crown & bridge. **TriniQ is already cleared for permanent veneers and anterior**, so run the test on TriniQ: same material, same protocol, several units, find the failing step. | Alex + Laura | **2026-11-12** | Decides whether a whole product line reopens. Anterior is where margin and reputation both live |
| 17 | **Standardize one adhesive/cement protocol and write it down.** Both published 2-year studies on printed definitive crowns failed at the bond and the margin, not in the bulk material. Add cement as a logged field in the longevity log. | Alex | **2026-11-05** | Attacks the actual published failure mode, costs nothing, and is a process lever we own |
| 18 | **Flag `strategy.md` §5 and §8 for revision.** Both rest on "nobody in the category has clinical survival data." Two 2-year prospective studies now exist (93% survival n=30; ≥99.5% A/B scores n=33). The longevity log is still an asset, but the uniqueness claim has to get more modest. | Alex | **2026-11-03** | We'd be making a claim to dentists that a doctor with a literature habit can falsify |

---

## Rules

- Every item has an owner and a date. An undated item is not a plan.
- Items move out of here into `company/momentum.md` one at a time, chosen by the owner.
- Done items get struck through with the date, not deleted.
