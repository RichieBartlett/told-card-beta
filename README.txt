TOLD CARD — PERSONAL IPAD BETA

FILES
index.html  — complete standalone interface
sw.js       — offline cache service worker
manifest.webmanifest — installable web app metadata
icon.png    — Home Screen icon

INSTALL / PUBLISH
1. Upload ALL FOUR files together to the same directory on an HTTPS static website (e.g. GitHub Pages, Cloudflare Pages, Netlify). Do not publish DSC or real operational information in repository files.
2. Visit the HTTPS address in Safari on your iPad while online. Wait for the page to load; revisit once to allow offline caching to complete.
3. Safari Share > Add to Home Screen > Open as Web App > Add.
4. Launch the new icon and test entering data, closing and reopening, switching sides, and airplane mode BEFORE depending on the app.

DATA / PRIVACY
No analytics, network APIs, account, or external dependencies are included. Flight entries use localStorage on that device and browser/app origin; they do not automatically sync or back up. DSC is never written to localStorage, but remains in JavaScript memory while this page stays alive. Reloading or closing the app may lose DSC. Device backups, screen captures, browser extensions, and device access are outside this prototype's control.

OFFLINE
Service worker caching requires HTTPS (or localhost for development). Opening index.html as a local file will NOT install offline caching. Cache availability depends on browser and iPadOS storage policies; test regularly.

SAFETY
This is an unvalidated personal design beta, not certified aviation software. It does not validate performance inputs, fuel, speeds, runway, ATIS, or procedures. Always use approved operational sources and procedures.
