# CampusCash — Student Finance Companion

A working mobile-first student finance PWA built with plain HTML, CSS and JavaScript so it can run without a build system, API key or paid service.

## Features
- Add real income and expense transactions.
- Browser persistence using localStorage.
- Monthly balance, income, expenses and budget tracking.
- Spending breakdown by category.
- Money-coach suggestions generated from the user's actual logged activity.
- 60+ ISO currency codes with locale-aware formatting through `Intl.NumberFormat`.
- No pre-seeded fake transactions or fake bank balances.
- Responsive mobile-first UI with installable PWA manifest.
- Delete individual transactions and clear local data.

## Run
The simplest option is to open `index.html` in a browser.

For PWA/service-worker-style browser behavior, serve the folder with any static server, for example:

```bash
python -m http.server 8080
```

Then open `http://localhost:8080`.

## Data behavior
The app intentionally does not invent bank balances, exchange rates, transactions, or financial activity. Currency selection changes display context; it does not pretend to convert money using an unverified exchange-rate feed.

All current data stays in the user's browser. A production version can add authenticated cloud sync and a verified FX provider without changing the core UI model.
