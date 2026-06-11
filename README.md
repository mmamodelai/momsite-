# Charlene Clare — Personal Website

A simple one-page personal site for Charlene Clare, Certified Peer Support Specialist (San Diego, CA).

- Single static `index.html` — no build step, no dependencies.
- Plus `robots.txt` + `sitemap.xml` for SEO. Structured data (JSON-LD Person schema), canonical, and Open Graph tags are inline in `index.html`.
- Target: Vercel hosting, custom domain **charleneclare.com** (domain is registered, DNS managed at Cloudflare).

## Deploy (not yet done — checklist)
1. **Vercel**: import the `mmamodelai/momsite-` repo → deploy with default settings (no framework, output = repo root).
2. **Vercel → Settings → Domains**: add `charleneclare.com` and `www.charleneclare.com`.
3. **Cloudflare DNS** (charleneclare.com zone — currently has NO records, which is why the domain doesn't resolve):
   - `A` record: `@` → `76.76.21.21` (DNS only / grey cloud)
   - `CNAME` record: `www` → `cname.vercel-dns.com` (DNS only / grey cloud)
4. Verify https://charleneclare.com loads, then submit `https://charleneclare.com/sitemap.xml` in Google Search Console.

## Edit
Everything lives in `index.html`. Open it in a browser to preview locally.
