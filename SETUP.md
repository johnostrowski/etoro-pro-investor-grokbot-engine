# Setup — level 1

About an hour for the Starter team. You need a Grok account that can run bots, a Notion workspace,
and your trading account connected **read-only**.

## 1. Pick a tier

Open [`content/tiers.md`](content/tiers.md) and choose the row whose hours you can keep every week
for a quarter. Starting on Starter and moving up is better than starting on Full and stopping.

## 2. Create the team

| Tier | Seats |
|---|---|
| Starter | Chief of Staff, Content Lead, Market News |
| Core, Full | Chief of Staff, Chief Marketing Officer, Content Specialist, Market News, Marketing Business Analyst. Add a Chief Investment Officer for fund facts, a Chief Content Officer if you run more than one brand, a Chief Product Officer if you ship apps |

1. Create the Chief of Staff first and give it [`bots/chief-of-staff-setup.md`](bots/chief-of-staff-setup.md).
2. It walks you through the rest. For each seat it uses the card in [`bots/role-cards.md`](bots/role-cards.md).
   If it cannot create a teammate itself, it hands you the card to paste.

On the Starter team the Content Lead holds two seats from the registry, `cmo` and `cco`.

## 3. Build the Content Engine in Notion

One database. One row per piece per channel.

| Property | Type | Values |
|---|---|---|
| `Name` | Title | Starts with the series prefix from the registry |
| `Status` | Select | `Ideation` → `Working on it` → `Review` → `Scheduled` → `Done`, plus `Archived` |
| `Tags` | Multi-select | Your brand, and one pillar: `Educational`, `Performance`, `Engagement`, `Promotional` |
| `Format` | Multi-select | `Thought`, `Video`, `Article`, `Repurpose` |
| `Schedule by` | Date | The slot from the registry |
| `Post link` | URL | Filled when it is live. `Done` without a link is not done |
| `QA Ready` | Checkbox | Level 2 only: the draft is ready for the bar raiser |
| `Notes` | Text | The parent row, the sources, what is *Not verified* |

The lead channel is the parent row. Each cut for another channel is its own row, `Format`
`Repurpose`, with a link back to the parent.

## 4. Write the foundation pages

The Chief of Staff interviews you and saves each page only after you confirm it. No bot drafts
until the first three exist.

| Page | Holds |
|---|---|
| **Audience** | Who you want copying you, where they are on their journey, what scares them |
| **Voice** | Your three best posts per platform, what makes them good, words you never use |
| **Guardrails** | The rules above, plus your platform's and your employer's limits |
| Goals | What you are judged on this half-year |
| Philosophy | How you invest, in your own words, in percentages |

## 5. Give the team the registry

Paste the section of [`content/content-types.toml`](content/content-types.toml) for your tier into
the Chief of Staff, or point it at this repository. Change any slot that does not fit your week,
then run:

```bash
python3 tools/content_strategy/build.py
```

It rewrites `content/tiers.md` and warns if your tier is over its hours cap.

## 6. Run the first week

| Day | You | The team |
|---|---|---|
| Sunday | 45 minutes: approve, edit or drop what is waiting | Has the week's drafts ready in one batch |
| Monday | 10 minutes: read the log | Logs last week's numbers |
| Tuesday | Post the weekly quote | — |
| Any day | Give one idea in chat | Returns a draft pair at `Review` |

## 7. Keep the queue short

- **Eight drafts waiting on you at most.** When the queue is full the team stops drafting series.
- **A pitch before a draft.** For any idea a bot starts, it sends one line first. A pitch costs you ten seconds.
- **Drafts go stale.** Each type has a shelf life in the registry. Past it, the draft is reworked or dropped.

## 8. Measure

Every Monday, one row: originals posted, reply sessions, drafts created and published, followers,
impressions, copiers, hours spent. After a month the team reads it back to you and proposes one
change to the registry.

## Then

When drafts ship every week and you want them better, go to [`system/bar-raiser.md`](system/bar-raiser.md).
