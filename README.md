# Antifrazzle

Barebones company website for antifrazzle.com, owned by GitHub `samvancise`.

Static HTML and CSS with the owner-supplied PNG logo. No JavaScript, cookies,
analytics, contact-form backend, or connection to the game's wallet or QA service.
The contact link opens the visitor's email client addressed to info@antifrazzle.com.
The address is configured as a shared mailbox in Lark, accessible from the owner's
existing account. End-to-end email delivery has not been tested.

## Local preview

Serve this directory with a static HTTP server, for example
`py -3 -m http.server 4174 --bind 127.0.0.1`, then visit http://127.0.0.1:4174.

## Hosting

Hosting is GitHub Pages from the root of `main` in
`samvancise/antifrazzle-site`, with GoDaddy DNS for antifrazzle.com.
The apex has GitHub Pages' four A records (185.199.108.153 through
185.199.111.153); `www` is a CNAME to `samvancise.github.io`. GitHub's domain
health check passed for both names on October 12, 2026. The existing Lark MX
records and solitaire QA subdomain are unchanged. HTTPS is enabled and enforced;
`https://www.antifrazzle.com` redirects to `https://antifrazzle.com`.

Desktop and 390-pixel phone browser checks confirmed the supplied logo loads,
the contact link targets the correct address, and the page has no horizontal
overflow. HTTPS serving on the custom domain and the `www` redirect were verified
after the DNS change.

Only this website directory belongs in the public repository; never copy game
provider documents, credentials, or local game data into it.
