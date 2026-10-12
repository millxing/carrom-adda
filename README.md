# Carrom Adda

Single-player carrom (or AI vs AI) against an AI opponent, played in the browser. Realistic 2-D rigid-disc physics with spin, a ring striker, cushion and piece friction, and tunable table settings.

## Play

Open `carrom_adda_v05.html` in any modern browser. No install, no server, no network needed.
(`sounds/score.mp3` is optional: if it is missing the pocket sound is synthesised.)

- Mouse: click the board to aim, drag the striker along your baseline.
- Keyboard:

  | Keys | Action |
  |---|---|
  | ← → | Aim left / right (0.1° per press) |
  | ↑ ↓ | Power up / down (0.05 m/s per press) |
  | A D | Slide the striker along the baseline (1 cm per press; `carrom_ada_opus.html` only) |
  | Hold Shift | 10× bigger steps |
  | Hold Alt / ⌥ | Finer steps |
  | Space or Enter | Shoot |
- Win the hand-guess toss to break; the breaker plays white.
- Pocket a piece and shoot again. Cover the queen with one of your own pieces on the next shot.
- Winner scores 1 point per opponent piece left, plus 3 for a queen they covered.
- Every game is recorded automatically. Start screen > Recordings & replays: watch at 1-8x, save a game as a `.json` file, load one back in. Replays re-run the physics from the recorded seed and shots, so they are exact.
- Players: choose AI vs AI on the start screen to watch two AIs play, each with its own level.
- Three AI levels. Physics presets and every tunable parameter are behind the ⚙ button.

## Files

- `carrom_adda_v05.html` - the game (everything is in this one file)
- `index.html` - redirects to the game (for GitHub Pages)
- `sounds/score.mp3` - pocket sound (optional)

## License

Copyright (c) 2026 Rob Schoen. Free for noncommercial use under the
[PolyForm Noncommercial License 1.0.0](https://polyformproject.org/licenses/noncommercial/1.0.0). See `LICENSE`.
