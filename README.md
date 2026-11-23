# TokenCost Zero — Free Local LLM Token Counter & Multi-Model API Cost Calculator

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Zero-dependency, 100% browser-local LLM prompt token estimator and API pricing comparator across **OpenAI (GPT-4o-mini / GPT-4.1 / GPT-5)**, **Anthropic (Claude 3.5 Haiku / Sonnet 4 / Opus 4)**, **Google (Gemini 2.5 Flash-Lite / Flash / Pro)**, **DeepSeek (V3.2 / R1)**, and **Alibaba (Qwen-Max / Plus)**.

- **Live Web App (No Signup / Zero Telemetry)**: https://devbox-zero-ops.github.io/tokencost-zero/
- **Privacy Guarantee**: Every token calculation executes client-side in plain JavaScript. No prompts, API keys, cookies, or usage metrics ever leave your browser.

## Key Capabilities

- **Bilingual EN / CJK Token Estimator**: Separately estimates CJK characters (`~1.45` tokens/char) vs ASCII/Latin text (`~3.8` chars/token) for realistic input token sizing.
- **Prompt Cache Hit-Rate Modeling**: Models effective blended input pricing `inputPrice * (1 - hitRate) + cachedPrice * hitRate` per provider.
- **Coding Agent Workload Preset**: One-click preset (`25k` input tokens, `2k` output tokens, `70%` cache hit rate, `200` requests/day) for Claude Code / Codex / Cursor agent spend planning.
- **Sorted Cost Table & CSV Export**: Compares per-1k-call spend and 30-day monthly spend sorted lowest-to-highest, with instant `.csv` export.
- **Bilingual UI (English / 中文)**: Automatic browser language detection plus manual switcher.

## Local Usage

Open `index.html` directly in any modern browser, or serve locally:

```bash
python -m http.server 8080
```

## Related Zero-Tracking Developer Utilities

- [XiaheAI Developer Hub](https://devbox-zero-ops.github.io/xiaheai-hub/) — Guides, cost comparisons & open-source utility suite
- [DevBox Zero](https://devbox-zero-ops.github.io/devbox-zero/) — Local JSON / JWT / Base64 / Cron / Diff / UUID utilities
- [InvoiceZero](https://devbox-zero-ops.github.io/invoice-zero/) — Bilingual watermark-free A4 invoice & quotation generator
- [ResumeMD Zero](https://devbox-zero-ops.github.io/resumemd-zero/) — Markdown-to-PDF ATS resume builder

## Support Maintenance (Optional · MIT Open Source)

- **EVM USDT (Arbitrum / Polygon / Ethereum / BSC, USDC compatible)**: `0xe4c8739bCC488bD98978CE976511735e0499d432`
- **Solana USDT (SOL / USDC compatible)**: `89XqpaJDKajhYFs4Vmex853yxoEU7HqwnMAPtTDpgZgG`
