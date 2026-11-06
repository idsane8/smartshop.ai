# SmartShop AI — Version 0.1

A mobile-first UK shopping comparison dashboard. Static HTML/CSS/JavaScript, no build tools or paid hosting required.

## Deploy to GitHub Pages
1. On GitHub, create a **new public repository** named `smartshop-ai`. Do not commit sensitive data.
2. Upload `index.html`, `app.js`, `manifest.webmanifest` to the repository root (and README.md if wanted).
3. Go to **Settings → Pages → Build and deployment → Deploy from a branch**. Select `main` and `/ (root)`, then save.
4. Visit `https://YOUR-USERNAME.github.io/smartshop-ai/` on iPhone Safari; Share → Add to Home Screen.

## Features
- UK retailer search shortcuts for teen girls', men's, women's and household categories.
- Copy ready-to-paste ChatGPT prompts requesting real price checks.
- Enter observed items with page URL, price, delivery, materials, reviews, date and returns evidence.
- Calculates indicative evidence-aware scores and records comparison groups.
- Locally stored watchlist targets, export/import of records.
- No payment flow and no purchases.

## Real limitations
- This static app **does not retrieve live retailer prices**, guarantee stock, or fetch product quality tests.
- A saved watch target is **not** a background price-tracking service.
- The separate ChatGPT SmartShop Deal Watch automation sends alerts but is not technically connected to this app's local storage.
- Scoring is heuristic, not a proof of durability or independently established quality.
- Retailer search URLs are shortcuts; retailers may change their website search structure.
- To achieve synced automatic app-level price history, build a backend with approved retailer data feeds/APIs, a database, and consent-based notification infrastructure. Avoid unauthorised scraping or circumvention of retailer restrictions.

## Security
No login, no personal information collection, no payment features. Saved items use `localStorage` on the current browser only. Data is not encrypted; do not save personal secrets. Only HTTPS product URLs accepted. All injected text is HTML-escaped. External links open separately.

## Next milestones
1. Verify mobile deployment; test adding a real listing.
2. Add a managed database and access control.
3. Integrate compliant product APIs and price history.
4. Add synced deal alerts and matching algorithms.
5. Audit sourcing, returns, data retention and notification accuracy.
