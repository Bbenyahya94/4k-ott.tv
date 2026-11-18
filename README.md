# 4K OTT / ProMax IPTV website

This is a static, four-language website for `4k-ott.tv`.

- English: `/en/`
- German: `/de/`
- French: `/fr/`
- Simplified Chinese: `/cn/`

Each language has its own pricing, reseller, apps, guides, blog, contact, about, privacy, refund and DMCA pages. The root URL sends visitors to English. Prices are set to €12, €25, €35, €55 and €99 for 1, 3, 6, 12 and 24 months respectively.

## Deploy with Coolify

Upload the files at the root of a GitHub repository, including `Dockerfile`, `nginx.conf` and the entire `dist` folder. Deploy the repository as a Dockerfile application. Point `4k-ott.tv` to that application. Submit `https://4k-ott.tv/sitemap.xml` to Google Search Console once the domain is live.

To regenerate the localized HTML after editing translations or pricing in `build-pages.js`, run `node build-pages.js` and deploy the updated `dist` folder.

## Confirm before launch

The site currently uses the previously provided WhatsApp, Telegram, support email, Google Analytics ID and Google verification tag. Confirm they are also intended for `4k-ott.tv`; a Search Console tag from another property may not verify this new domain. Confirm subscription and reseller terms before making the site public.
