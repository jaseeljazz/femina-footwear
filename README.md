# FEMINIA_FL36 — complete static storefront

## Run
Extract the ZIP, keep the files together, then open index.html. Internet access is required for Bootstrap, icons, Google Fonts and Unsplash photos. For consistent cart storage across pages, serve the folder using any static web server (VS Code Live Server, or `python -m http.server 8000` if Python is installed), then visit http://localhost:8000.

## Pages
- index.html — home, collections, story, contact
- products.html — category filtering, search, sorting, wishlist
- product.html?id=1 — details, EU size selection, quantity, related products
- cart.html — per-size bag, quantity changes, removal, totals
- checkout.html — validated Indian delivery details, demo payment selection
- order-success.html — latest demo order receipt, print/save PDF
- assets/style.css — shared responsive design
- assets/app.js — catalog and all shared interactions

## Demo boundaries
All prices, stock, product descriptions, size availability, and delivery fees are illustrative. Stock photographs are styling references, not verified product inventory. Photo references are repeated across demo variants. Confirm contact/social details before publication. Checkout never takes payment, sends an order, or promises real delivery. Newsletter is not connected. Cart and wishlist use browser localStorage, with a sessionStorage fallback; customer details and the latest demo order use sessionStorage only. Address details are not sent over the network by the application. The checkout warns if browser storage is blocked. No passwords or payment credentials are requested.

## Connect for live commerce
Replace the catalog with real products and licensed product photos, fetch and validate inventory/prices on a server, calculate shipping/tax there, create orders in a database, integrate a payment provider with verified server webhooks, implement email confirmations, publish store-approved returns/privacy/terms policies, and connect the newsletter provider. Do not use browser totals as authoritative prices.

## Editing
Change PRODUCTS near the start of assets/app.js. Change shared header/footer there. Styling lives in assets/style.css. There are no build tools or npm dependencies. Shipping demo rule: free from ₹2,999; otherwise ₹99. EU sizes: 36–41. Demo quantities: 1–10 per size.
