# Pro Investor content engine

A content system for an investor who posts about their own portfolio: one calendar, one registry of
content types, and a small team of AI agents that runs it. You stay the only person who approves
and posts.

A community kit by a Popular Investor, built and run on a real account first. Not an official eToro
product, and not investment advice.

## The idea

At the Pro Investor Summit 2026 the closing session described a one-person fund: agents do the
research, the debate, the risk checks and the review, and one step never runs without you. If you
built the research agent and the council from that session, **this is the next seat: investor
relations.** It is the letter to your copiers, drafted from what actually happened, approved by you.

The loop is the same one:

| The fund's loop | In this engine | Runs without you? |
|---|---|---|
| Research | Your facts: the portfolio pull, the market tape, your saved quotes | Yes |
| Council | A pitch, then a first draft | Yes |
| Risk | The rules check, the queue cap, your hours budget | Yes |
| **You** | **You approve. You post by hand** | **Never** |
| Review | The Monday log and the monthly audit | Yes |

## Two levels

| | Level 1 · first level of execution | Level 2 · the bar raiser |
|---|---|---|
| What | A Grok bot team runs the calendar and writes first drafts | A second model, Claude, checks every draft before you see it |
| For | Getting started this week | When drafts are flowing and quality is the limit |
| Start with | [`SETUP.md`](SETUP.md) | [`system/bar-raiser.md`](system/bar-raiser.md) |

Do level 1 first. Level 2 adds nothing until there are drafts to raise.

## Three sizes

Pick by the hours you will really give it. Details in [`content/tiers.md`](content/tiers.md).

| Tier | Your hours a week | What ships |
|---|---|---|
| **Starter** | about 2, cap 3 | A monthly report, a mid-month update, a weekly quote, a weekly take, one reply session |
| **Core** | about 5 | Adds a weekly clip reaction, a report video, questions, anniversaries, earnings checks |
| **Full** | about 7, cap 8 | Adds a long form every two weeks, video episodes, a third reply session, event campaigns |

## What is in here

| Path | What it is |
|---|---|
| [`SETUP.md`](SETUP.md) | Level 1, step by step |
| [`content/content-types.toml`](content/content-types.toml) | **The registry**: every content type with its slot, channels, tier, minutes and owner. The single source for what ships and when |
| [`content/tiers.md`](content/tiers.md) | Hours and types by tier. Generated from the registry |
| [`content/calendar.md`](content/calendar.md) | The week and the month |
| [`system/operating-model.md`](system/operating-model.md) | Who does what, the hand-offs, the queue rules |
| [`system/bar-raiser.md`](system/bar-raiser.md) | Level 2 |
| [`bots/`](bots/) | The setup prompt and a role card for each seat |
| `tools/content_strategy/build.py` | Sums the hours after you edit the registry. Python 3.11, nothing to install |

## The rules, before anything else

1. **Agents propose. You decide.** Nothing is posted, scheduled or sent without your explicit OK.
2. **No agent trades.** Connect your account read-only.
3. **Nothing invented.** No made-up numbers, quotes, holdings or sources. A gap is marked *Not verified*.
4. **Fresh numbers.** Every performance figure is pulled on the day and checked again on the day you post.
5. **Percentages, not money**, unless you decide otherwise for a specific post.
6. **A losing month ships on the same day as a winning one.**
7. **Know your platform's rules** for Popular Investors: disclaimers, calls to action, what you may say. This kit does not replace them.

## Status

Version 0.1. Generated from a private working system; changes are made there first and exported
here. No licence has been chosen yet.
