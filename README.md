# Referee — Sports Decision Intelligence

**A player-prop analytics platform that scores betting-market opportunities from data, lines, and game context — and turns them into clear, confidence-rated picks.**

> 📌 This repository is a **public case study**. It documents the product, the analytics engine, and the design. Built as an independent product venture under the Vizwin umbrella.

---

## The idea

Sports prop markets are noisy and overwhelming: dozens of players, multiple sportsbooks, lines that move, and context (injuries, matchups, recent form) scattered everywhere. Referee's job is to **compress that into a decision** — a scored, explained opinion on a given player prop, plus tools to combine picks and track results.

The product direction deliberately evolved from a simple "betting assistant" into a broader **sports decision-intelligence** system: the value isn't a hot take, it's a *repeatable, data-driven scoring process* with confidence and transparency.

## What it does

| Feature | What it does |
| --- | --- |
| **AI Odds scoring** | Generates a model-driven price for a player prop (Over/Under) so users can compare it against the sportsbook line |
| **Parlay Calculator (hero)** | Build a slate of picks, auto-suggest combinations, and compute combined AI odds before committing |
| **The Vizwin Vision** | Per-prop writeup — game info, injury status, and a plain-English rationale for the score |
| **Report Card** | Turns a user's pick history into letter-grade analytics (discipline, consistency, chasing longshots) instead of a raw P&L blur |
| **Multi-book aware** | Designed around major sportsbooks (DK / MGM / CZ / FD / UD) for line comparison |

## Engineering & design highlights

- **Deterministic analytics core** — scoring is computed from structured inputs, not vibes, so the same data yields the same call and results are explainable.
- **Confidence scoring** — every opportunity carries a confidence signal, the honest acknowledgement that not all edges are equal.
- **Consumer-grade UX** — pure-black + electric-cyan neon system, mobile-first, built to feel like a product a real user wants to open, not a spreadsheet.
- **Separation of concerns** — analytics/backend logic kept independent of the presentation layer (the frontend was redesigned without touching the verified scoring backend).

## What I took from building it

This project was a deep lesson in **noisy-signal product discipline**: data pipelines, confidence scoring, consumer UX, API integration, and — most importantly — *product-market-fit honesty* about where a data product genuinely adds value versus where it's just noise dressed up as insight.

## Tech stack

`TypeScript` · `Next.js` · `Node` · `Prisma` · structured analytics engine · deterministic scoring · responsive web UI

---

<sub>Built by Austin Stevens — Applied AI & Data Analytics, University of Tennessee, Knoxville. Product/architecture case study; full source kept private. Referee is an analytics & decision-support tool, not betting advice.</sub>
