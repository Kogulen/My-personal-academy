MY PERSONAL ACADEMY – OFFLINE EDITION 1.0
==============================================

This is an initial iPad-installable Progressive Web App (PWA) conversion of the supplied SwiftUI Version 1.6 source.

FILES
- index.html: app shell
- style.css: layout and styling
- app.js: MBA, English, planner, local PDF library and local data
- manifest.webmanifest: Home Screen app metadata
- sw.js: offline application-shell cache
- icon-192.png / icon-512.png: app icons

IMPORTANT LIMITATIONS
1. The app must be hosted from an HTTPS website to install as a PWA on iPad.
2. Open the hosted site online once, then use Safari > Share > Add to Home Screen.
3. Open the installed icon once while online so the service worker caches the app shell. Then test Airplane Mode.
4. The PDF library stores imported PDFs in this browser's IndexedDB and can open them locally. The first edition does not yet include PDF text extraction, so MBA Tutor keyword search and automatic question generation are not active yet.
5. Browser local data is separate from the Swift Playgrounds app. Existing Swift app progress and PDFs do not automatically transfer.
6. This is a web app, not a native signed iOS .ipa application.
7. Do not clear Safari website data if you want to preserve this app's local data. Keep separate backups.

HOSTING
Upload all files and folders in this package to an HTTPS static host. GitHub Pages is one possible option. The root of the hosted site must contain index.html, sw.js and manifest.webmanifest.
