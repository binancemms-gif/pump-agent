# PumpAgent v2.5

Mobile-first autonomous Pump.fun token scanner and sniper control dashboard.

## Features

- **Live Scanner** — Real-time new token feed via PumpPortal WebSocket (falls back to simulation).
- **Autonomous Agent** — Start/stop button. Evaluates tokens against strategy rules + Shell Armor and logs snipe / skip / auto-sell decisions with latency.
- **Solana RPC Aware** — Parses getTransaction / simulateTransaction structures: meta.fee, computeUnitsConsumed, pre/postTokenBalances for accurate P&L calculation from balance deltas.
- **Tx Inspector** — View parsed transaction metadata, fees, compute units, and token balance changes.
- **Strategy Settings** — Min investment, max developer holdings, auto-sell, Shell Armor filters (including token balance delta and fee monitoring).
- **AI Analysis** — Agent chat that references Solana RPC meta for decisions.
- **P&L + Success Tracking** — Live dashboard with fees deducted and success rate from closed trades.
- **Referral Program** — Tiered SOL commissions UI.
- Fully mobile-optimized dark theme, bottom navigation, PWA-ready.

## Quick Start

```bash
git clone https://github.com/binancemms-gif/pump-agent.git
cd pump-agent
python3 -m http.server 8080
# Visit http://localhost:8080
```

Add to home screen on mobile for app-like experience.

## Notes

This is a frontend prototype. Real trade execution requires a separate backend bot (never store private keys in the browser). The agent now conceptually uses Solana RPC JSON structures (from the official reference) for more realistic P&L and safety checks.

High risk: most Pump.fun launches fail. Use only with funds you can afford to lose.
