# Callio Landing Page

Public landing site for **Callio** — your missed-call rescue assistant.

**Canonical domain:** [https://trycallio.app/](https://trycallio.app/)

## Positioning

> Missed a call? Find out why they called.

Callio helps people recover the context behind missed calls from unknown numbers — without blindly calling back.

## GitHub Pages

- Source: `main` branch
- Folder: `/` (repository root)
- Custom domain: `CNAME` → `trycallio.app`

### DNS (apex)

A records to GitHub Pages:

- `185.199.108.153`
- `185.199.109.153`
- `185.199.110.153`
- `185.199.111.153`

Optional www CNAME → `semprog25.github.io`

Enable **Enforce HTTPS** after the certificate is ready.

## Local preview

```bash
cd Callio_landing
python3 -m http.server 8765
# open http://127.0.0.1:8765/
```

## Files

- `index.html` — marketing site (home, guides, FAQ, privacy, contact, waitlist admin)
- `assets/mascot/` — transparent Callio mascot assets
- `CNAME` — GitHub Pages custom domain
- `robots.txt` / `sitemap.xml` / `site.webmanifest` — SEO + PWA metadata

## Contact

- Support: [support@trycallio.app](mailto:support@trycallio.app)
- Privacy: [privacy@trycallio.app](mailto:privacy@trycallio.app)

## Waitlist

Emails are stored in browser `localStorage` (client-side only). Admin is linked subtly in the footer.

© 2026 Callio. All rights reserved.
