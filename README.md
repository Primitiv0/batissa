# Uniformes Batissa — sitio web

Temporary/primary website for Uniformes Batissa, served via GitHub Pages on
**batissa.com**. Single-page, no build step, no dependencies beyond Google Fonts.

Pioneers in manufacturing and selling uniforms in the Dominican Republic since 1970
(BATISSA = **Bat**as + **Issa**).

## Files
- `index.html` — the whole site (HTML, CSS, JS inline)
- `images/logo.png` — official Batissa logo (UB monogram + UNIFORMES + Batissa wordmark)
- `images/logo-white.png` — white (knockout) version for dark backgrounds (footer)
- `images/favicon.png` — UB monogram favicon

## Brand palette (from the official logo)
- Batissa blue `#0096C7` (primary) · deep blue `#0077B6` · bright cyan `#00B8D8`
- Batissa orange `#F88018` (accent) · deep orange `#F87800`
- background `#F2FAFD` · text `#0C2230`
- `CNAME` — custom domain (batissa.com)

## Bilingual (ES / EN)
Spanish is the default; the EN/ES button in the nav switches everything instantly
(no reload). All copy lives in the `DICT` object near the bottom of `index.html`,
plus `[data-i18n]` / `[data-i18n-html]` tags for static text. Category, service and
location cards are rendered from the same dictionary.

## WhatsApp
Every "Cotiza / Quote" button opens a WhatsApp chat. The number is set once at the
top of the script:

    const WA_NUMBER = "18096864043";  // (809) 686-4043

Change this single line if a different WhatsApp business line should be used.

## To update later
- Phone/emails: footer + `WA_NUMBER` + `locs` arrays in both languages.
- Add a product category: append to the `cats` array in both `es` and `en`.
