# Pro Investor engine

A one-person fund, run by a small team of AI agents, with you as the only person who decides.
Two sides: **investing**, the desk that researches and briefs you, and **marketing**, the team
that turns what actually happened into what you publish.

A community kit by a Popular Investor, built and run on a real account first. Not an official eToro
product, and not investment advice.

## The idea

At the Pro Investor Summit 2026 the closing session described a one-person fund: agents do the
research, the debate, the risk checks and the review, and one step never runs without you. This
engine builds that fund in two halves that share one loop.

| The loop | Investing side | Marketing side | Runs without you? |
|---|---|---|---|
| Research | The morning brief, from your account, your newsletters and primary sources | The facts the desk hands over, your saved quotes | Yes |
| Council | Bull, Bear, Risk Officer, Macro Desk, Chair | A pitch, then a first draft | Yes |
| Risk | Your rulebook | The rules check, the queue cap, your hours budget | Yes |
| **You** | **You decide. You place the order** | **You approve. You post by hand** | **Never** |
| Review | The weekly performance page, the decision log | The Monday log, the monthly audit | Yes |

Start with whichever side you need first. They connect through one rule: the desk hands the
content team **facts, never pitches**.

| Side | Start here |
|---|---|
| **Investing** | [`investing/README.md`](investing/README.md) |
| **Marketing** | [`SETUP.md`](SETUP.md) |

## Two levels

| | Level 1 · first level of execution | Level 2 · the bar raiser |
|---|---|---|
| What | A Grok bot team runs the calendar and writes first drafts | A second model, Claude, checks every draft before you see it |
| For | Getting started this week | When drafts are flowing and quality is the limit |
| Start with | [`SETUP.md`](SETUP.md) | [`system/bar-raiser.md`](system/bar-raiser.md) |

Do level 1 first. Level 2 adds nothing until there are drafts to raise.

## Three sizes

For the marketing side, pick by the hours you will really give it. Details in [`content/tiers.md`](content/tiers.md).

| Tier | Your hours a week | What ships |
|---|---|---|
| **Starter** | about 2, cap 3 | A monthly report, a mid-month update, a weekly quote, a weekly take, one reply session |
| **Core** | about 5 | Adds a weekly clip reaction, a report video, questions, anniversaries, earnings checks |
| **Full** | about 7, cap 8 | Adds a long form every two weeks, video episodes, a third reply session, event campaigns |

## What is in here

| Path | What it is |
|---|---|
| [`investing/`](investing/) | **The investing side**: the loop, the desk's sources and clock, the council, your rulebook and off switch |
| [`SETUP.md`](SETUP.md) | The marketing side, level 1, step by step |
| [`content/content-types.toml`](content/content-types.toml) | **The registry**: every content type with its slot, channels, tier, minutes and owner. The single source for what ships and when |
| [`content/tiers.md`](content/tiers.md) | Hours and types by tier. Generated from the registry |
| [`content/calendar.md`](content/calendar.md) | The week and the month |
| [`system/operating-model.md`](system/operating-model.md) | Who does what, the hand-offs, the queue rules |
| [`system/bar-raiser.md`](system/bar-raiser.md) | Level 2 |
| [`bots/`](bots/) | The setup prompt and a role card for each seat, on both sides |
| `tools/content_strategy/build.py` | Sums the hours after you edit the registry. Python 3.11, nothing to install |

## The rules, before anything else

1. **Agents propose. You decide.** Nothing is posted, scheduled or sent without your explicit OK.
2. **No agent trades.** Connect your account read-only. This engine has no execution agent.
3. **Nothing invented.** No made-up numbers, quotes, holdings or sources. A gap is marked *Not verified*.
4. **Fresh numbers.** Every performance figure is pulled on the day and checked again on the day you post.
5. **Percentages, not money**, unless you decide otherwise for a specific post.
6. **A losing month ships on the same day as a winning one.**
7. **Know your platform's rules** for Popular Investors: disclaimers, calls to action, what you may say. This kit does not replace them.

## Status

Version 0.2: the investing side added. Generated from a private working system; changes are made there first and exported
here. No licence has been chosen yet.
