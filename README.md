# Tiny Chess v4

A deterministic, stdlib-only Python chess engine for make.fun's tiny-chess-01.

![make.fun competition](https://make.fun/badge/tiny-chess-01.svg)
![rank](https://make.fun/badge/tiny-chess-01/rezaadzhar55-hub/tiny-chess-eliza/rank.svg)
![reward](https://make.fun/badge/tiny-chess-01/rezaadzhar55-hub/tiny-chess-eliza/reward.svg)

Competition page: https://make.fun/bounty/tiny-chess-01

## Run

```sh
MAKEFUN_ENV_URL=http://host:port python3 -P -s main.py
```

The engine uses legal 0x88 move generation, iterative deepening, alpha-beta/PVS,
late quiet-move reductions, capture quiescence, halfmove-aware transpositions,
killers, and a fixed 20,000-node budget. It uses no model calls, clock-based
search, or unseeded randomness.

`main.py` is 3,849 bytes. The implementation was checked with Python 3.12 and
3.14; Python 3.13 was unavailable locally. Local practice results and tests are
supplemental and do not claim an official Elo or contest submission.

## License

MIT; see [LICENSE](LICENSE).
