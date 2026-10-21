# Changelog

## v5.3.3 — Crash resistance on model restore
- Default model changed back to **Llama 3.2 1B** (more stable on iPhone than 1.5B).
- Auto-restore is now conservative: only ≤1B models auto-load after a page refresh. 1.5B / 3B require a manual Load tap (prevents crash loops).
- Longer GPU memory release pause before loading a new model.
- On OOM / memory kill, the selector automatically switches to SmolLM2 360M and clears the last heavy model preference.
- Clearer progress warnings when a heavier model is chosen.

## v5.3.2 — More free information sources
- **Wikipedia improved**: direct summary + OpenSearch fallback when the exact title fails.
- **Research (free path)** now also pulls:
  - Free Dictionary API for short phrases
  - Free RSS headlines via feed2json (BBC / NPR / Guardian)
  - Hacker News top stories (tech / current discussion)
- News still prefers Serper/Tavily when keys exist; free RSS remains available without keys.
- Default model: Qwen2.5 1.5B. (reverted in 5.3.3 for stability)

## v5.3.1 — News keys-first
- When Serper or Tavily keys are present, news uses those APIs first.
- Free RSS converters kept as fallback.

## v5.3 / earlier
- Learning ledger, training pipeline, model selector, etc.
