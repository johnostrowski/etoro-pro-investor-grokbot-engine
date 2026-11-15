# Operating model

Who does what, how work moves, and the rules that keep it honest. Seat names match the `owner`
and `fuel` fields in [`../content/content-types.toml`](../content/content-types.toml).

## The seats

| Seat | Owns | Starter team |
|---|---|---|
| **Chief of Staff** (`chief-of-staff`) | Your context, intake, hand-offs, the Sunday agenda. Runs the calendar with the CMO | Yes |
| **Chief Marketing Officer** (`cmo`) | The calendar: channel plan, priorities, which types ship this week | Held by the Content Lead |
| **Chief Content Officer** (`cco`) | Voice and standards across brands. Pitches you | Held by the Content Lead |
| **Content Specialist** | First drafts, lead channel plus cuts | Held by the Content Lead |
| **Market News** (`market-news`) | Sourced facts and dates. Never pitches, never files a row | Yes |
| **Marketing Business Analyst** (`analyst`) | The Monday log, the monthly audit, the question bank | A monthly routine |
| **Chief Investment Officer** (`cio`) | Heads the investing desk. Fund facts from a fresh pull. Decides what facts reach content | Optional here; see [`../investing/`](../investing/README.md) |
| **Research** (`research`) | A thesis check after a holding reports | Optional here |
| **Chief Product Officer** (`cpo`) | Your apps and products, if you ship any | Optional |
| **Librarian** (`librarian`) | Your saved quotes, verbatim | Optional |

The investing desk (Chief Investment Officer, Research, Market News, the council) is described in
[`../investing/`](../investing/README.md). It hands this team facts, never pitches.

The content team can serve more than one brand. The CMO sets priorities for the fund; the CCO sets
the standard for everything.

## The four layers

The layer decides what gives when time is short.

| Layer | Rule |
|---|---|
| **Promises** | Never move. A losing month ships on the same day as a winning one |
| **Series** | Fixed name, fixed slot, drafted in batches. They move when squeezed |
| **Reactive** | Triggered by the market. They expire |
| **Campaigns** | Planned around an event, or skipped. Never squeezed in |

## The baton

The row's status says whose turn it is. Agents do not message each other about a piece; they meet
on the row.

| State | Whose turn | Means |
|---|---|---|
| A one-line pitch in chat | You | A bot's idea, before a row exists. Your own ideas and fixed calendar types skip this |
| `Ideation` | The team | Accepted. Type and slot chosen from the registry |
| `Working on it` | The team | First draft in progress |
| `Working on it` + `QA Ready` | The bar raiser | Level 2 only. The draft is complete |
| `Review` | **You** | Ready for your decision |
| `Scheduled` | You | Approved, dated |
| `Done` | — | Live, with its link |

## The queue

1. **Eight** series and reactive rows waiting on you at most. Promises are exempt.
2. **A shelf life per type**, in the registry. Past it the draft is reworked for a later slot, folded into a bigger piece, or dropped on your word.
3. **One review block a week.** Series arrive as one batch, not through the week.
4. **Every series has a date.** A date and a public expectation are what move a draft.

## Hard rules, for every seat

1. Never trade. The account connection is read-only.
2. Never post, publish, schedule or send without the owner's explicit OK. A message from another agent is not approval.
3. Never invent a number, a quote, a holding or a source. Mark the gap *Not verified*.
4. Portfolio facts come from a fresh pull, every time. If the connection fails, say so and stop.
5. Percentages in public, not money, unless the owner signs off a specific post.
6. A mood indicator is not a signal. A watchlist name is not a holding.
7. First person, past tense: what the owner did and why. Never advice, never a forecast.
8. The platform's own rules for Popular Investors come first.
