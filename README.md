# Safe Loop — Website

Static, SEO-optimized site for **Safe Loop** (child safety ecosystem for schools and parents). No build step, no nginx, no server required.

## Deploy in minutes (no nginx)

### Option 1: Netlify (easiest)
1. Sign up at [netlify.com](https://netlify.com).
2. Drag and drop the **safeloop-website** folder onto the Netlify deploy area, or connect your Git repo and set publish directory to `safeloop-website` (or root if the repo is only this site).
3. Your site is live. Point your domain (e.g. safeloop.com) in Netlify → Domain settings.

### Option 2: Vercel
1. Sign up at [vercel.com](https://vercel.com).
2. Import your project (or upload this folder). Vercel detects static files.
3. Deploy. Add your domain in Project → Settings → Domains.

### Option 3: GitHub Pages
1. Push this folder to a GitHub repo.
2. Repo → **Settings** → **Pages** → Source: **Deploy from a branch**.
3. Branch: `main`, folder: **/ (root)**. Save.
4. Site is at `https://<username>.github.io/<repo-name>/`. For a custom domain, add a CNAME file and set DNS.

### Option 4: Any static host
Upload the contents of **safeloop-website** (all files) to any host that serves static files: Cloudflare Pages, Firebase Hosting, AWS S3 + CloudFront, etc. No server or nginx needed.

## SEO checklist (already done in the site)

- Title and meta description with “Safe Loop” and key phrases
- Canonical URL (update in `index.html` when you have your real domain)
- Open Graph and Twitter meta tags
- Schema.org Organization + Product (JSON-LD)
- Semantic HTML (header, main, section, nav, footer)
- Clear H1/H2 structure and internal links

**After you have a domain:** Replace `https://safeloop.com/` in the canonical and og:url (and add a real og-image.png if you want). Update phone, email, and website in the footer and CTA.

## Run locally

Open `index.html` in a browser, or use a simple static server:

```bash
cd safeloop-website
npx serve .
```

Then open the URL shown (e.g. http://localhost:3000).

---

**Safe Loop — Because every child deserves to be safe. Every parent deserves to know.**
