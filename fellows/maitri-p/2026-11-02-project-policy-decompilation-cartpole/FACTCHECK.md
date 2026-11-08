# FACTCHECK — policy-decompilation-cartpole (week of 2026-11-02)

All numbers are the fellow's own results, read from her weekly notes
(saved reports: `artifacts/verification_report.json`, `artifacts/decompiled_policy.py`,
`artifacts/fidelity_vs_ast_curve.png`, `artifacts/neuron_correlations.png`).
Not re-run by Claude.

| # | Claim (beat) | Verdict |
|---|---|---|
| 1 | Network: 2 hidden layers, 16 + 8 neurons, 234 parameters (B02) | Fellow's result. Arithmetic consistent: 4·16+16 + 16·8+8 + 8·2+2 = 234 for CartPole's 4 inputs, 2 actions |
| 2 | Trained with policy gradient (B02) | Fellow's account |
| 3 | Original scores 477.99 / 500 over 100 unseen games (B02) | Fellow's result; CartPole-v1 caps an episode at 500 steps — TRUE |
| 4 | 30 games, 14,916 steps, all 24 neurons recorded (B02) | Fellow's result; 16 + 8 = 24 hidden neurons — consistent |
| 5 | L2_N3 ↔ push right, corr 0.81; L2_N6 ↔ push left, corr −0.80 (B03) | Fellow's result |
| 6 | Size vs same-move: 47→92.8%, 65→96.2%, 115→96.7%, 191→97.8% (depth 2/3/4/6), on recorded games (B04) | Fellow's result |
| 7 | Code vs rebuilt network: 10,000 / 10,000 steps identical (B05) | Fellow's result |
| 8 | 100 unseen games, 47,799 steps; 95.91% same move; rebuilt 484.67 vs 477.99 — 73-node version (B05) | Fellow's result. Note: 73 nodes is not one of the depths in the scan (B04); it is the saved report's version |
| 9 | Larger 115-node version: 96.01%, 492.28 | Fellow's result — in notes, not on screen |
| 10 | 0 of 100 games match at every step (B06) | Fellow's result, stated as the open goal |
| 11 | Rules fitted from behaviour, not from neurons; CartPole only; no VIPER or LLM comparison yet (B06) | Fellow's account |
| 12 | 19 tests passing; CLI; live dashboard (B06 footer) | Fellow's account |
| 13 | Next: rules from neuron activations; MountainCar, MiniGrid (B07) | Fellow's plan |
| 14 | "like a gas and a brake pedal" (B03) | Fellow's analogy |
