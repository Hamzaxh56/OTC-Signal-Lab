SIGNAL LAB LITE — ANDROID-FRIENDLY SETUP

WHAT THIS IS
- A simple static website (one index.html file).
- TradingView embedded chart.
- Analyze Signal button using Twelve Data OHLC candles and EMA/RSI rules.
- No Render build command or Python backend is required.
- No guaranteed win rate. The signal rule is educational, not financial advice.

EASIEST WAY TO PUT IT ONLINE
1. Open https://github.com and sign in.
2. Create a NEW repository named quotex-signal-lite.
3. Choose Public (or Private if you understand GitHub Pages access limitations).
4. Tap Add file -> Upload files.
5. Upload index.html directly (not inside another folder).
6. Tap Commit changes.
7. Open repository Settings -> Pages.
8. Under Build and deployment, choose Deploy from a branch.
9. Select branch main and folder /(root), then Save.
10. Wait a few minutes. The Pages section shows your website URL.

API KEY
- Get your own Twelve Data API key from https://twelvedata.com/
- Enter it into the page when you want to analyze. The page does not save it.
- WARNING: A browser-based page cannot keep an API key secret from visitors. Do not use this approach for a public commercial service. For public use, use a backend proxy.
- Availability and quotas depend on the data provider's plan.

If the page opens but analysis fails, read the error shown under Analyze Signal.
