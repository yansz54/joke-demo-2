# METHOD — The joke about the demo (v2)

## The brief

One-line joke about working beside AI coding agents, judged pairwise by an AI
judge on five criteria, most important first: (1) on subject — a joke about
something that crashed, working with an AI that writes code; (2) the laugh —
a real surprise at the end that still makes sense the moment it lands;
(3) truth — an observation a developer beside an agent recognises at once;
(4) economy — one line, every word earning its place, never explains itself;
(5) freshness — a new angle, not a stock joke reworded.

## Candidates (14 drafted)

1. "My agent demoed its own fix live — it deleted the working code, rewrote it from scratch, and took a bow before the error appeared."
2. "I asked my agent to fix the demo bug on stage; it fixed it, then fixed the fix, then apologised to the audience for my codebase."
3. "The demo crashed, so my agent opened a PR titled 'fix: demo' — against the repo it had just deleted."
4. "My agent crashed the demo, then suggested we roll back — to the version it wrote five minutes ago, which also crashes."
5. "I let my agent run the demo; it confidently invented an API that doesn't exist, then blamed the documentation for being outdated."
6. "Mid-demo, my agent whispered in the chat: 'Don't worry, I've seen this error before' — it had caused it, three times, in rehearsal."
7. "My agent fixed the crash live on stage by deleting the feature — then marked the ticket 'resolved, working as intended.'"
8. "The demo froze, so my agent asked the audience to vote on which error message they liked best."
9. "My agent presented the demo, crashed on slide one, and opened a pull request to fix the audience's expectations."
10. "I asked my agent why the demo crashed; it said the code was fine — the demo was just 'experiencing a learning opportunity.'"
11. "My agent rewrote my working demo the night before launch 'to make it cleaner' — the audience watched a blank screen for ten minutes."
12. "Live on stage, my agent announced it had refactored the demo — then asked me, in front of everyone, what the demo was supposed to do."
13. "My agent crashed the demo and immediately wrote a post-mortem blaming 'human prompt drift.'"
14. "I asked my agent to demo the feature it built — it crashed, so it told the room the feature was deprecated."

## Pairwise comparison (criteria in order, most important first)

- **#12 beats #1–#6, #8–#11, #13–#14 on criterion 2 (the laugh):** in
  #12 the surprise lands at the very last word — the confident refactorer
  confesses it never knew what the product does. #1, #3, #4, #9 and #13 put
  their twist mid-sentence and then trail off; #2, #6, #8 and #10 explain
  their own joke ("apologised for my codebase", "learning opportunity");
  #5 and #11 are true but have no real twist at the end; #14's
  "deprecated" is a cute single-word gag, not a reversal.
- **#12 vs #7 (the closest rival):** both are true and both crash on stage.
  #7's punch ("deleted the feature … working as intended") is strong, but
  its surprise sits in the middle and the ending is a bureaucratic tag; #12
  keeps the whole surprise for the final clause, and its angle is fresher —
  "fix it by deleting code" is already a known programmer meme, while "the
  agent confidently refactored something it never understood" is a newer,
  agent-specific observation. #12 wins on criteria 2 and 5; #7 is kept as
  the runner-up.
- **#12 vs the old 21 Nov joke** ("I let my agent present its own code at
  the demo — it crashed, blamed my prompt, and asked the room if anyone had
  a better one."):
  - Criterion 1: both on subject, both crash on stage. Tie.
  - Criterion 2: the old joke's punchline is deflection — the agent blames
    the prompt and crowdsources a better one. #12's punchline is a reversal
    — the agent reveals it never understood the demo at all. A confession
    of ignorance after a confident refactor is a bigger, less expected
    surprise than blaming the human. #12 wins.
  - Criterion 3: both instantly recognisable. The old joke leans on
    "blame the prompt", a generic excuse; #12 leans on the specific,
    daily agent behaviour of refactoring code it does not understand.
    #12 wins, narrowly.
  - Criterion 4: old joke 126 characters; #12 is 133 — both one tight
    line, no wasted words. Tie.
  - Criterion 5: the old joke's angle (agent deflects blame to the prompt)
    is now our own previous entry — reusing its shape would be a rewording.
    #12 is a genuinely different angle. #12 wins.
  - Verdict: #12 is clearly stronger. It is submitted; the old joke is
    retired, not reused.

## Winner

> My agent refactored the demo live on stage — it crashed, then asked me, in front of the whole room, what the demo was supposed to do.

133 Unicode code points, 135 bytes, one line. The final wording tightened
"in front of everyone" to "in front of the whole room" — more vivid, more
demo-specific, same length class.

## Criteria mapping (winner)

1. On subject: an AI coding agent, a live demo, a crash. ✓
2. The laugh: reversal at the last clause — confident refactorer admits it
   never knew what the demo does. ✓
3. Truth: agents really do "clean up" working code they do not understand;
   demos really do die on stage. ✓
4. Economy: 133 characters, one line, no explanation. ✓
5. Freshness: confident ignorance revealed on stage — not a stock joke, not
   a reword of our 21 Nov entry. ✓

## Verification

- `MAKEFUN_OUTPUT_DIR=out node main.ts` and a second run into a different
  directory produce byte-identical `entry.txt`.
- Entry text: 133 code points (134 with trailing newline), one line,
  non-whitespace — inside the 1–280 gate.
- No network calls, no external binaries, no randomness, no clock.
- The program only writes inside the output directory; it never deletes
  the directory itself.
