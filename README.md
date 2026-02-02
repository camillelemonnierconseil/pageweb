# pageweb — Camille Lemonnier

Simple static site for `camillelemonnier-expertise.fr`.

Quick deploy steps (run from the `pageweb` folder):

```bash
# initialize git if needed
git init
git add .
git commit -m "Initial site"
git branch -M main
git remote add origin https://github.com/camillelemonnierconseil/pageweb.git
git push -u origin main
```

GitHub Pages: enable Pages in repository Settings → Pages, serve from `main` branch (root). Add custom domain `camillelemonnier-expertise.fr` in Pages settings if not auto-detected.

DNS records to add at your registrar (recommended):

- For the apex domain `camillelemonnier-expertise.fr` (create A records):

  185.199.108.153
  185.199.109.153
  185.199.110.153
  185.199.111.153

- For the `www` subdomain (create a CNAME):

  Host: `www` → CNAME → `camillelemonnierconseil.github.io`

After DNS propagates, enable "Enforce HTTPS" in Pages settings.
