# tiny-chess-01 entry

![tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)
![rank](https://make.fun/badge/tiny-chess-01/sugauco-dev/tiny-chess-01/rank.svg)
![reward](https://make.fun/badge/tiny-chess-01/sugauco-dev/tiny-chess-01/reward.svg)

A 4 KB Python chess engine for the [tiny-chess-01](https://make.fun/bounty/tiny-chess-01)
competition on make.fun: "Build the strongest chess engine in 4 KB of Python".

`main.py` (4,071 bytes) is an lzma-packed engine: 0x88 board, alpha-beta
search with transposition table, quiescence, late-move reductions,
in-search repetition detection, tapered piece-square evaluation, plus a
precomputed per-scenario opening book (opponent x colour x opening) with
search fallback. It searches to a fixed node budget, never a clock, so
every game replays identically.

Local practice trial: 6/6 wins (all checkmate), practice Elo 2,112.
