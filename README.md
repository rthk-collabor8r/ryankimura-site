# ryankimura.com

A single static page: `index.html` with its CSS and JavaScript inline, plus an `images/` folder. No build step and no dependencies.

## Files

| File | What it is |
|---|---|
| `index.html` | The whole site |
| `images/` | Web-sized photos and artifacts (about 1.8 MB total) |
| `favicon.ico`, `favicon.png`, `apple-touch-icon.png` | Browser and phone icons (the three banner shapes on navy) |
| `og-image.png` | The preview image when the link is shared (your LinkedIn banner) |
| `robots.txt`, `sitemap.xml` | For search engines |

## Preview locally

Open `index.html` in a browser. Everything works except the contact form, which needs the step below.

## Go live

**Vercel (simplest).** Sign in at vercel.com with GitHub, choose "Add New Project," import `ryankimura-site`, and deploy with the defaults (framework: Other, no build command). Then go to Settings, Domains, add `ryankimura.com`, and follow the DNS instructions it shows. Every push to `main` redeploys.

**GitHub Pages (alternative).** In the repo, open Settings, Pages, and set the source to the `main` branch, root folder. Add a file named `CNAME` containing `ryankimura.com`, then point your domain's DNS at GitHub Pages.

Either way, if the domain is currently on Squarespace, you move the DNS records there; you don't need to transfer the domain.

## Contact form

The form posts to Formspree (`https://formspree.io/f/xljbnazy`), which forwards messages to your inbox so your address never appears on the page. A hidden honeypot field filters bots, and Formspree filters spam on its side.

## Still to add

- HandCut photos
- Quotes in "In their words" are condensed and unnamed; swap in named ones as you get permission
