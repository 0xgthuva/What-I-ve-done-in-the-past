# Thuvaragan Gobalakrishnan — Portfolio

> 6+ Years in Digital Marketing. Accidental Strategist | Generalist | Hustler + Hacker + Hipster

## About

Personal portfolio site for **Thuvaragan Gobalakrishnan**, Manager of Digital Marketing (Cluster) at Pulse Hotels & Resorts, based in Malé, Maldives. The site showcases previous work across Performance Marketing, SEO / GEO / Growth Marketing, and a career timeline — all in a single responsive page.

## Live Site

```
https://YOUR-DOMAIN.com
```

> Replace `YOUR-DOMAIN.com` with your actual domain everywhere in this repo before deploying. See the [Deployment](#deployment) section below.

## Tech Stack

- **Pure HTML / CSS / JS** — no frameworks, no build step, no dependencies
- **Fonts** — GeistSans, GeistMono, ClashDisplay loaded from the local `fonts/` folder
- **Charts** — Canvas-based (LinkedIn career area chart, GitHub contribution graph), drawn with vanilla JS and `ResizeObserver` for fluid resizing
- **Network graph** — Inline SVG with `viewBox` for automatic scaling
- **Responsive** — Four breakpoints: 480 px, 700 px, 900 px, 1200 px+

## Project Structure

```
.
├── index.html       Main portfolio page (HTML + CSS + JS, single file)
├── robots.txt       Crawler directives + sitemap reference
├── sitemap.xml      XML sitemap for search engines
├── fonts/           Local webfont files (.woff2)
├── images/          Local images (avatar, background tile)
└── README.md        This file
```

## Deployment

1. **Upload** all files (keeping the directory structure intact) to your web host, CDN, or static hosting service (Netlify, Vercel, GitHub Pages, Cloudflare Pages, etc.).

2. **Find-and-replace** `YOUR-DOMAIN.com` across these files:

   | File | Where |
   |---|---|
   | `index.html` | `og:url`, `og:image`, `twitter:image`, `canonical` `<link>`, JSON-LD `url` + `sameAs` |
   | `robots.txt` | `Sitemap:` directive at the bottom |
   | `sitemap.xml` | `<loc>` tag |

3. **Fill in remaining placeholders** in `index.html`:
   - `REPLACE_WITH_LINKEDIN_HANDLE` → your LinkedIn profile slug (e.g. `thuvaragan-g`)
   - `og:image` / `twitter:image` → full URL of your hosted OG cover image (recommended size: 1200 × 630 px)

4. **Uncomment the SEO block** in `index.html` — it sits between the `<!-- ═══ SEO META TAGS ═══ -->` delimiters in `<head>`. Remove the outer comment wrappers once you have real values.

5. **Submit your sitemap** to Google Search Console:
   `https://search.google.com/search-console` → Sitemaps → Add `https://YOUR-DOMAIN.com/sitemap.xml`

6. **Verify robots.txt** is reachable at `https://YOUR-DOMAIN.com/robots.txt` and test it in the [Google Search Console robots.txt tester](https://search.google.com/search-console/robots-testing-tool).

## SEO

The `<head>` of `index.html` contains a clearly marked placeholder block with templates for:

| Tag type | Purpose |
|---|---|
| **Open Graph** | Rich link previews on LinkedIn, Facebook, WhatsApp, Slack |
| **Twitter / X Card** | `summary_large_image` card on Twitter / X |
| **Schema.org JSON-LD** | `Person` structured data for Google Knowledge Panel eligibility |
| **Canonical URL** | Prevents duplicate-content issues if the site is mirrored |
| **robots meta** | `index, follow` — tells crawlers to index and follow all links |

`robots.txt` and `sitemap.xml` are ready to serve once the domain placeholder is replaced.

## Social Profiles

| Platform | Handle / Link |
|---|---|
| GitHub | [github.com/0xgthuva](https://github.com/0xgthuva) |
| Twitter / X | [@0xgthuvaDEV](https://twitter.com/0xgthuvaDEV) |
| Spotify | [open.spotify.com/user/31trew…](https://open.spotify.com/user/31trewszrbvsnstny2hjubyiilp4) |
| Email | gthuva@yahoo.com |

## License

All rights reserved. &copy; Thuvaragan Gobalakrishnan. Do not reproduce or redistribute without permission.
