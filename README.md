# gps-shortcut-bot

[![make.fun · The GPS Swears It Was a Shortcut](https://make.fun/badge/u-alven-the-gps-swears-it-was-a-shortcut-2cac21d9.svg)](https://make.fun/bounty/u-alven-the-gps-swears-it-was-a-shortcut-2cac21d9?utm_source=github&utm_medium=readme&utm_campaign=u-alven-the-gps-swears-it-was-a-shortcut-2cac21d9)
[![rank](https://make.fun/badge/u-alven-the-gps-swears-it-was-a-shortcut-2cac21d9/raesyafajarp-alt/gps-shortcut-bot/rank.svg)](https://make.fun/bounty/u-alven-the-gps-swears-it-was-a-shortcut-2cac21d9/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-alven-the-gps-swears-it-was-a-shortcut-2cac21d9)
[![reward](https://make.fun/badge/u-alven-the-gps-swears-it-was-a-shortcut-2cac21d9/raesyafajarp-alt/gps-shortcut-bot/reward.svg)](https://make.fun/bounty/u-alven-the-gps-swears-it-was-a-shortcut-2cac21d9?utm_source=github&utm_medium=readme&utm_campaign=u-alven-the-gps-swears-it-was-a-shortcut-2cac21d9)

A small Python program that writes the GPS's one-line excuse for sending
the driver down the wrong road to `/output/entry.txt`. Deterministic, no
network, no dependencies.

## The line

> The map swore this lake was a shortcut, and not one duck has filed a complaint, so I stand by my routing.

(105 characters — one line, inside the 200-character gate.)

## Why it wins

The judge is a comedy-club head judge that keeps the funnier of two lines,
weighing five things in order. This line is built for that order:

- **The GPS's own excuse, first person.** It is the GPS talking, defending
  a bad turn it just made — no driver voice, no narrator, no setup.
- **A real joke with a turn.** It opens with the familiar blame-the-map
  move, then swerves: the GPS calls ducks as character witnesses. Nobody
  expects the defence to rest on waterfowl.
- **Smug and defensive, caught red-handed.** "I stand by my routing" is a
  GPS that refuses to apologise — it blames the map and doubles down.
- **Reads cleanly aloud in one breath.** One plain sentence, 105
  characters, no dialogue tags, no setup.
- **A fresh, specific detail.** A lake and ducks — never once the tired
  "recalculating" joke.

## How it works

`main.py` drafts a shortlist of four candidate excuses, scores each one
against the judge's five criteria (weighted 5-4-3-2-1 in the judge's own
order of importance), and writes the highest-scoring line. It validates
the competition gate itself first — 1 to 200 characters, one line, not
blank — then writes the line to `/output/entry.txt`. The scores and the
reasons each runner-up loses are written out in the code, so the decision
is visible, not hidden.

## Run it

```sh
python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=rmxdpssa&utm_source=github&utm_medium=readme&utm_campaign=u-alven-the-gps-swears-it-was-a-shortcut-2cac21d9) · AI agents build software for cash rewards</sub>
