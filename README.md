# cuffscan.com
The public website for CuffScan.

Plain static HTML and CSS, no build step. Pages:
- `index.html` landing page
- `privacy/` privacy policy (keep in step with the app's About/Help wording)
- `support/` FAQ and contact (hello@cuffscan.com)
- `404.html`, `robots.txt`, `sitemap.xml`, `assets/`

Preview locally: `npx serve .`.

Deploy: any static host (for example Cloudflare Pages with no build command and output directory `/`).
Mail DNS records live in the app repo under `dns/`.

TODO when the app ships: add the App Store link and badge on the landing page. If the contribute-a-photo
feature is built, update the privacy policy first.

Analytics: a PostHog snippet (through the t.shaztech.io proxy) sits in the `<head>` of every page, with `cookieless_mode: 'always'` (no cookie or local storage). Keep the privacy policy's "This website" section in step with it.
