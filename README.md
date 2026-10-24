# PumpAgent v3.0

Mobile-first autonomous multi-chain token scanner and sniper control dashboard.

## Features

- **Multi-Chain** — Switch between Solana (Pump.fun) and BNB Chain (four.meme style) with one tap.
- **Live Scanner** — Real-time new token feed on Solana via PumpPortal WebSocket; realistic simulation on BNB.
- **Autonomous Agent** — Start/stop button. Evaluates tokens against strategy rules + Shell Armor and logs snipe / skip / auto-sell decisions with latency.
- **Adaptive P&L** — Tracks profit in SOL or BNB depending on active chain, with success rate and fees.
- **Tx Inspector** — Parses Solana RPC structures (getTransaction meta, pre/postTokenBalances, compute units) or BSC receipts.
- **Strategy Settings** — Min investment, max developer holdings, auto-sell, Shell Armor filters.
- **AI Analysis** — Multi-chain aware agent chat.
- **Referral Program** — Tiered commissions UI.
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

This is a frontend prototype. Real trade execution requires a separate backend bot (never store private keys in the browser). Solana uses live PumpPortal data when available; BNB uses simulation modeled on four.meme bonding curves.

High risk: most meme launches fail. Use only with funds you can afford to lose.
