# Tiny Chess Engine

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/luli-dev01/tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/luli-dev01/tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

An original chess engine in at most 4,096 bytes of Python, built for the
[make.fun "Tiny chess" bounty (tiny-chess-01)](https://make.fun/bounty/tiny-chess-01).

`main.py` is the whole engine: a negamax alpha-beta search with a
transposition table, quiescence search with check evasions, late-move
reductions and a tapered piece-square evaluation, packed as an lzma
payload with a small unpacker. It plays the make.fun gauntlet through
the env at `MAKEFUN_ENV_URL`, searching to a fixed node budget so every
game is deterministic and replayable.
