# Vazcooez — vazcooez.com

Static marketing site for Vazcooez LLC. No build step, no backend.

## Structure

```
.
├── index.html         Home
├── xinbox.html        Product: Xinbox
├── about.html         Company
├── 404.html
├── robots.txt
├── sitemap.xml
├── css/style.css
├── js/main.js         Mobile nav + footer year
└── assets/favicon.svg
```

## Local preview

Any static server works. From this folder:

```powershell
# Python 3
python -m http.server 8080

# Or Node
npx --yes serve -l 8080 .
```

Then open <http://localhost:8080>.

## Deploy

Drop the whole folder onto any static host — Cloudflare Pages, Netlify,
GitHub Pages, S3 + CloudFront, Vercel. No build command required.

If using Cloudflare Pages / Netlify, set the publish directory to the
repo root and leave the build command empty.

## Things to fill in before launch

- [ ] Replace the four `#` placeholders in each footer (X, Facebook, Instagram, YouTube) with real URLs.
- [ ] Add real Open Graph share image at `assets/og.png` (1200×630) and link it from `<meta property="og:image">` on each page.
- [ ] Confirm `leo@vazcooez.com` is the right public contact.
- [ ] If you ship a privacy policy / terms, add `privacy.html` and link from the footer.
