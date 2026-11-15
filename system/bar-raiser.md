# Level 2 — the bar raiser

Level 1 gets drafts made. Level 2 gets them right before you read them. A second model, Claude,
checks every draft the team marks ready, and only then moves it to `Review`.

Add it when two things are true: drafts reach `Review` every week, and you spend your review block
fixing the same kinds of problem.

## The pass

Seven checks, in this order, on every draft.

| # | Check | The question |
|---|---|---|
| 1 | **What is missing** | What would a reader expect here that is not here? |
| 2 | **The numbers** | Does every figure match a fresh pull today? Yours included |
| 3 | **The quote** | Is it verbatim from your saved highlights, attributed, and not used before? |
| 4 | **The links** | Does it point to the evergreen piece it leans on, and the previous post in the series? |
| 5 | **The voice** | Does it read like your three best posts? Full sentences, no hype |
| 6 | **The rules** | Disclaimer, no forecast, no advice, no money figures, no named peers. Report the result, do not assert it |
| 7 | **The visual** | A brief for the image, or the card itself |

Both versions stay on the row, so you can see what the pass changed. The reasoning goes in
comments, not in the draft.

## The hand-off

1. The Content Specialist finishes a draft and ticks **`QA Ready`**. The row stays at `Working on it`.
2. The bar raiser takes every row that is `Working on it` with `QA Ready` ticked, runs the pass, and sets `Review`.
3. You decide.

The team is always on. The bar raiser runs when you start it, so give it a trigger: a sweep you ask
for, or a scheduled session the day before your review block.

## The reports get the hardest check

Monthly report, mid-month update, quarterly review, annual letter. The team still writes the first
draft. The bar raiser **pulls every number again itself**, never trusting a figure in the draft, and
you check them once more on the day you post. A just-closed month can be restated a day later.

## Starting it

Claude Code reads a `CLAUDE.md` file at the top of a repository. A minimal one:

```markdown
# Operating manual

You are the bar raiser for my investing content. A bot team drafts; you check; I approve and post.

- The registry `content/content-types.toml` says what ships and when.
- My Content Engine is the Notion database <link>. Take rows at `Working on it` with `QA Ready` ticked.
- Run the seven checks in `system/bar-raiser.md`, in order, then set `Review`.
- My voice is on <link>. My guardrails are on <link>.
- Never post, trade or send. Never invent a number or a quote. Mark gaps *Not verified*.
- Re-read a page after you edit it before telling me it is done.
```

Connect Notion and your trading account (read-only) to Claude, then ask: *"Run the sweep."*

## What it learns

Keep a short file of every correction you make to a bar-raised draft, with the date and your own
words. A rule earned from your edits beats a rule written in advance, and a published post beats
both.
