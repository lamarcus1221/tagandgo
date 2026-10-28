# Tag & Go parent app

An installable phone app for the Tag & Go parent "I'm here" check-in.
It holds no student data: it only sends a tag number and family code to the
school's Parent Check-In Apps Script, which does all the checking.

## Files
- index.html: the app
- config.js: the ONLY file to edit (paste the Parent Check-In /exec URL and school name)
- manifest.webmanifest, sw.js, icons/: make it installable with the Tag & Go icon

## Hosting
Any static HTTPS host works (GitHub Pages, Netlify, Firebase Hosting, Cloudflare Pages).
Upload all files, keeping the icons folder.

## After changing config.js or index.html
Bump the CACHE name in sw.js (taggo-v1 -> taggo-v2) so installed phones pick up the change.
