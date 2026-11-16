# Your Face, as Numbers

**Type:** STEM explainer · **Week 6** (26 Oct 2026)
**Fellow:** Maitri P. · **Voice:** Kokoro `af_bella` (Bella), a synthetic narrator — disclosed on the outro card.

## This week's contribution
Explainer on how a phone recognizes your face: Face ID projects 30,000+ infrared dots to build a 3D depth map, a neural network turns it into a list of numbers, and each unlock checks whether the new list is close enough to the saved one. Covers the strict-vs-loose threshold trade-off, on-device storage in the Secure Enclave, Apple's under 1-in-a-million figure, and why 2D camera face unlock is easier to fool than a 3D scan.

## Human and AI work
**My decisions and verification:** chose the topic, supplied the explanation and every number the video states, and reviewed the cuts.
**AI tools and what they generated:** Claude Code (Anthropic) turned my notes into the beat sheet, built and rendered the scenes, and fact-checked the claims (see `FACTCHECK.md`). Kokoro produced the narration.

## Reproduce
- **Brutalist toolkit:** commit `6fc9987` plus local uncommitted changes (scenes in `scenes/`). Not yet upstream.
- **Beat sheets:** `beat_sheet.json` (16:9), `vertical/beat_sheet.json` (9:16 native layouts).
- **Checks:** `FACTCHECK.md`, `SHOTLIST.md`, `PROMPTS.md`.

## Watch and review
- **Landscape** — `face-unlock.mp4` — 3840×2160 — 1:19.0 — SHA-256 `3836e1fed8e67a5b3510d27b8ba5c29b59b31251895b850cb6c5454ff59d9af7`
  Drive: pending
- **Vertical** — `face-unlock-vertical.mp4` — 2160×3840 — 1:19.0 — SHA-256 `8104e714a85a63fae29b1f3d6709e79b36281ef065d49abcae44c69b37507be3`
  Drive: pending
