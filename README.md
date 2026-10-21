# Crazy Bob v5.3.4 — Stable load on iPhone

Local AI web app for iPhone (WebLLM + WebGPU).

## Critical change in v5.3.4

**Auto-load of the last model is disabled.**

Previously the page tried to restore the model as soon as it opened. On iOS this frequently caused Safari to kill the tab with no error message (jetsam / memory pressure). The tab would just disappear.

Now:
1. Open the page.
2. Wait a couple of seconds for it to settle.
3. Close other Safari tabs if possible.
4. Tap **Load**.

The last model you used is still pre-selected in the dropdown.

## Models

- SmolLM2 360M — safest
- Qwen2.5 0.5B — light
- Llama 3.2 1B — balanced
- Llama 3.2 1B q4f32 — if f16 is a problem
- Qwen2.5 1.5B — default (worked for you before)
- Llama 3.2 3B — heavy, high crash risk

## Deploy

Upload the files to the root of your GitHub Pages repo so `index.html` is at the site root.
