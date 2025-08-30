SPACEGATE SHUTDOWN PAGE — QUICK DEPLOY

Files:
- index.html (the notice page)

A) Deploy with GoDaddy Hosting (cPanel)
1) Upload index.html to the document root for your domain/subdomain.
2) If this is a subdomain, create it in cPanel (e.g., app.example.com) and upload index.html to its root.

B) Deploy with Netlify (no server needed)
1) Go to app.netlify.com → "Add new site" → "Deploy manually".
2) Drag-and-drop index.html.
3) In GoDaddy DNS, point the domain/subdomain to Netlify (add a CNAME to your Netlify subdomain).

C) Deploy with GitHub Pages
1) Create a repo with index.html in the root.
2) Settings → Pages → Deploy from main branch (root).
3) In GoDaddy DNS, add a CNAME record to your GitHub Pages URL.

D) Optional: Serve HTTP 410 (Gone) at the server level
- This is handled by your hosting/platform configuration, not the HTML file.
- Nginx example:
    location = / { return 410; }
- Apache example (.htaccess in site root):
    Redirect gone /

E) Wording / Legal
- The text provided is neutral and avoids definitive allegations. If you want stronger wording (e.g., naming parties),
  consult your lawyer first and edit index.html accordingly.
