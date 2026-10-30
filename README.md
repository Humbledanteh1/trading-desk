# Trading Desk

A general-purpose, multi-asset trading workspace for watchlists, positions, risk planning, market monitoring and trade review.

## Features
- TradingView ticker tape spanning forex, crypto, US stocks, gold, silver, oil and major indices.
- Interactive TradingView chart with market-class selectors and representative instruments.
- Manual market watchlist with asset classes and price updates.
- Open-position book with entry, stop, target, quantity and estimated planned risk.
- Closed-trade journal with setup, execution grade, notes and CSV export.
- Risk calculator for sizing and illustrative reward/risk target.
- Performance summary: realized P&L, win rate, average win/loss and profit factor.
- Desk notes for session plans and levels.

## Run locally
Open `index.html` in a modern browser. No build step or dependencies are required. The browser must be able to load TradingView's widget scripts.

## Deploy
Import this repository into Vercel. It is a static site; use the repository root as the project root and leave the build command empty.

## Market data notes
- TradingView widgets provide the embedded market data; no API key is required for this widget-based integration.
- Forex and crypto widget data is generally real-time. US stock widgets may be delayed; futures, indices and other instruments vary by exchange, symbol coverage and data entitlements.
- A TradingView paid plan does not automatically remove website-widget exchange delays. Check the instrument's market-status/data notice in TradingView.
- Widgets are display-only. This does not connect a broker, synchronize account positions, provide an execution API, or place orders.
- TradingView's widgets do not expose a general-purpose market-data API for this application to consume.

## Local storage and safety
- Watchlist, positions, journal and notes are stored in browser localStorage on the current device/browser.
- Position sizing is an estimate. Verify contract specifications, pip/point value, lot increments, commissions and slippage for the instrument you trade.
- Do not put API keys, passwords, wallet seed phrases or broker secrets in this repository.
