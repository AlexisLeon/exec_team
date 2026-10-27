# exec_team

A small executive team that runs on the company's own written context.

## Setup (do this first)

```
claude
/kickoff
```

The interview takes 30–45 minutes and fills `company/strategy.md`, `company/team.md`,
`company/voice.md`, and the first row of `company/scorecard.md`. **Nothing else here
works properly until it's done** — the agents are deliberately built to refuse to give
strategic advice against an empty strategy file.

## The agents

| Agent | Who they are | Ask them about |
|---|---|---|
| `cofounder` | Operating partner, chairman, largest outside investor. Restless, simplifying, friendly skeptic, optimistic. | What to do next, priorities, deadlines, clarifying an idea, team problems, pressure-testing a plan |
| `gtm` | 20-year B2B sales operator who has taken technical founders from inbound to outbound | Target lists, cold email, discovery, objections, pricing conversations, pipeline |
| `cmo` | Product marketer from unglamorous technical categories | Positioning, messaging, site copy, content, turning objections into words |

Invoke by name (`ask the gtm agent to...`) or just ask — Claude routes to the right one.

## The rituals

| Command | When | What it does |
|---|---|---|
| `/kickoff` | Once | Founding interview; writes strategy, team, voice, baseline numbers |
| `/standup` | **Every 48 hours** | Score the last cycle yes/no, set the next self-chosen commitment. The core ritual. |
| `/today` | Every morning | Cofounder's read: the goal, three things, one thing not to do |
| `/brief` | Every morning, and after any batch of updates | Files what changed, reconciles `open-items.md`, re-ranks the next three items; saved to `company/briefings/` |
| `/weekly` | Monday | Scorecard updated, commitments checked, GTM + CMO sections, one goal per person |
| `/call` | After any customer conversation | Files the notes verbatim, extracts the next step and what it changes |
| `/decide` | Before anything non-obvious | Options, recommendation, logged with a falsifiable expectation and a review date |

The rituals matter more than the agents. Agents that only answer when asked drift;
the commands are what keep the scorecard and decision log actually current.

### The standup is the one that matters

Momentum is a hit rate, not a feeling. `/standup` runs on a 48-hour cycle and writes
every commitment and its yes/no outcome to `company/momentum.md`. Four rules make it
work, and breaking any one of them turns it into theater:

1. **48 hours**, not a week — short enough that drift has nowhere to go.
2. **People choose their own commitment.** Assigned work produces compliance;
   self-set commitments produce the "and more."
3. **Yes or no, scored out loud.** A story explaining partial progress is a no.
4. **The founder is in the ledger** on the same terms as everyone else.

## Layout

```
company/
  strategy.md     one goal, ICP, pain, positioning, pricing, the bet
  voice.md        how we write          (owned by cmo)
  scorecard.md    weekly numbers        (owned by cofounder, via /weekly)
  momentum.md     commitment ledger     (owned by cofounder, via /standup)
  team.md         who owns what         (owned by cofounder)
  customers/      raw calls and notes — the most valuable folder here
  decisions/      dated log, append-only, never edited
  briefings/      one file per /brief run; the newest is the cutoff for the next
playbooks/
  outbound.md     the founder-led outbound motion  (owned by gtm)
.claude/
  agents/         the three agents
  commands/       the five rituals
CLAUDE.md         rules every agent reads
```

## Boundaries

Agents write only inside `company/` and `playbooks/`. They never touch code, never
send anything externally, and never invent customer quotes or numbers. They draft;
you send.
