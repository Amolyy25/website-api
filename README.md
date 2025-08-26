Spam Detector API – Static Website
=================================

Production-ready, responsive static site for the Spam Detector API hosted on RapidAPI.

Pages
-----

- `index.html`: Landing page with hero, benefits, and examples
- `docs.html`: Endpoints, examples (curl, JS, Python), error codes, pricing

Configure
---------

Edit `website/config.js`:

- `rapidApiListingUrl`: your RapidAPI listing link
- `rapidApiHostDefault`: e.g., `spam-detector-api.p.rapidapi.com`
- `baseUrlDefault`: e.g., `https://spam-detector-api.p.rapidapi.com`
- `githubUrl`: optional repository link
- Pricing values are prefilled from your `config.yaml`

Deploy
------

Vercel (recommended)

1. Import this repository into Vercel
2. Framework preset: Other
3. Output directory: `website`
4. Build command: none (static)
5. Optional Edge function for proxy: `vercel_functions/proxy-check.js`

Netlify

1. New site from Git
2. Publish directory: `website`
3. Build command: none (static)

SEO
---

- Update canonical URLs in each HTML head
- Ensure `og:image` points to a hosted image (`/website/assets/hero-illustration.svg` works when deployed)

Security Notes
--------------

- Do not hardcode secrets into the frontend

Development
-----------

Open `website/index.html` in your browser. Tailwind is loaded via CDN for zero-build workflow.


