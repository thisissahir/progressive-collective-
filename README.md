# Progressive Collective — Website

Static website for **Progressive Collective**, migrated from Wix to a static build hosted on **Vercel**. Domain registered at Hostinger (`progressivecollective.in`).

## Stack
- Plain HTML + CSS (no build step). Deploys instantly on Vercel as a static site.
- Fonts: Fraunces (display) + Inter (body) + Space Mono (labels) via Google Fonts.
- Media (images) served from the existing Wix CDN (`static.wixstatic.com`). Audio/video embeds from Spotify, YouTube, Vimeo, SoundCloud.

## Pages
| File | Route |
|------|-------|
| `index.html` | `/` |
| `portfolio.html` | `/portfolio` (old Wix `/artists-1` redirects here) |
| `ecosystem.html` | `/ecosystem` (old Wix `/blank-1` redirects here) |
| `contact.html` | `/contact` |
| `privacy.html` | `/privacy` (old `/privacy-policy` redirects here) |
| `terms.html` | `/terms` (old `/terms-and-conditions` redirects here) |
| `404.html` | custom not-found |

`vercel.json` handles clean URLs and redirects from the old Wix paths so existing links/SEO don't break.

## Deploy
Connected to Vercel. Pushing to `main` on GitHub triggers an automatic deploy.

## TODO / nice-to-have
- Self-host images instead of hotlinking the Wix CDN (download assets into `/assets`).
- Wire the contact form to a real backend (Formspree / Web3Forms) instead of the `mailto:` fallback.
- Add the **Collective Signal** (web / SEO / GEO / AI) services section when ready.
