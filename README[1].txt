# Lumber River Native Plants — Upload Pack

This is a turnkey static site ready for Netlify.

## How to deploy
1. Put these files at the **repo root** (same level as `index.html`).
2. In Netlify **Site settings → Build & deploy**:
   - Base directory: *(leave blank)*
   - Build command: *(leave blank)*
   - Publish directory: `.`
3. **Deploy → Clear cache and deploy site**.

## Where to place your real photos
Put images here and reference them as `/public/img/<name>`:

```
/public/img/
  hero.jpg      # homepage banner
  logo.png      # small square logo
  nursery.jpg   # optional content image
  lilies.jpg    # optional content image
```

## DNS (GoDaddy → Netlify)
Create these DNS records at GoDaddy for `lumberrivernativeplants.online`:

- A @ 75.2.60.5  (TTL 600)
- A @ 99.83.190.102 (TTL 600)
- CNAME www → lumberrivernativeplants.online (TTL 1 hour)

Then in Netlify: **Domain Management → Verify DNS → Set as primary → Enable SSL**.

Generated 2025-10-16.
