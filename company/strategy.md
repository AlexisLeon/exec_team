# Strategy

**Company:** Digital Dental Lab
**Last updated:** 2026-10-27 (founding interview)
**Next review:** 2026-11-24

Written from the founding interview. Anything marked **?** is unknown and needs an
answer — a visible `?` is information, a blank is a lie.

---

## 1. What we do

> We're the one lab a dental clinic sends all its work to — crowns, prostheses,
> aligners — back in five days instead of six weeks, with a status you never have
> to chase.

Dentistry in Latin America is under-tooled and under-served. Corporates sold expensive,
poor-quality digital equipment to dentists who had no way to evaluate it. We're an
engineering-led lab doing the operations work so dentists can do clinical work.

**The long game (McKelvey's innovation stack).** Each layer is copyable alone; the
stack isn't. **Layer 1: lab** — quality and consistency across all materials, so a
clinic stops juggling specialist labs. **Layer 2: scanners + order visibility** —
hardware placed against minimum volume, and software that shows case status and
reaches a technician, so clinics stop chasing us. **Layer 3: practice management** —
the Square-for-dentists layer; they grow, we grow.

**We are at layer 1, and not all of it.** Layers 2 and 3 are roadmap, not product.

## 2. The one goal

**12 active clinics by 2027-04-27** (26 weeks; the 10%/week midpoint of the
7–13% band). Active = **sends the minimum monthly consumption**, currently 18,000 MXN.

| | |
|---|---|
| Today | **1** — Omnidental, which Alex part-owns, with the ordering dentist exiting |
| Arm's-length clinics | **0** |
| Required | 11 more in 6 months ≈ 2/month |

**The milestone that matters is clinic two.** Two clinics at the minimum is 36,000 MXN
against ~29,900 of fixed cost — the month the company stops losing money. Twelve is
the destination; clinic two is where the company starts existing.

## 3. ICP

**Private practice, owner-dentist, high-ticket case mix.**

- **Buyer and champion are the same person** — the owner-dentist signs *and* feels the
  six-week wait. The cleanest sale available.
- **Case mix, not chair count, is the variable.** Rosario's single chair comfortably
  produced 15,000/month for Futura; the churned clinic couldn't reach 18,000 at all.
  One chair doing crowns, bridges and aligners beats three doing cleanings.
- **Qualifying question:** *"What share of your cases are crowns, bridges, aligners?"*
  It predicts consumption without asking about money.
- **Shape of the practice:** open 6 days (8h Mon–Fri, half Saturday), ~8 patients per
  chair per day, high-ticket work, patients not price-led.
- **Trigger events:** a bad lab experience (late case, misfit, a case marked delivered
  that wasn't); opening or expanding; going digital; being sold a scanner they can't use.

**Disqualify:**
- **DSOs, for now.** Managers sign and don't feel the delay. The Stripe-style
  bottom-up wedge — getting individual doctors to demand us — is a later motion.
- General-dentistry-led practices, price-led patient bases, high cancellation rates.
- Anything below the consumption line. We have already paid for this once.

**Channel:** the X-ray / imaging lab (see `customers/`) owns relationships with
orthodontists and is a faster route than one-at-a-time outbound. Referral share beats
ads to doctors whose relationship someone else owns. **Channels are not counted as
clinics.**

## 4. The pain

From `customers/` — real, not theorized:

- **Delays.** Six weeks for simple zirconia (Rosario, at Futura).
- **Dishonesty about status.** Futura marked orders delivered that weren't; cases went
  to the wrong address.
- **Fit problems and remakes.**
- **Bad equipment sold into the digitalization wave** — scanners and computers that
  break and don't scan properly.
- **Fragmentation** — juggling several specialist labs for different components.

**What it costs them:** rescheduled patients, lost chair time, their own credibility
with the patient.

**What they do instead of us:** incumbent labs like Futura, or several specialist labs
at once. The competitor isn't better technology — it's an unreliable status quo.

## 5. Positioning

- **Category:** full-service digital dental lab.
- **We are the lab that tells you the truth about your case and gets it back in days.**
- **The thing only we can say (for now):** permanent 3D-printed restorations at roughly
  half the cost of zirconia, with the margin going to the dentist — backed by our own
  logged clinical placements. Nobody in this category has clinical survival data, so
  the longevity log is a real asset. See `materials.md`.
- **Communication is the moat we're underclaiming.** The bar in this market is *tell
  the truth about where the case is.* Incumbents fail it. It costs us nothing.

## 6. Pricing

| Product | Price (MXN) | COGS | Gross margin | % |
|---|---|---|---|---|
| Clear aligner case | ~14,000 | ? | ? | ? |
| Printed guard | 1,250 | 100 | **1,150** | 92% |
| Zirconia unit | 1,800 | 800 | **1,000** | 56% |
| Printed crown | 800 | 130 | **670** | 84% |
| E.max unit | 1,600 | ? (no reliable partner) | ? | ? |

**Fixed monthly:** furnace 12,500 + lease 12,600 (scanner ~10,100 + vacuum ~2,500)
= **25,100**. Breakeven ≈ **29,900 MXN/month**.

**Minimum consumption: 18,000 MXN** — *below breakeven, and being repriced*
(open item #5). One aligner case ≈ 14,000, so the minimum is roughly one aligner plus
a few guards — not 23 crowns.

**Product ladder:** aligners for volume · guards for margin and easy first orders
(92%, no fit or aesthetic risk — the best first order from a dentist who doesn't know
us) · crowns as base load.

**Scanners:** 3Shape TRIOS ~200k MXN, at scale 48–60 months / 30% residual ≈ 4–4.5k/mo.
Runyes ≈ 3,500/mo including laptop. The current 13k/mo 3Shape was a deliberate
short-term lease for a roaming scanner and **does not represent scale economics.**
The choice at scale is about **scan quality, not price** — a bad scan means a bad fit,
which is the failure we sell against. Needs a measured comparison.

## 7. Distribution

- **Warm intros — working, and the priority.** Rosario's network, practice events.
- **Channel partners** — the X-ray lab, with a referral reward.
- **Founder-led outbound** — list exists in Attio (INEGI, COFEPRIS, Google Maps),
  not yet filtered to names. See `playbooks/outbound.md`.
- **Inbound** — has worked historically, not systematized.
- **Explicitly not doing:** ads to doctors reached through a partner's relationship;
  DSO sales; hiring an SDR before 20 founder-led conversations.

## 8. The bet

**Two assumptions, either of which kills the plan.**

1. **Dentists will consolidate onto one lab for reliability and honest communication.**
   Testable within weeks — it's the whole sales pitch.
2. **Permanent 3D-printed restorations hold up clinically over 3+ years.**
   **This is the one that can't be fixed by working harder.**

**Current evidence for #2:** one 3-unit posterior bridge at 1 year, no failure. The
whole category is cleared on bench testing, not clinical trials — nobody has survival
data (`materials.md`). The upside: our longevity log becomes the only clinical evidence
base in the market. The downside: if these fail at 24–36 months, it's a reputation
collapse in a market where everyone knows everyone.

**Third risk, financial not technical:** the model places leased hardware against
promised volume. It has already failed once, at n=2, with Alex covering the gap from
his own pocket. Twelve clinics is twelve scanners. **Working capital, not demand, is
the most likely cause of death.**

**How we'd know we're wrong:** failures in the longevity log; clinics signing but not
reaching the minimum; loss rate staying above 15% of potential revenue.

## 9. Known constraints

- **Zero arm's-length customers.** All revenue and all evidence come from a clinic
  Alex part-owns, with the ordering dentist leaving.
- **Loss rate ~37% of potential revenue** in the best month on record (6 veneers +
  a 9,000 prosthesis lost to an unchecked outsourced design). Tripwire proposed at 15%.
- **Design is outsourced and unguarded.** Milling is outsourced. We control printing.
- **Anterior aesthetics is where the product fails** — possibly process, not material.
- **Alex is not a technician** and learning ceramics is a poor use of his hours.
  `persons/laura_garcia.md` is the capability, and likely a better investment than a mill.
