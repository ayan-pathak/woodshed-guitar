# Woodshed

A guitar playground for learning to solo by ear. Put your hand in the box, play anything in it, and it fits the song.

Live: https://woodshed-guitar-b98.pages.dev

## What it does

- **The neck**: shows the pentatonic box for any key, with finger, scale-degree or note-name labels. Tap notes to hear them. Bluesy (minor) and Sweet (major) moods, plus an optional blue note and whole-neck view.
- **Jam**: synthesized backing tracks (12-bar blues, minor groove, sweet pop, ballad, vamps) with a tempo control. The current chord's notes are ringed on the neck.
- **Listen to me**: mic pitch detection shows each note you play, green if it's in the box, red if not.
- **Find a song's key**: listens to any song through the mic, estimates the key (Krumhansl–Schmuckler) and says the fret out loud.
- **Echo game**: plays a short phrase from the box. Play it back by ear and hear a chime when you match it. Phrases get longer as you improve.

## Run locally

It's a single static file with no build step:

```
python -m http.server 8765
```

Then open http://localhost:8765. The mic needs https or localhost.

## Deploy

```
npx wrangler pages deploy . --project-name woodshed-guitar --branch main
```
