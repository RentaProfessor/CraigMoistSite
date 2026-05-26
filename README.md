# 🌱 PlantWatch — Web Dashboard

Static PWA for the PlantWatch garden moisture system. Calls the
Supabase edge function and renders per-plant moisture, status, and
watering advice.

## Hosted on Cloudflare Pages

This repo is the dashboard only. The root of the repo IS the site
(no build step). Cloudflare Pages config:

- **Build command:** *(none)*
- **Build output directory:** *(leave blank — the root)*
- **Root directory:** *(blank)*

Push to `main` → Cloudflare deploys.

## Backend

The edge function and iOS app live in a separate repo:
<https://github.com/RentaProfessor/Craigmosit>

The endpoint this site calls is hard-coded in `config.js`. It's
public by design (single trusted audience, `verify_jwt = false`).

## Install on iPad

Open the deployed Pages URL in Safari → share → **Add to Home Screen**.
The icon launches the dashboard full-screen, like a native app.
