# IPPT Tracker

A personalised **Singapore IPPT** (Individual Physical Proficiency Test) score tracker — single-file web app, dark sporty dashboard. Computes your score live, logs attempts over time, shows trends, and gives **rule-based AI insights & recommendations**.

Live site: **https://ncheewee.github.io/ippt-tracker/**

## Features

- **Live score calculator** — enter 2.4km time, sit-ups, push-ups → total score (/100), per-station points, and award.
- **Accurate SAF male scoring tables** — 14 age groups, run (50 pts) + sit-ups (25) + push-ups (25). Tables adapted from [`ninest/ippt-utils`](https://github.com/ninest/ippt-utils) (MIT).
- **Awards** — Gold (≥85, or ≥90 for Commando/Diver/Guards), Silver (≥75), Pass with Incentive (≥61), Pass (≥51), Fail.
- **Attempt history** — log every IPPT, see a trend chart, and per-station deltas vs your last attempt.
- **AI insights (rule-based)** — identifies your weakest station, the fastest point-path to your target award, trend analysis, and station-specific coaching.
- **GitHub sync** — your history is committed to `history.json` in this repo via the GitHub Contents API using your own Personal Access Token. Cross-device, no backend.
- **Private** — all data lives in your browser's localStorage + your own repo. No tracking, no server.

## Scoring data source

Tables adapted from [`ninest/ippt-utils`](https://github.com/ninest/ippt-utils) and [`ninest/IPPT`](https://github.com/ninest/IPPT) (both MIT). This is an **unofficial** tool — always verify against [ns.sg](https://www.ns.sg/).

## Local usage

Just open `index.html` in a browser. No build step.

## Deploy

This repo is published via GitHub Pages from the `main` branch (`/` root).
