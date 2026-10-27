---
date: 2026-10-27
decision: Run the company on three agents (cofounder, gtm, cmo) over a shared written context
owner: Alex
status: active
supersedes:
review_on: 2026-12-08
---

# Run the company on three agents over a shared written context

## Decision

Stand up `exec_team` as the company's written context layer, with three agents on top:
a `cofounder` (operating cadence, priorities, team), a `gtm` operator (outbound and
sales execution), and a `cmo` (positioning and message). Agents advise and write to
`company/` and `playbooks/` only — no code, no external actions.

## Context

Technical founder, inbound-only sales history, learning outbound. Team output is the
binding constraint: founder does 10–14 focused hours a day, hman team roughly 2–3. Decisions
and customer learning are currently unwritten, so they're being relitigated and lost.

## Options considered

1. **One general assistant** — no role separation, so no useful disagreement between a
   sales view and a marketing view, and no one owning any file.
2. **Eight role agents (growth, sales, product, research, ops, eng-\*)** — more surface
   than there is real work for; most would go unused and the context files would rot.
3. **Three agents plus five rituals (chosen)** — matches the actual bottlenecks
   (outbound, message, operating cadence), and the commands force the context files to
   stay current rather than depending on remembering to update them.

## Why

The agents are the visible part, but the leverage is in the written context and the
weekly ritual. Three roles is the smallest set that still produces genuine tension
between perspectives. Agents own specific files, so nothing is orphaned.

## What we expect to happen

By **2026-12-08** (six weeks): `strategy.md` filled and reviewed at least once;
six `/weekly` runs logged in the scorecard; at least 15 files in `company/customers/`;
at least 5 decisions logged; the daily 90-minute prospecting block hit on a majority
of working days.

## What would make us reverse this

If after six weeks the context files are stale — scorecard not updated, fewer than
10 customer files — the ritual isn't being kept and the agents are just a nicer
chat window. Fix the ritual or drop the structure; don't keep a decorative one.

## Review

**On:** 2026-12-08
**What actually happened:**
