# sovichapps.com (SayWhen legal)

Static Privacy Policy + Terms for App Store Connect.

**Live:** https://sovichapps.com/privacy/ · https://sovichapps.com/terms/

Source of truth is the private `dating_app` repo (`PRIVACY.md` / `TERMS.md` / `apps/mobile/lib/legal-copy.ts`).  
Ops write-up: `dating_app` → [SETUP.md §4b](https://github.com/sovichn7/dating_app/blob/main/SETUP.md) (path may differ by branch).

Regenerate from `dating_app`: `pnpm legal-site`, then copy `site/` into this repo and push.

## Custom domain (Cloudflare → GitHub Pages)

DNS only / grey cloud on Cloudflare for `sovichapps.com`:

| Type | Name | Content |
|------|------|---------|
| A | `@` | `185.199.108.153` |
| A | `@` | `185.199.109.153` |
| A | `@` | `185.199.110.153` |
| A | `@` | `185.199.111.153` |
| CNAME | `www` | `sovichn7.github.io` |

Repo **Settings → Pages** → custom domain `sovichapps.com` + Enforce HTTPS.
