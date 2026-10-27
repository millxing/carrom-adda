# Carrom Adda: notes for agents

## Which file is the game
- `index.html` is the one live file, always the latest version. The whole game (HTML, CSS, JS) is in it. Edit it directly.
- Do NOT create new `carrom_adda_vNN.html` copies for releases. Versions are tracked with git tags (below).
- `carrom_adda_v08.html` is only a redirect stub to `/` for old links. Never edit it as if it were the game.
- `archive/` holds old versions (v05-v07), noindex, kept for reference only.

## Hosting
- GitHub Pages serves `main` at https://carromadda.org/ (`CNAME`). Pushing to `main` publishes it. Pages caches for about 10 minutes.
- SEO bits live in `index.html` (title, description, canonical, JSON-LD, the visually hidden `#about` text), `robots.txt`, `sitemap.xml`. Keep the `#about` text accurate if the rules or modes change. Update `sitemap.xml` `lastmod` on releases.
- The social card is `social-card.jpg` (1200x675).

## Versions and releases
- `VERSION` in `index.html` (shown on the menu screen) is the current version, e.g. `08.1`.
- To release: bump `VERSION`, add a line to `CHANGELOG.md`, commit, `git tag v<VERSION>`, push main and the tag (`git push --follow-tags`).
- Previous versions: `git checkout v08` (or any tag). `git tag` lists them.
- Tag `v08` is the game as of the last commit before the carromadda.org restructure.

## Conventions
- Match the existing style of the single file: compact, comments explain why.
- Replays are deterministic (seeded physics); do not change physics or rules without thinking about old recordings in `recorded_games/`.
