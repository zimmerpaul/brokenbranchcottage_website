# Broken Branch Cottage

Static marketing site for brokenbranchcottage.com, served by GitHub Pages. No build step.

- `index.html`, `styles.css`, `favicon.svg`
- `images/` — web-sized photos (800w / 1600w), metadata stripped
- `CNAME` — custom domain

## To do
- Replace the two `https://www.airbnb.com/` links in `index.html` (search for `AIRBNB:`) with the listing URL.

## GitHub Pages + domain
1. Repo → Settings → Pages → Source: Deploy from branch, `main`, `/ (root)`.
2. Custom domain: `brokenbranchcottage.com`, then tick "Enforce HTTPS" once the certificate is issued.
3. DNS at the registrar:
   - Apex `A` records: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `AAAA` (optional): `2606:50c0:8000::153`, `2606:50c0:8001::153`, `2606:50c0:8002::153`, `2606:50c0:8003::153`
   - `CNAME` `www` → `zimmerpaul.github.io`
