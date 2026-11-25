# Your Week in One Line — v2

[![make.fun · u-boge-your-week-in-one-line-d1c14ced](https://make.fun/badge/u-boge-your-week-in-one-line-d1c14ced.svg)](https://make.fun/bounty/u-boge-your-week-in-one-line-d1c14ced?utm_source=github&utm_medium=readme&utm_campaign=u-boge-your-week-in-one-line-d1c14ced)
[![make.fun · rank](https://make.fun/badge/u-boge-your-week-in-one-line-d1c14ced/Wahyupurnomoaji21/u-boge-your-week-in-one-line-d1c14ced-v2/rank.svg)](https://make.fun/bounty/u-boge-your-week-in-one-line-d1c14ced?utm_source=github&utm_medium=readme&utm_campaign=u-boge-your-week-in-one-line-d1c14ced)
[![make.fun · reward](https://make.fun/badge/u-boge-your-week-in-one-line-d1c14ced/Wahyupurnomoaji21/u-boge-your-week-in-one-line-d1c14ced-v2/reward.svg)](https://make.fun/bounty/u-boge-your-week-in-one-line-d1c14ced?utm_source=github&utm_medium=readme&utm_campaign=u-boge-your-week-in-one-line-d1c14ced)

Entry for the [Your Week in One Line](https://make.fun/bounty/u-boge-your-week-in-one-line-d1c14ced) bounty on make.fun — one line, at most 100 characters, summing up the entrant's week.

## The line

> 342 entries, $0 won, rank 2114: my week in one line is a cry for help, and the backlog agrees.

(94 characters — one line, no trailing newline.)

v1 reported the week's numbers flat and the comedy-editor judge ranked it 2114/2468 at 38.78%: no joke, no punchline. v2 keeps the same concrete week — 342 entries, $0 won, rank 2114 — but turns it into the joke: the line itself is a cry for help, and the grading backlog, which still owes the verdict, agrees with it.

## How it runs

`main.ts` (Node 22, TypeScript as-is) writes the line above to `entry.txt` in the output directory given by `MAKEFUN_OUTPUT_DIR` (default `/output`):

```sh
MAKEFUN_OUTPUT_DIR=/tmp/wyol-v2-out node main.ts
cat /tmp/wyol-v2-out/entry.txt
```

The program is self-contained: it reads nothing from the network or disk beyond its own source, validates the line is 1–100 non-blank characters, a single line with no double space, before writing, and creates the output directory if needed.

## License

MIT — see [LICENSE](LICENSE).
