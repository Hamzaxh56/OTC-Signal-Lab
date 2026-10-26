# Quotex Signal Analyzer AI — Market Companion

Responsive static website prototype for analyzing supported public crypto candles and tracking signal outcomes.

## Added in this version
- Market-category selector: Currencies, Crypto, Commodities, Stocks
- Currency list includes pairs shown in the supplied Quotex screenshots, including the visible OTC pairs
- Separate chart-timeframe selector (1m through 24h) and signal-expiry selector (0.5 seconds through 24 hours)
- Candlestick and Heikin Ashi views
- EMA 9/21, RSI 14, MACD, ATR and indicator-confluence scoring
- CALL / PUT / WAIT with adjustable score threshold
- Local signal history and win/loss percentages for settled signals
- Unsupported markets show WAIT / no live feed rather than generating fabricated prices or signals

## Run locally
Open `index.html` in a modern browser with internet access.

## Deploy to Render
1. Upload this folder to a GitHub repository.
2. In Render, choose **New + → Static Site** and connect the repository.
3. Leave Build Command blank and set Publish Directory to `.`.
4. Deploy.

## Important limitations
- Live candles currently come from the public Binance spot API for supported crypto/USDT pairs only.
- The currency, OTC, commodities and stock lists are selectable catalog entries; they do not imply a live feed is available for those instruments. Unsupported instruments are deliberately blocked from signal generation.
- Quotex OTC prices are broker-specific. A real OTC analyzer needs an authorized compatible feed; unrelated market prices must not be substituted.
- Expiry options from 0.5 seconds to 24 hours are available in the interface, but this candle feed cannot reliably validate sub-minute expiry results. Select a supported feed and treat results as estimates only.
- This site does not connect to a Quotex account or place trades. The 0–100 score is indicator agreement, not a calibrated probability; no 90% win rate is promised.
- Win/loss rates are computed from recorded and settled local signals only. Results may differ from broker execution, entry prices, payout rules and expiry prices.
