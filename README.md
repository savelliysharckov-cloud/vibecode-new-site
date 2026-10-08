# vibecode-new-site

Live: https://savelliysharckov-cloud.github.io/vibecode-new-site/

A placeholder page for now — the actual project is coming. What it does:

- White `HELLO` on black grows organically into `GOODBYE` and back, one cycle every 3 seconds: a liquid morph between the two words' distance fields (WebGL2 shader, no dependencies). The motion never rests.
- With every cycle the word comes closer. After eight cycles (24 s) it spills past the screen edges and dissolves while the next run is already growing out of the centre.
- During the last two cycles lightning strikes behind the letters, on the kicks and accented snares.
- An old-school drum & bass break (160 BPM, synthesised in Web Audio, no samples) plays on the same clock: it gets louder and more distorted as the word grows. Browsers need one click or key press before sound can start; click again to mute.
- Colours are taken from a reference image: indigo, plum, brick, rust, olive-yellow, moss, teal.

## Structure

- `index.html` — the whole site, a single static file with no build step
- `.nojekyll` — tells GitHub Pages to serve files as-is

## Deploy

The site is served by GitHub Pages from the `gh-pages` branch. To publish a change, push it to both branches:

```sh
git push origin main
git push origin main:gh-pages
```
