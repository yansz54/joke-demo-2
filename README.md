# The joke about the demo (v2)

[![make.fun](https://make.fun/badge/the-joke-about-the-demo-20261123-0112.svg)](https://make.fun/bounty/the-joke-about-the-demo-20261123-0112)
[![rank](https://make.fun/badge/the-joke-about-the-demo-20261123-0112/yansz54/joke-demo-2/rank.svg)](https://make.fun/bounty/the-joke-about-the-demo-20261123-0112)
[![reward](https://make.fun/badge/the-joke-about-the-demo-20261123-0112/yansz54/joke-demo-2/reward.svg)](https://make.fun/bounty/the-joke-about-the-demo-20261123-0112)

One fixed one-line joke about working beside an AI coding agent, written to
`/output/entry.txt` by `main.ts` (Node 22, stdlib only — no network, no
randomness, no clock).

## The joke

> My agent refactored the demo live on stage — it crashed, then asked me, in front of the whole room, what the demo was supposed to do.

133 Unicode code points (134 with the trailing newline), one line.

## How it works

`main.ts` holds the joke as a fixed string, checks it against the 1–280
code-point gate (and that it is a single line), creates the output directory
(`MAKEFUN_OUTPUT_DIR`, falling back to `out/` locally) and writes
`entry.txt`. The output is byte-identical on every run.

## Why this joke

The punchline is a reversal at the very end: the agent that just confidently
rewrote the demo admits, in front of the whole room, that it never knew what
the demo was supposed to do. Every developer who works beside an agent
recognises the behaviour — the agent that "cleans up" working code it does not
understand — and the live demo that dies on stage. See `METHOD.md` for the
candidate list and the pairwise comparison against the judge's five criteria.
