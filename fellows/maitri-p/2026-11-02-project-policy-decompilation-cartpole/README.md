# Can a Network Become Code?

**Type:** Project update · **Week 7** (2 Nov 2026)
**Fellow:** Maitri P. · **Voice:** Kokoro `af_bella` (Bella), a synthetic narrator — disclosed on the outro card.

## This week's contribution
Policy Decompilation on CartPole: trained a 234-parameter agent (477.99 / 500), recorded 30 games and all 24 neurons, found a push-right / push-left neuron pair, fitted short if/else code (47 nodes → 92.8% same move), rebuilt a network from the code by hand (10,000 / 10,000 steps identical to the code) and tested it on 100 unseen games (95.91% same move, 484.67 / 500). Not yet a full match: 0 of 100 games match at every step.

## Human and AI work
**My decisions and verification:** chose the topic, supplied the explanation and every number the video states, and reviewed the cuts.
**AI tools and what they generated:** Claude Code (Anthropic) turned my notes into the beat sheet, built and rendered the scenes, and fact-checked the claims (see `FACTCHECK.md`). Kokoro produced the narration.

## Reproduce
- **Brutalist toolkit:** commit `6fc9987` plus local uncommitted changes (scenes in `scenes/`). Not yet upstream.
- **Beat sheets:** `beat_sheet.json` (16:9), `vertical/beat_sheet.json` (9:16 native layouts).
- **Checks:** `FACTCHECK.md`, `SHOTLIST.md`, `PROMPTS.md`.

## Watch and review
- **Landscape** — `policy-decompilation-cartpole.mp4` — 3840×2160 — 1:43.2 — SHA-256 `05bcb5bb470e8468815016b9683b1e10e6f3aa3da6103ddacc65d9e2fcc321db`
  Drive: pending
- **Vertical** — `policy-decompilation-cartpole-vertical.mp4` — 2160×3840 — 1:43.2 — SHA-256 `420bb1150c18998b0bfaf34a9568919d2707f1f5a523726b25c4897112870f9c`
  Drive: pending
