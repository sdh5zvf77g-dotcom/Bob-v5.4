# Changelog

## v5.3.2 — More free information sources
- **Wikipedia improved**: direct summary + OpenSearch fallback when the exact title fails.
- **Research (free path)** now also pulls:
  - Free Dictionary API for short phrases
  - Free RSS headlines via feed2json (BBC / NPR / Guardian)
  - Hacker News top stories (tech / current discussion)
- News still prefers Serper/Tavily when keys exist; free RSS remains available without keys.
- Default model: Qwen2.5 1.5B.

## v5.3.1 — News keys-first
- When Serper or Tavily keys are present, news uses those APIs first.
- Free RSS converters kept as fallback.

## v5.3 / earlier
- Learning ledger, training pipeline, model selector, etc.
