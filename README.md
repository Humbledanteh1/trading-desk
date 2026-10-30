# Trading Desk

A general-purpose, multi-asset trading workspace for watchlists, positions, risk planning and trade review.

## Features
- Market watchlist with manual price updates and asset classes.
- Open-position book with entry, stop, target, quantity and estimated planned risk.
- Closed-trade journal with setup, execution grade, notes and CSV export.
- Risk calculator for sizing and illustrative reward/risk target.
- Performance summary: realized P&L, win rate, average win/loss and profit factor.
- Desk notes for session plans and levels.

## Run locally
Open `index.html` in a modern browser. No build step or dependencies are required.

## Deploy
Import this repository into Vercel. It is a static site; use the repository root as the project root and leave the build command empty.

## Data and safety
- This version is manual-only. It has no live market feed, broker connection, account sync or order execution.
- Watchlist, positions, journal and notes are stored in browser localStorage on the current device/browser.
- Position sizing is an estimate. Verify contract specifications, pip/point value, lot increments, commissions and slippage for the instrument you trade.
- Do not put API keys, passwords, wallet seed phrases or broker secrets in this repository.

## Next
Choose your preferred market-data and trading platform before adding integrations. Start with read-only data access; add execution only with explicit approvals and robust safeguards.
