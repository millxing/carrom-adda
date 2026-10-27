# Changelog

## 08.6
- Striker can move forward off the baseline, up to (not over) the inner square: W/S keys, Forward slider, or drag. The AI uses it too.
- New rule: if the queen goes in on the break together with a white, she stays off the table (and can't be covered) until the breaker's turn ends, then goes back to the centre. Older replays keep the old rule.
- Inner square is a setting (default 0.28 m from the cushion); default piece diameter 40 mm.
- Side panel opens on the Watch Log; video-recorder build removed.

## 08.5
- AI goes for the queen earlier: when it can pocket her and has an easy cover shot lined up, it takes her instead of waiting until its last piece.

## 08.4
- AI breaks hard again: dedicated opening-break shots, with power set by difficulty (Easy ~2, Expert ~3).
- Menu: version number under the title, and a "What is Pakistani Carrom?" link.

## 08.3
- AI thinks 6-7x faster (Expert ~2 s on the opening board, was ~14 s). Physics results are unchanged, so old recordings replay the same.

## 08.2
- New Expert AI difficulty.
- AI rebalance: stronger Easy, weaker Hard; occasional blunders; bank shots limited by level (none on Easy, one bounce on Medium, two on Hard and Expert).

## 08.1
- Served at https://carromadda.org/ as `index.html` (no more versioned copies); versions tracked by git tags.
- SEO: keyword title and description, JSON-LD, crawlable how-to-play text, robots.txt, sitemap.xml.
- New social sharing card.
- Version number shown on the menu.

## 08
- Bug/feedback email on the selection screen; selection screen centred; one striker in the menu background; social sharing card tags.

## 05-07
- Earlier versions, in `archive/` (v06 has no online play and lets the queen go down first).
