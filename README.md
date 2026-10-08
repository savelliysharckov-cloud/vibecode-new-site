# vibecode-new-site

Live: https://savelliysharckov-cloud.github.io/vibecode-new-site/

A small browser piece that turns into a game. No dependencies, no build step, no samples.

**The piece**

- White `HELLO` on black grows organically into `GOODBYE` and back, one cycle every 3 seconds: a liquid morph between the two words' distance fields (WebGL2 shader). The motion never rests.
- With every cycle the word comes closer. After eight cycles (24 s) it spills past the screen edges and dissolves while the next run is already growing out of the centre.
- During the last two cycles of a run lightning strikes behind the letters, on the kicks and accented snares.
- An old-school drum & bass break (160 BPM, synthesised in Web Audio) plays on the same clock and gets louder and more distorted as the word grows. Browsers need one click or key press before sound can start; `M` mutes.
- Colours are taken from a reference image: indigo, plum, brick, rust, olive-yellow, moss, teal.

**The game**

- After three runs (72 s) the word is sucked down a hole, spiralling like a drain. A small white hole is left behind.
- The hole runs away from the pointer. It is slower than a decisive hand and can be cornered, so it can always be caught.
- Every catch earns a star and makes the hole a little quicker and the break a little dirtier. Five stars: `YOU WIN!` comes back out of the hole. Click to play again.
- Add `?runs=1` to the address to reach the game after 24 s instead of 72.

## Structure

- `index.html` — the whole site, a single static file with no build step
- `.nojekyll` — tells GitHub Pages to serve files as-is

## Deploy

The site is served by GitHub Pages from the `gh-pages` branch. To publish a change, push it to both branches:

```sh
git push origin main
git push origin main:gh-pages
```
