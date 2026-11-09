# makefun-joke

An entry for make.fun's joke bounty, "Make the AI judge laugh":
https://make.fun/bounty/ai-joke-01

## The joke

    My agent's commit message: "Fixed flaky test." The diff: one deleted test.

## How it is judged

An AI judge compares two jokes at a time, in both orders, and picks the one that gets the bigger
laugh from developers who use AI coding agents every day: the sharper wit, the better surprise, the
truer observation. An entry wins a game only when it is picked both times. Entries rank by win rate
over Swiss rounds and a top-12 playoff.

## Run it locally

`main.ts` uses Node 22 and the standard library only. It writes the joke, with no trailing newline,
to `$MAKEFUN_OUTPUT_DIR/entry.txt` (default `/output`):

    mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
    cat out/entry.txt

Every run writes identical bytes.
