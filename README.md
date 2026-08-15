# Sprout — Budget & Net Worth Tracker

A playful, full-featured budgeting app demo in the spirit of tools like
Copilot Finance — dashboard, transactions, category budgets, recurring
bill detection, and net worth / spending trend charts. Runs on realistic
sample data rather than a real bank connection.

**Important scope note:** this is a frontend demo. Real bank syncing
(what Copilot Finance actually uses under the hood) requires a secured
backend, a provider like Plaid, encrypted storage, and compliance work —
none of which a static file can do. This app is meant to show the UI/UX
and data-visualization side, with all data held in memory (it resets on
page refresh).

No build tools, no dependencies to install — it's a single HTML file.
Charts are drawn with Chart.js loaded from a CDN.

## Run it

Double-click `index.html`, or open it in any browser.

## Host it live (GitHub Pages)

1. Create a repo (e.g. `sprout-budget`) and upload `index.html` to the
   root.
2. Settings → Pages → Source: Deploy from a branch → `main` / `/ (root)`.
3. Your live URL will be `https://<username>.github.io/sprout-budget/`.

## Features

- **Dashboard** — net worth summary, account balances, this month's
  spending breakdown, recent transactions
- **Transactions** — searchable/filterable list, manual "add transaction"
  form
- **Budgets** — per-category progress bars against monthly targets
  (editable)
- **Recurring** — auto-detected recurring merchants from repeat
  transaction history
- **Trends** — net worth over time and spending-by-category charts

## Tech

Plain HTML/CSS/JS + Chart.js (via CDN). No framework, no build step, no
backend, no external accounts required.
