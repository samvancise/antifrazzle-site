# Antifrazzle

Barebones company website for antifrazzle.com, owned by GitHub `samvancise`.

Static HTML and CSS with the owner-supplied PNG logo. No JavaScript, cookies,
analytics, contact-form backend, or connection to the game's wallet or QA service.
The contact link opens the visitor's email client addressed to info@antifrazzle.com.
The mailbox must be configured separately in Lark.

## Local preview

Serve this directory with a static HTTP server, for example
`py -3 -m http.server 4174 --bind 127.0.0.1`, then visit http://127.0.0.1:4174.

## Hosting

Intended hosting is GitHub Pages from the root of `main` in
`samvancise/antifrazzle-site`, with GoDaddy DNS for antifrazzle.com.
Hosting and mail setup are not complete until independently verified.
Only this website directory belongs in the public repository; never copy game
provider documents, credentials, or local game data into it.
