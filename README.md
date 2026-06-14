# Ledger — Personal Finance Tracker

A private, single-file web app to track your daily spending, income, bank
balances, credit cards, Pay Later dues, and investments. No accounts, no
servers, no tracking — all your data lives only in your own browser.

## Features

- **Daily spend & income** at a glance, plus a 14-day flow chart
- **Net worth** = cash + investments − credit/Pay Later dues
- **Multiple accounts** — bank, credit card, Amazon Pay Later, cash, wallet/UPI
- **Investments** — stocks & mutual funds with units, average cost, live P/L
- **Custom categories** with colours and emojis
- **Import** — paste a bank/UPI SMS or upload a CSV statement to create
  entries in bulk (auto-detects amount, debit/credit, date, merchant)
- **Backup & restore** your data as a JSON file anytime
- Works fully **offline** once loaded; fully responsive on phone and desktop

## Run it

It’s just one file. Either:

- **Open locally:** download `index.html` and double-click it, or
- **Host free on GitHub Pages** (below) so you can open it from any device.

### Deploy to GitHub Pages

1. Create a new repository and add `index.html` (and this README).
1. Go to **Settings → Pages**.
1. Under *Build and deployment*, set **Source: Deploy from a branch**,
   pick `main` and `/ (root)`, then **Save**.
1. Wait a minute — your app is live at
   `https://<your-username>.github.io/<repo-name>/`.

## Your data & privacy

Everything is stored in your browser’s local storage on the device you use.
It is never uploaded anywhere. Two things to remember:

- Clearing your browser data (or using a different device/browser) means a
  fresh, empty app — so **download a backup regularly** from the top bar.
- To move to a new device, download the backup on the old one and use
  **Restore** on the new one.

## About “automatic” tracking

Browsers don’t let any website silently read your phone’s SMS or open your
PDF invoices — that’s a privacy protection, not a bug. The practical private
workflow built in here is:

- **Paste an SMS** alert → it reads the amount and direction → you confirm.
- **Upload a CSV** statement from your bank → bulk-import all rows.
- For a PDF invoice, copy its total into the SMS box, or add it manually.

If you ever want true background SMS capture, that requires a native phone app
with explicit SMS permissions — out of scope for a browser app, by design.

## Tech

Plain HTML, CSS, and vanilla JavaScript in one file. No build step, no
dependencies (fonts load from Google Fonts; the app works without them too).

## License

MIT — do whatever you like with it.