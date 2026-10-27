---
description: Briefing — what changed since the last brief, and the re-ranked list of what to work on next
---

Run a briefing as the `cofounder` agent. $ARGUMENTS

This runs every morning, and again any time during the day after work got done or new
information came in. Its one job: **take everything that changed, and recompute what
to work on next.** It does not set commitments (that's `/standup`) and it does not
make decisions (that's `/decide`).

Readable in sixty seconds. If it isn't, cut it.

## 0. Gates — before anything else

- `company/strategy.md` unfilled or past its review date → say so first.
- No standup in `company/momentum.md` in the last three days → that is the first line
  of the brief, above everything else.

## 1. Take in what Alex just gave you

If `$ARGUMENTS` or the conversation contains updates, sort each one into exactly one of:

| It's a… | Do this |
|---|---|
| **Done claim** ("sent the X-ray lab email", "furnace decided") | Mark it done in `company/open-items.md` — struck through, dated, with the source ("Alex, brief 2026-10-28 14:30"). Not done unless Alex says done. "Mostly" is not done. |
| **Customer conversation** | File it in `company/customers/` per `/call` rules. Their words verbatim, untidied. If the raw material isn't here, ask for it — don't reconstruct quotes from a summary. |
| **Decision made or needed** | Don't write it to `decisions/`. List it under *Needs a decision* with the command to run: `/decide <one line>`. |
| **New work** | Add to `company/open-items.md` with one owner and one date. If either is missing, ask — all missing owners/dates in **one** question, not one at a time. |
| **New fact** (a price, a number, a name) | Write it where it belongs (`materials.md`, a `persons/` file, the relevant customer file) and say where. |

No input → skip to step 2. That's the normal morning run.

## 2. Find what changed since the last brief

- The last brief is the newest file in `company/briefings/`. Its timestamp is the
  cutoff. No previous brief → use the last 48 hours.
- Run `git log --since="<cutoff>" --name-status` and `git status --porcelain`.
  Uncommitted changes count — notes often land before they're committed.
- Read every changed file under `company/` and `playbooks/`. New customer files and
  new decisions first; they're the ones most likely to change the ranking.

## 3. Reconcile `company/open-items.md`

- **Done** items: strike through with the date. Only with evidence (step 1, or a file
  that shows it). If you think something is done but can't show it, list it as
  *unconfirmed* and ask.
- **Overdue** items: flag with days overdue. Never move a date silently. A new date
  gets written next to the old one: `~~2026-10-29~~ 2026-11-01 — moved because <reason>`.
  Moved twice → say so in the brief; that's a commitment problem, not a calendar one.
- **Changed by new information**: if a customer file or decision makes an item
  obsolete, bigger, or more urgent, update it and cite the file.
- **New**: add with owner, date, and a one-line *why it matters*.

## 4. Recompute what's next

Rank the open items. Apply these in order and stop at the first that separates them:

1. **What breaks if it slips today.** Existing revenue at risk (Omnidental is 100% of
   it), money being lost every day, a deadline someone outside the company set.
2. **What moves the one goal** — clinic #2 at arm's length, then the 12 by 2027-04-27.
   Be explicit about the chain: "this → that → a signed clinic." If you can't draw the
   chain, it doesn't rank here.
3. **What unblocks someone else.** Team output is the binding constraint; an hour of
   Alex that frees a day of Laura or Claudia beats an hour of Alex's own work.
4. **Everything else**, by date.

Pick **three**. Not five. For each: why now, what "done" looks like in a form someone
else can verify in ten seconds, and a time today it should be done by.

Then name the one thing Alex will be tempted to do instead — usually engineering,
usually something that feels productive and doesn't move a clinic.

## 5. Write it

Save to `company/briefings/YYYY-MM-DD-HHMM.md` (create the folder if needed) and show
it. Same content in both places:

```
# Brief — <YYYY-MM-DD HH:MM>  ·  since <cutoff>

**Goal:** <n>/12 active clinics · clinic #2: <status> · <weeks> weeks left
**Ritual:** last standup <date> · next due <date>   ← or the warning, if lapsed

## What changed
- ✅ <done item> — <source>
- ➕ <new item> — <owner>, <date>
- 📝 <what we learned> — <file>
(Nothing changed → say "Nothing new since <cutoff>." That is itself information.)

## Overdue
- #<n> <item> — <owner> — <k> days late

## Next, in order
1. **<item>** — <why now, one line> — done = <verifiable outcome> — by <time>
2. …
3. …

## Waiting on others
- <who> owes <what> since <date> — chase by <time>

## Needs a decision
- `/decide <one line>` — <why it can't wait>

## Don't
<the tempting thing>

## For the next standup
<the one item from this list each person could pick as their 48h commitment — a
suggestion, not an assignment>
```

Leave out any section that's empty, except *What changed* and *Next*.

## Rules

- **Never invent evidence.** A number, quote, or status not in the files or said by
  Alex in this conversation is marked as an estimate or left out.
- **Never edit `decisions/` or `momentum.md`.** Those have their own rituals.
- **One owner, one date, every line.** No "we."
- **Questions only if the answer changes the ranking.** Ask them at the end, all at
  once, and give the brief anyway with your best assumption stated.
