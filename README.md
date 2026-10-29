# rwtgames-apex-redirect

Serves the bare domain rwtgames.com (GitHub Pages) and sends every visitor to
https://www.rwtgames.com with the same path: `index.html` for `/`, `404.html`
for every other path (a script keeps path, query and hash).

Why: GoDaddy's domain forwarding only forwarded `/`; `rwtgames.com/osrs` gave a
404. The real site is he-ventures/yellow-hat on Railway (www.rwtgames.com).
DNS (GoDaddy): `@` A records to GitHub Pages (185.199.108-111.153); `www`
stays a CNAME to Railway.
