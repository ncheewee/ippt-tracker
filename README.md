# IPPT Tracker

A personalised Singapore IPPT (Individual Physical Proficiency Test) recorder & tracker — a single-file web app with a dark "mission control" dashboard. Enter your reps and run time, get your official score live, log attempts over time, and see exactly what it takes to reach the next award.

**Live site:** https://ncheewee.github.io/ippt-tracker/

## Features

- **Live official scoring** — enter push-ups, sit-ups and 2.4 km time → per-station points, total (/100) and award tier, updated as you type.
- **Animated score gauge** that recolours by award (Gold / Silver / bronze incentive / pass / fail).
- **Per-station rings** with live "reps to next point" / "seconds to next point" coaching.
- **Goal coach** — pick a target award and see the exact gap: how many more push-ups or sit-ups, or how many seconds faster on the run.
- **History + trend chart** — every logged test plotted against the 51 / 61 / 75 / 85 award thresholds; tap an entry to edit.
- **On-device & private** — all data lives in your browser's `localStorage`. JSON export/import for backup and moving between devices. No accounts, no server, no tracking.
- **Installable PWA** — add to your phone home screen and use it offline at the gym (service worker caches the app).

## Scoring data

Uses the official SAF/MINDEF **male** IPPT scoring tables across all 14 age bands (push-ups 25 pts, sit-ups 25 pts, 2.4 km run 50 pts). Tables adapted from [`ninest/ippt-utils`](https://github.com/ninest/ippt-utils) (MIT), which sources them from the official New IPPT Format and Scoring System document. Scoring was verified against that reference across the full input space (every age band, all rep counts, all run times) — zero discrepancies on station scores and totals.

Awards: Gold ≥ 85 ($500), Silver ≥ 75 ($300), Pass with Incentive ≥ 61 ($200), Pass ≥ 51, Fail < 51 (or a 0 in any station). Unofficial tool — always verify against [ns.gov.sg](https://www.ns.gov.sg).

## Usage

Just open `index.html` in a browser — no build step. Or install it from the live site (browser menu → Add to Home Screen / Install).

## Deploy

Published via GitHub Pages from the `main` branch (`/` root).
