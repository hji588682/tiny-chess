# tiny-chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/hji588682/tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/hji588682/tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

Tiny Lantern is an original chess engine written from scratch in under 4 KB of Python (`main.py`, 3,348 bytes, packed with the kit's own compressor). Inside: negamax alpha-beta search with iterative deepening under a fixed 60,000-node budget (no clock, no randomness — the same position always gets the same move), quiescence search over captures with check evasions, a transposition table with its own Zobrist hashing, late-move reductions, MVV-LVA move ordering, and an evaluation built from material plus hand-written piece-square tables, bishop-pair and passed-pawn terms. It plays the make.fun house gauntlet over HTTP, and in local practice trials against the kit's own scorer it rated 1451 Elo on both practice sets (house anchors run from 855 to 1596).

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8080 python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=htr5vzs0&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
