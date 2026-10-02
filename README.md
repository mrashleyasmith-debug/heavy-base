# Heavy Base

Be hard to move.

A phone-first strength training log: tap-to-log sets, plate math, rest timer, automatic progression,
multiple programs, and training together on one phone. Heavy Base × FlyTy.

## Use it

Open the site in Safari on iPhone, tap Share, then **Add to Home Screen**. It opens full screen and works
offline in the gym. Your log is saved on your phone; use Settings → Your data to back it up or move it.

## How it's built

A single `index.html` (all CSS and JS inline), `manifest.webmanifest` and `sw.js` for install and offline,
and `icons/`. No build step. Hosted free on GitHub Pages from the `main` branch.

Saved state lives in localStorage under the key `barbell-logbook-v1`. Any change to the state shape goes
through `normalize()` so existing logs keep working.
