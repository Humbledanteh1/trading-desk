# Trading Desk

A browser-based funded-account command center for manual tracking.

## Current features
- Account settings: starting balance, equity, drawdown floor, profit target, payout cap and consistency limit.
- Consistency monitor: best positive day divided by total net journal profit.
- Daily P&L journal with local browser persistence and CSV export.
- Drawdown buffer monitor.
- Risk and estimated position-size calculator.
- Payout-readiness checklist.

## Run locally
Open `index.html` in a modern browser. No build step or dependencies are required.

## Deploy
Import this repository into Vercel. It is a static site; use the repository root as the project root and leave the build command empty. Vercel will serve `index.html`.

## Important limitations
- This is a manual tracking and planning tool. It does not connect to a broker, prop firm, exchange, or trading account.
- Journal and settings are stored in the browser's localStorage on that device/browser. They are not synced to a server.
- The consistency calculation uses best positive day / total net journal profit. Prop-firm definitions vary; verify the official rule, payout eligibility, drawdown model, trading-day minimums and risk limits with your provider.
- Position sizing is an estimate. Confirm instrument contract specifications, pip/point value, commissions, slippage and lot constraints before trading.
- No trade execution or automated order placement is included.

## Next step
Choose the intended platform (for example MT5, cTrader, MatchTrader or Hyperliquid) before adding any account-data integration. Keep integrations read-only first and never commit API secrets to the repository.
