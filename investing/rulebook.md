# Your rulebook

Every agent gets the same rules. Write them once, in numbers, and paste them into each seat.
The values below are examples. Set your own, and keep them tighter than your platform's limits for
Popular Investors.

```yaml
account: demo                  # move to real only after weeks of clean runs
agents_may_place_orders: false # this engine keeps it false
max_position_pct: 20           # of the portfolio, any single name
max_sector_pct: 40
max_leverage: 1
stop_loss_required: true       # the session's example. A long-term plan may set false: decide, do not default
target_risk_score: 3           # an addition of this kit, not from the session: flag any break
max_names: 10                  # also this kit's: individual companies, outside your core funds
max_daily_loss_pct: 3          # past this, the desk stops proposing new ideas
max_weekly_drawdown_pct: 10
restricted_names: []           # names you never touch, or must not write about
decision_log: required         # every verdict and every override, written down
stop_word: "STOP"              # on this word, every agent halts
```

## Write these down too

| Question | Why the desk needs it |
|---|---|
| The parts of your book and their target ranges, in percentages | So drift can be flagged |
| What earns a name its place, as four or five filters | So Research checks the same things every time |
| What your plan does not do (leverage, shorts, cash held for timing) | So an exception is named as an exception |
| How you buy and rebalance | So "nothing changed" is a finding, not a gap |
| What would change the plan | So a red quarter is not mistaken for a reason |

Mark anything you have not decided as *To decide*. The desk treats an undecided rule as no rule and
asks you, it does not invent one.

## Your off switch

Know it before any agent can act on anything.

- **The real switch is your API key.** Delete it in your platform's settings and every agent loses
  access at once.
- Make sure you can do that from your phone.
- The stop word halts the agents. The key removes their access. Use the key when in doubt.
