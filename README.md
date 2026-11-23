# NPM Tech Solutions

Website for NPM Tech Solutions: our apps, games and their privacy policies. Plain static HTML and CSS, no JavaScript, no analytics, no build step. Served by GitHub Pages from `main`, root.

## URLs
- Site: https://npmtechsolutions-arch.github.io
- SpeakEasy home and support: https://npmtechsolutions-arch.github.io/speakeasy/
- SpeakEasy privacy policy: https://npmtechsolutions-arch.github.io/speakeasy/privacy.html
- Mammoth Hunt privacy policy: https://npmtechsolutions-arch.github.io/mammoth-hunt/privacy.html
- Dragon Hunt privacy policy: https://npmtechsolutions-arch.github.io/dragon-hunt/privacy.html
- app-ads.txt (AdMob, shared by all apps of publisher pub-6254026885647002): https://npmtechsolutions-arch.github.io/app-ads.txt

## Preview locally
- VS Code: open this folder and use the Live Server extension ("Go Live").
- Or in Terminal, from this folder: `python3 -m http.server 8000`, then open http://localhost:8000/ (the 404 page only works on GitHub Pages).

## Deploy
Commit and push to `main`; GitHub Pages publishes within a minute or two (Settings → Pages shows the status).

## SpeakEasy pages (`speakeasy/`)
- `index.html` (home and support), `privacy.html`.
- `assets/css/style.css`: brand colours, light and dark mode. Contrast was checked for every colour pair (WCAG AA, most AAA): text 16.9:1, muted 7.7:1, links 7.7:1 (light); 16.1:1, 10.6:1, 9.3:1 (dark); text on the orange band at least 7.7:1.
- `assets/fonts/`: Plus Jakarta Sans and Inter (Latin subset), self-hosted so the site sends nothing to Google Fonts. SIL Open Font License, see the `OFL-*.txt` files.
- `assets/img/`: logo, favicon, Apple touch icon and Open Graph image, copied from the SpeakEasy brand folder.
- The privacy policy describes what the app build actually does. Update it before switching on a feature that sends data off the phone (place lookup, crash reports, a downloadable AI model, the remote settings file).

## Other files
- `app-ads.txt`: one line for Google AdMob.
- `404.html`, `robots.txt`, `.nojekyll` (serve files as they are).
