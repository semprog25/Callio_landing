# Callio Landing Page

Public landing site for **Callio** (missed-call rescue assistant), hosted on GitHub Pages.

**Canonical domain:** [https://trycallio.app/](https://trycallio.app/)

## GitHub Pages

Deployment uses the built-in GitHub Pages publisher (legacy / branch deploy):

- Source: `main` branch
- Folder: `/` (repository root)
- Custom domain file: `CNAME` → `trycallio.app`

There is no GitHub Actions workflow; pushing to `main` publishes the static files at the repo root.

### Custom domain DNS (external)

After the domain is provisioned at your registrar, GitHub Pages expects:

**Apex (`trycallio.app`)** — A records to GitHub Pages:

- `185.199.108.153`
- `185.199.109.153`
- `185.199.110.153`
- `185.199.111.153`

Optional IPv6 AAAA records:

- `2606:50c0:8000::153`
- `2606:50c0:8001::153`
- `2606:50c0:8002::153`
- `2606:50c0:8003::153`

**`www.trycallio.app` (recommended)** — CNAME to:

- `semprog25.github.io`

Then in the repository: Settings → Pages → Custom domain = `trycallio.app`, verify, and enable **Enforce HTTPS** once the certificate is ready.

Do not point the apex CNAME file at anything other than `trycallio.app` (canonical host).

## Contact

- Support: [support@trycallio.app](mailto:support@trycallio.app)
- Privacy / data requests: [privacy@trycallio.app](mailto:privacy@trycallio.app)

## Email waitlist

- Emails are stored in browser `localStorage` (client-side only)
- Admin link is in the footer (subtle)
- Default admin password is in `index.html` — change before relying on it in production

## Files

- `index.html` — landing SPA (home, FAQ, contact, privacy, admin)
- `CNAME` — GitHub Pages custom domain
- `robots.txt` / `sitemap.xml` — SEO
- `README.md` — this file

© 2026 Callio. All rights reserved.
