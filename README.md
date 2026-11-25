# Levuche design

Design source for Levuche, a site builder for creators. A creator claims `handle.levuche.page`, picks a layout, sets their brand, and sells or showcases packs from their social accounts. The marketing site is levuche.com.

Levuche is a product managed by Jagodana LLC ([jagodana.com](https://jagodana.com)), founded by Dharmendra Jagodana.

Levuche is its own product, separate from BuildBase. It uses BuildBase as a third-party service for products, checkout, files and some account screens. Where a board says "Opens BuildBase", that screen belongs to the third-party service and is not redesigned here.

## What's here

```
canvas/            Every artboard from the Levuche design canvas, plus its index
  canvas.json      Board positions, titles, pages and notes
  *.dc.html        One artboard each, in light and dark
tokens/
  levuche-tokens.css   Design tokens v1.1 (--lv-* for product UI, --site-* for creator sites)
brand/             Brand kit: logo, favicon set, social images, brand guide,
                   Sora font files and the levuche.com rollout checklist
```

The `.dc.html` files are design-canvas artboards. They load `./support.js` and a stylesheet at `/_blob/4d3230c7f0c56e1f37d88a4aaef2bc1b`, which the canvas serves; that stylesheet is the same file as `tokens/levuche-tokens.css`.

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

## Help and feedback

- Questions and ideas: [Discussions](https://github.com/Levuche/design/discussions)
- Something wrong in a board or the tokens: [Issues](https://github.com/Levuche/design/issues/new/choose)
- Security problems: privately, see [SECURITY.md](SECURITY.md)
- Your own account, an order or a payout: [levuche.com/contact](https://levuche.com/contact)

How issues are handled and how the team works: [CONTRIBUTING.md](CONTRIBUTING.md).

## License and ownership

Everything in this repository belongs to Jagodana LLC. It's public so you can see it, not so you can reuse it. You may not copy, modify, redistribute, use commercially or use as AI training data any part of it without written permission. See [LICENSE](LICENSE).

Levuche™ and the Levuche logo are trademarks of Jagodana LLC. See [TRADEMARKS.md](TRADEMARKS.md).

The Sora font files in `brand/fonts/` are third-party and stay under the SIL Open Font License 1.1 ([brand/fonts/OFL.txt](brand/fonts/OFL.txt)).

For permission, contact Jagodana LLC through [jagodana.com](https://jagodana.com).

© 2026 Jagodana LLC. All rights reserved.
