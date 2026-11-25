# levuche.com rollout checklist

Use this when putting the brand kit live. Tick each line on every site and app surface (marketing site, app, creator pages on levuche.page, emails, app stores, social profiles).

## Domains

- [x] levuche.com bought (main site, app, contact addresses)
- [x] levuche.page bought (creator storefronts, e.g. yourname.levuche.page)
- [ ] Turn on auto-renew and registrar lock for both
- [ ] Redirect www.levuche.com to levuche.com (or the reverse), one choice only, with a 301
- [ ] Redirect any older domains to the matching levuche.com page with a 301

## Canonical links and URLs

- [ ] Every page has `<link rel="canonical" href="https://levuche.com/...">` with https and the chosen host
- [ ] Creator pages use their own levuche.page address as canonical, not levuche.com
- [ ] No canonical, hreflang or og:url still points to a staging host, old domain or BuildBase address

## Sitemap and robots

- [ ] `https://levuche.com/sitemap.xml` lists only levuche.com URLs
- [ ] `https://levuche.com/robots.txt` has `Sitemap: https://levuche.com/sitemap.xml`
- [ ] Staging and preview sites are set to noindex
- [ ] Add levuche.com (and levuche.page) in Google Search Console and Bing Webmaster Tools; submit the sitemap

## Metadata

- [ ] `<title>` pattern: `Page name | Levuche`
- [ ] Meta description on every public page
- [ ] Favicons: copy `favicon/` to the site root and paste `favicon/head-snippet.html` into `<head>`
- [ ] `site.webmanifest` name "Levuche", theme colour #24257A

## Share images (Open Graph and Twitter/X)

- [ ] `og:image` = `social/levuche-og-1200x630.png` (absolute https URL on levuche.com)
- [ ] `og:site_name` = Levuche, `og:url` = the canonical URL
- [ ] `twitter:card` = summary_large_image, same image
- [ ] Profile pictures on social accounts: `social/levuche-avatar-400.png`
- [ ] Test with a link preview tool after deploy

## Structured data (JSON-LD on the home page)

```json
{
  "@context": "https://schema.org",
  "@type": "Organization",
  "name": "Levuche",
  "url": "https://levuche.com",
  "logo": "https://levuche.com/levuche-icon-512.png",
  "parentOrganization": {
    "@type": "Organization",
    "name": "Jagodana LLC",
    "url": "https://jagodana.com",
    "founder": { "@type": "Person", "name": "Dharmendra Jagodana" }
  }
}
```

- [ ] Add `sameAs` with the official social profile URLs once claimed

## Contact addresses

- [ ] All public addresses use @levuche.com (for example hello@, support@, privacy@, security@, legal@)
- [ ] Set up those mailboxes or forwards before publishing them
- [ ] Fill the canvas placeholders: [SECURITY CONTACT] and [Privacy contact and company address.] on the legal pages
- [ ] SPF, DKIM and DMARC records for levuche.com so emails don't land in spam
- [ ] `https://levuche.com/.well-known/security.txt` with the security contact

## Ownership and legal lines

- [ ] Footer: "© 2026 Jagodana LLC. Levuche is a product managed by Jagodana LLC." (link Jagodana LLC to jagodana.com)
- [ ] About page: "Levuche was founded by Dharmendra Jagodana and is managed by Jagodana LLC."
- [ ] Terms and Privacy name Jagodana LLC as the operating company
- [ ] App store listings: seller or developer shown as Jagodana LLC
- [ ] Use ™ after the name or logo if wanted; ® only after registration

## "Formerly" line (only where it helps)

- [ ] About page: "Levuche (formerly [OLD NAME]) ..."
- [ ] Press or media page: one line in the boilerplate
- [ ] Optional: footer for the first few months only, then remove
- [ ] Not in titles, meta descriptions, ads, app name, logo or share images
- [ ] Old-name search terms land on the About page via redirects, not keyword stuffing

## Leftover sweep

- [ ] Search code, content, emails and templates for the old name, "BuildBase", old domains and old logos
- [ ] Check email footers, PDF invoices, notification templates, app store screenshots and social bios
- [ ] Check alt text and file names of images
- [ ] Replace any hard-coded colours with the brand tokens (see `guide/`)

## After launch

- [ ] Claim @levuche on Instagram, X, TikTok, YouTube, LinkedIn and Facebook
- [ ] Have a trademark lawyer run a full India and US search and file
