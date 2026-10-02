# Ember – Chat Trading Agent

Static app (no build step). Orange/black UI. Wallet connect (Sphere Connect) → confirm → chat commands + portfolio.

## Deploy (phone only)
1. GitHub app/website → New repository → Add file → Upload files: `index.html`, `vercel.json`, `README.md`.
2. vercel.com → Add New Project → import the repo → Framework: Other → Deploy.

## Commands
`swap 10 uct to solana`, `swap 1 sol to uct`, `bridge 5 uct to bitcoin`, `swap 10 uct to solana or bitcoin`, `portfolio`

## Notes
- Prices are demo values in `PRICES`; swap in a live feed.
- Real mode sends a `transfer` intent through Sphere Connect; routing to Solana/Bitcoin needs your own swap/bridge backend.
- Never retry on error code 4201 (outcome unknown).
