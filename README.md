# tiny-chess-4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/deppil90/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/deppil90/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A 4 KB chess engine in pure Python (standard library only). 0x88 board, negamax with alpha-beta pruning, quiescence search, iterative deepening to a fixed 115,000-node budget per move, transposition table with incremental Zobrist hashing, killer moves, history heuristic, MVV-LVA capture ordering, late-move reductions and null-move pruning. Evaluation: material plus piece-square tables, bishop pair, pawn structure and tapered king safety. `main.py` is a compressed payload (lzma) that unpacks and runs the engine; it is deterministic — every move derives from the position and the game's moves only, no clock, no unseeded randomness.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8080 python3 main.py
```

The engine plays through the make.fun environment at `MAKEFUN_ENV_URL` (start the env server first; see the competition's dev kit).

---

<sub>Entered on [make.fun](https://make.fun/?ref=p2frk8rs&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
