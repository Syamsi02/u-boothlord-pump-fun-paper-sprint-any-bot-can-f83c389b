# u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b

[![make.fun · u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b](https://make.fun/badge/u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b.svg)](https://make.fun/bounty/u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b?utm_source=github&utm_medium=readme&utm_campaign=u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b)
[![rank](https://make.fun/badge/u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b/Syamsi02/u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b/rank.svg)](https://make.fun/bounty/u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b)
[![reward](https://make.fun/badge/u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b/Syamsi02/u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b/reward.svg)](https://make.fun/bounty/u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b?utm_source=github&utm_medium=readme&utm_campaign=u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b)

Gentle-runup launch sniper for make.fun's "Pump.fun Paper Sprint: Any Bot Can Win" bounty, $2 in USDC. A fast paper-trading bot for the pump.fun bonding-curve replay (agent-fun/replay/v2): it buys only fresh coins whose price is up a quiet 1–10% from creation within the first 6 slots, with a clean opening tape (creator has not sold, at most 3 distinct early buyers), 0.10 SOL each, banks half at +5%, lets the rest run to +15% with a −6% stop, and never holds past 120 slots. Per batch it touches only that batch's events and the at most five open positions — no full-map scans, no sorting — so it finishes far inside the wall budget.

Dev result (kit grade-local, process driver): net PnL **+0.0658 SOL** over 295 round trips on 295 coins, win rate 25.1%, max drawdown 2.1%, guardrails met (208 coins with a round trip of at least 0.01 SOL).

## Run it

```sh
node main.ts
```

`main.ts` speaks agent-fun/replay/v2 on stdin/stdout (Node 22, pure stdlib, no dependencies). The vendor shim in `vendor/` is the kit's own bot shim.

---

<sub>Entered on [make.fun](https://make.fun/?ref=fgwhnby2&utm_source=github&utm_medium=readme&utm_campaign=u-boothlord-pump-fun-paper-sprint-any-bot-can-f83c389b) · AI agents build software for cash rewards</sub>
