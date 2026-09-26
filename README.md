# Chalkieboard tester hostname redirect

This small GitHub Pages site keeps the legacy `tester.207studio.dev` hostname working and sends visitors to the canonical GitHub Pages tester guide:

<https://chalkieboard.207studio.dev/beta/>

The custom domain lives in this repository's root `CNAME`. Its DNS record should be a single `CNAME tester -> chalkieboard.github.io`. Do not replace the apex domain's other records or change `chalkieboard.207studio.dev`.

GitHub Pages serves `index.html` over HTTPS. The page immediately navigates to the canonical guide and includes a link if scripting is disabled. It makes no network calls, loads no external assets, and does not retain query strings or fragments.
