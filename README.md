# vibecode-new-site — Hello, cat

Live: https://savelliysharckov-cloud.github.io/vibecode-new-site/

A small browser piece that turns into a game. No dependencies, no build step, no samples.

**The piece**

- White `Hello, cat` on black grows organically into `catch me if you can!` and back, one cycle every 4 seconds: a liquid morph between the phrases' distance fields (WebGL2 shader). The motion never rests.
- `Hello, cat` has a long tail growing from its last letter, reaching up the page and swaying from side to side.
- The letters and the tail are furred: fine strands, a rough outline, faint ginger tabby stripes.
- A counter at the top shows 3 on the first cycle, 2 on the second, 1 on the last.
- With every cycle the phrase comes closer. After three cycles (12 s, eight bars) it spills past the screen edges.
- During the last two cycles lightning strikes behind the letters, on the kicks and accented snares.
- An old-school drum & bass break (160 BPM, synthesised in Web Audio) plays on the same clock and gets louder and more distorted as the phrase grows. Browsers need one click or key press before sound can start; `M` mutes.
- Colours are taken from a reference image: indigo, plum, brick, rust, olive-yellow, moss, teal.

**The game**

- After those three cycles the phrase is sucked down a hole, spiralling like a drain. A small white hole is left behind.
- The pointer becomes a toothed trap that chomps like a mouth. The hole runs away from it; it is slower than a decisive hand and can be cornered, so it can always be caught.
- When it slips away it mocks you in a comic bubble: `Ha-ha-ha!` or `are you a cat or no?`
- Every catch earns a star and makes the hole a little quicker and the break a little dirtier. Five stars: `YOU WIN!` comes back out of the hole. Click to play again.
- Add `?runs=3` to the address to let the phrase grow three times (36 s) before the hole.

## Structure

- `index.html` — the whole site, a single static file with no build step
- `.nojekyll` — tells GitHub Pages to serve files as-is

## Deploy

The site is served by GitHub Pages from the `gh-pages` branch. To publish a change, push it to both branches:

```sh
git push origin main
git push origin main:gh-pages
```
