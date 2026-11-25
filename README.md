# Levuche design

Design source for Levuche, a site builder for creators. A creator claims `handle.levuche.page`, picks a layout, sets their brand, and sells or showcases packs from their social accounts. The marketing site is levuche.com.

Levuche is its own product, a Jagodana product. It uses BuildBase as a third-party service for products, checkout, files and some account screens. Where a board says "Opens BuildBase", that screen belongs to the third-party service and is not redesigned here.

## What's here

```
canvas/            Every artboard from the Levuche design canvas, plus its index
  canvas.json      Board positions, titles, pages and notes
  *.dc.html        One artboard each, in light and dark
tokens/
  levuche-tokens.css   Design tokens v1.0 (--lv-* for product UI, --site-* for creator sites)
```

The `.dc.html` files are design-canvas artboards. They load `./support.js` and a stylesheet at `/_blob/16490de4fd085992f4b80feb1a7e5129`, which the canvas serves; that stylesheet is the same file as `tokens/levuche-tokens.css`.

## Boards by page

| Page | Boards |
| --- | --- |
| 0 · Tokens | Brand |
| 1–4 · System | Atoms, Molecules, Organisms, Templates |
| Marketing site | MarketingDesktop, MarketingTablet, MarketingPhone, MarketingPages (pricing, legal and security layout) |
| Dashboard | DashboardDesktop/Tablet/Phone, InboxDesktop/Tablet/Phone, OnboardingFlow, SettingsFlow (pages, brand and theme, handle and domain, short link, API keys, empty states) |
| Editor | EditorDesktop/Tablet/Phone, EditorStates (phone editor sheets, insert tabs, publish error, unsaved changes, rollback) |
| Creator site | SiteDesktop/Tablet/Phone, PackDesktop/Tablet/Phone, SitePagesFlow (video, contact sent and error, document, order and download, 404, removed, suspended, report) |
| Source pages | Main, Dashboard, Inbox, Editor, SiteHome, Pack (the components the device boards import) |

## Design rules

- Font: Sora. Wordmark is always lowercase `levuche`.
- Product screens use only `--lv-*` tokens; creator sites use only `--site-*` tokens, set from the creator's own brand. The sample brand on the boards is "Desi Origins".
- Every screen ships in light and dark.
- Touch targets are at least 44 px. Icon-only buttons carry an accessible label.
- Prices, fees, legal text, security contacts, DNS targets and keys are placeholders in `[BRACKETS]`. Nothing in these boards is final copy or real data.
