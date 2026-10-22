# Carrom Adda

Carrom against an AI, AI vs AI, or a friend online (2 players over the internet), played in the browser. Realistic 2-D rigid-disc physics with spin, a ring striker, cushion and piece friction, and tunable table settings.

## Play

Play at https://carromadda.org/ or open `index.html` in any modern browser. No install and no server. Playing the AI needs no network; online play loads PeerJS from a CDN when you use it.
(`sounds/score.mp3` is optional: if it is missing the pocket sound is synthesised.)

- Mouse: click the board to aim, drag the striker along your baseline, scroll the wheel over the board (Shift coarse, Alt fine) or drag the power bar on the board's left edge to set power. Optional: shoot when the bar is released (physics settings drawer).
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
- Pocket a piece and shoot again. The queen only counts once you have already pocketed one of your own pieces; before that she goes back to the centre. Cover the queen with one of your own pieces on the next shot.
- Winner scores 1 point per opponent piece left, plus 3 for a queen they covered.
- Every game is recorded automatically. Start screen > Recordings & replays: watch at 1-8x, save a game as a `.json` file, load one back in. Replays re-run the physics from the recorded seed and shots, so they are exact.
- Online: Start screen > Play a friend online. One player hosts and sends the invite link or 5-character code; the other opens it or types the code. The host's table physics and shot error apply to both, the guest sees the board turned around so they always shoot from the bottom, and a game can be restarted as a rematch. Only the shots travel between the browsers (the physics is deterministic); after each shot the shooter's final board is adopted by the other side, so browsers that round differently can't drift apart. Connection is peer to peer (WebRTC) and may fail behind strict firewalls.
- Players: choose AI vs AI on the start screen to watch two AIs play, each with its own level.
- Three AI levels. Physics presets and every tunable parameter are behind the ⚙ button.

## Files

- `index.html` - the game (everything is in this one file; always the latest version, see `CHANGELOG.md` and git tags)
- `CLAUDE.md` - notes for agents: file layout, hosting and the release steps
- `archive/` - previous versions (v05-v07; sounds paths are not fixed) (v06 has no online play and lets the queen go down first)
- `robots.txt`, `sitemap.xml` - search engine files
- `sounds/score.mp3` - pocket sound (optional)

## License

Copyright (c) 2026 Rob Schoen. Free for noncommercial use under the
[PolyForm Noncommercial License 1.0.0](https://polyformproject.org/licenses/noncommercial/1.0.0). See `LICENSE`.
