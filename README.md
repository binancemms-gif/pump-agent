# PumpAgent v2.4

Mobile-first autonomous Pump.fun token scanner and sniper control dashboard.

## Features

- **Live Scanner** — Real-time new token feed via PumpPortal WebSocket (falls back to simulation).
- **Autonomous Agent** — Start/stop button. Evaluates tokens against strategy rules + Shell Armor and logs snipe / skip / auto-sell decisions with latency.
- **Strategy Settings** — Min/max investment, slippage, TP/SL, max developer holdings, auto-sell.
- **Shell Armor Protection** — Rug-pull, honeypot, and scam filters.
- **AI Analysis** — Agent chat panel for token scoring and strategy questions.
- **P&L + Success Tracking** — Live dashboard cards that update from closed trades (success rate calculated from actual simulated outcomes) and agent logs.
- **Referral Program** — Tiered SOL commissions UI.
- Fully mobile-optimized dark theme, bottom navigation, PWA-ready.

## Quick Start

```bash
# Open directly or serve
python3 -m http.server 8080
# Visit http://localhost:8080
```

Add to home screen on mobile for app-like experience.

## Notes

This is a frontend prototype. Real trade execution requires a separate backend bot (never store private keys in the browser). Pair with the educational patterns from community pump.fun bots and local AI tools (Ollama + OpenCode) for production use.

High risk: most Pump.fun launches fail. Use only with funds you can afford to lose.
