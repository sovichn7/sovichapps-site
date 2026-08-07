# sovichapps.com (SayWhen legal)

Static Privacy Policy + Terms for App Store Connect.

Source of truth lives in the private `dating_app` repo (`PRIVACY.md` / `TERMS.md` / `apps/mobile/lib/legal-copy.ts`).
Regenerate from that repo: `node scripts/generate-legal-site.mjs`, then copy `site/` here and push.

## Custom domain

GitHub Pages serves this repo. In Cloudflare DNS for `sovichapps.com` (DNS only / grey cloud):

| Type | Name | Content |
|------|------|---------|
| A | `@` | `185.199.108.153` |
| A | `@` | `185.199.109.153` |
| A | `@` | `185.199.110.153` |
| A | `@` | `185.199.111.153` |
| CNAME | `www` | `sovichn7.github.io` |

`www` should 301 to `https://sovichapps.com/` (GitHub Pages does this when both hostnames are configured).

Then in the repo **Settings → Pages → Custom domain**, confirm `sovichapps.com` and enable HTTPS.

## Inbound mail

Public contact addresses are `support@sovichapps.com` and `privacy@sovichapps.com`.
Forward them with Cloudflare Email Routing (or equivalent) to your real inbox — listing the addresses without a forward will bounce mail.
