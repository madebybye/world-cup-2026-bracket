# World Cup 2026 — Knockout Bracket

A minimal, single-file interactive bracket for the 2026 FIFA World Cup knockout stage (Round of 32 → Final). No build step, no dependencies — just open `index.html`.

**Live:** https://madebybye.github.io/world-cup-2026-bracket/

## Features
- **Live during games** — polls ESPN's public scoreboard feed: in-game win probability, projected final score, and automatic result-locking at full-time (the whole bracket recomputes).
- **FIFA-ranking predicted scorelines** — every matchup's score is a function of the two teams' FIFA world rankings. Picking a lower-ranked team to beat a higher-ranked one is scored as a bigger upset (more goals); all 496 ordered matchups are pre-computed at load.
- **Pick overrides** — tap any team to send them through; downstream matchups, scores and the advancement bars update instantly. Picks persist and are shareable via the URL.
- Minimal light theme; responsive down to mobile.

## Data sources
- Fixtures, live scores & results: **ESPN** (`site.api.espn.com`).
- Team strength & predicted scorelines: **FIFA World Ranking** (men's, June 2026).
- The bracket structure, wiring and ESPN event IDs are derived deterministically from the ESPN feed.

Not affiliated with FIFA or ESPN.
