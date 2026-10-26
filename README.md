# Quotex Signal Analyzer — Render-ready static site

## Deploy on Render

1. Extract this ZIP on your device.
2. Upload **the contents of this folder** to the root of a new GitHub repository. `index.html`, `render.yaml`, and `README.md` must be directly in the repository root, not inside another nested folder.
3. In Render, choose **New + → Static Site** and connect that GitHub repository.
4. Set **Build Command** to blank (or `echo static site`) and **Publish Directory** to `.`.
5. Click **Create Static Site** / **Deploy**.

If the Render site already exists, push these root-level files to the connected repository and trigger **Manual Deploy → Deploy latest commit**.

## Important data limitations

This is a static website. Supported crypto pairs use Binance public candles. The listed forex/OTC, stock and commodity entries are catalog choices only unless a compatible live data provider is configured; the analyzer intentionally disables signals for unsupported feeds. It does not connect to a Quotex account. A 90+ score is an indicator-confluence score, not a verified 90% win probability. Local signal history is stored in the browser and may not sync between devices.
