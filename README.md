# SpartansXFinance — Next.js prototype

This is a lightweight Next.js prototype for SpartansXFinance (Zimbabwe). It is a P2P order flow — not a custody or on-site payment processor.

Features
- Homepage with live CoinGecko prices, sparklines, and Buy buttons.
- Buy flow: creates an in-memory order and opens WhatsApp with a prefilled order message so your ops team can complete settlement via Ecocash, Visa, or Mastercard.
- API proxy /api/prices to limit direct client calls to CoinGecko.
- Simple in-memory order endpoint /api/orders (replace with DB for production).
- Spartan helmet brand logo (SVG).
- Contact: WhatsApp +263 78 311 2606, Email SpartansXFinance@gmail.com
- Payments accepted: Ecocash, Visa, Mastercard.

Getting started
1. Install
   - npm install

2. Run dev server
   - npm run dev
   - Open http://localhost:3000

Notes & next steps (production)
- Replace in-memory orders with persistent database (Postgres, MongoDB).
- Integrate payments: Ecocash API or card acquirer (Stripe, local acquirer).
- Implement KYC/AML flows for regulatory compliance.
- Add authentication and admin dashboard to manage orders.
- For real-time Dex-like tracking, integrate DEX APIs or a websocket price feed.
- Use Redis or other caching for API rate-limiting and to avoid CoinGecko rate limits.

Want me to push this to GitHub?
- I can open a PR for you if you give me the repo in owner/repo format, or I can create a zip you can download. Tell me which.
