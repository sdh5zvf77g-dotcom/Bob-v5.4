# Changelog

## v5.3.4 — Stop auto-load crash (jetsam kill)

- **Completely disabled automatic model restore on page load.**
  This was the main cause of the tab dying with no error when reopening the app.
  Safari was being killed by iOS memory pressure (jetsam) while the model was being
  restored in the background. You must now tap **Load** yourself after the page settles.
- Longer GPU memory release pause after unloading a previous engine.
- History restore and embedder start are delayed until the LLM is fully ready.
- Clearer error message when an OOM / device-lost style failure is detected.
- Default remains Qwen2.5 1.5B (the model that was working for you).

## v5.3.2 — More free information sources
- Wikipedia improved, free dictionary, RSS, Hacker News paths.
- Default was Qwen2.5 1.5B.

## v5.3.1 / earlier
- Learning ledger, training pipeline, model selector, etc.
