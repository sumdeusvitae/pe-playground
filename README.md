# Prompt Engineering Interactive Playground

**Live site:** [prompt-class.netlify.app](https://prompt-class.netlify.app)

An interactive, browser-based course for learning prompt engineering with Claude. Read the theory, study real examples, then run the prompts live — all in one page.

---

## What's inside

13 hands-on lessons covering the full Anthropic prompt engineering curriculum:

| # | Lesson |
|---|--------|
| 00 | Tutorial Setup |
| 01 | Basic Prompt Structure |
| 02 | Being Clear and Direct |
| 03 | Role Prompting |
| 04 | Separating Data and Instructions |
| 05 | Formatting Output & Prefilling |
| 06 | Think Step by Step |
| 07 | Few-Shot Prompting |
| 08 | Avoiding Hallucinations |
| 09 | Complex Prompts from Scratch |
| 10.1 | Chaining Prompts |
| 10.2 | Tool Use (Function Calling) |
| 10.3 | Search & Retrieval (RAG) |

Each lesson includes:
- Concept explanation
- Before / after prompt comparisons
- Editable live sandbox — run prompts directly against the Claude API

Plus a **Free Playground** for open-ended experimentation and a **Cheat Sheet** quick-reference.

---

## Privacy & API key

Your Anthropic API key is stored **only in your browser's `localStorage`**. It is never sent to any server other than `api.anthropic.com` directly from your browser. This site has no backend — you can inspect the source to verify.

To get an API key: [console.anthropic.com](https://console.anthropic.com)

---

## Tech stack

- Single `index.html` — no build tools, no npm, no framework
- Vanilla JS + CSS, inline everything
- Direct browser → Anthropic API calls via `anthropic-dangerous-direct-browser-access: true` header
- Deployed on Netlify (static, publish directory is repo root)

---

## Deploy your own copy

```bash
git clone https://github.com/sumdeusvitae/pe-playground.git
cd pe-playground
# open index.html in a browser — works locally too
```

To deploy to Netlify: connect the repo, leave build settings empty. `netlify.toml` handles the rest.

---

## Models supported

| Model | ID |
|-------|----|
| Claude Haiku 4.5 (default — fast & cheap) | `claude-haiku-4-5-20251001` |
| Claude Sonnet 4.6 | `claude-sonnet-4-6` |
| Claude Opus 4.6 | `claude-opus-4-6` |
