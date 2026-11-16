# One Website, Millions of Users

**Type:** STEM explainer · **Week 8** (9 Nov 2026)
**Fellow:** Maitri P. · **Voice:** Kokoro `af_bella` (Bella), a synthetic narrator — disclosed on the outro card.

## This week's contribution
System-design explainer on how big websites serve millions of users: scale out to many identical servers, put a load balancer in front (round robin, least connections, IP hash), drop failed servers with health checks, autoscale on traffic spikes and serve from many regions plus a CDN. The catch: the balancer needs a backup, and the database is often the next bottleneck.

## Human and AI work
**My decisions and verification:** chose the topic, supplied the explanation and every number the video states, and reviewed the cuts.
**AI tools and what they generated:** Claude Code (Anthropic) turned my notes into the beat sheet, built and rendered the scenes, and fact-checked the claims (see `FACTCHECK.md`). Kokoro produced the narration.

## Reproduce
- **Brutalist toolkit:** commit `6fc9987` plus local uncommitted changes (scenes in `scenes/`). Not yet upstream.
- **Beat sheets:** `beat_sheet.json` (16:9), `vertical/beat_sheet.json` (9:16 native layouts).
- **Checks:** `FACTCHECK.md`, `SHOTLIST.md`, `PROMPTS.md`.

## Watch and review
- **Landscape** — `website-load-balancing.mp4` — 3840×2160 — 1:27.1 — SHA-256 `8feb03aa771ac159f3e500bd35a710514b41063e1591aeeb45e608b26bb89bab`
  Drive: pending
- **Vertical** — `website-load-balancing-vertical.mp4` — 2160×3840 — 1:27.1 — SHA-256 `00896a4e5482f8d31312cadc4ecdb762e56c8fff28a4f47ba2388cb4f6ee89f3`
  Drive: pending
