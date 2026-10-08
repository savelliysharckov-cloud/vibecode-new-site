# vibecode-new-site — Hello, cat

Live: https://savelliysharckov-cloud.github.io/vibecode-new-site/

A small browser piece that turns into a game. No dependencies, no build step, no samples.

**The piece**

- White `Hello, cat` on black grows organically into `catch me if you can!` and back, one cycle every 3 seconds: a liquid morph between the phrases' distance fields (WebGL2 shader). The motion never rests.
- `Hello, cat` has a long tail growing from its last letter, arching back over the whole phrase and swaying.
- A counter at the top shows 3 on the first cycle, 2 on the second, 1 on the last.
- With every cycle the phrase comes closer, but it always stays wholly inside the page: it starts at 40% and ends as large as the page allows (9 s, six bars).
- During the last two cycles lightning strikes behind the letters, on the kicks and accented snares.
- An old-school drum & bass break (160 BPM, synthesised in Web Audio) plays on the same clock and gets louder and more distorted as the phrase grows. Browsers need one click or key press before sound can start; `M` mutes.
- Colours are taken from a reference image: indigo, plum, brick, rust, olive-yellow, moss, teal.

**The game**

- After those three cycles the phrase is sucked down a hole, spiralling like a drain. A small white hole is left behind.
- The pointer becomes a toothed trap that chomps like a mouth. Every three seconds it grows a tail, ears or whiskers for a moment. The hole runs away from it; it is slower than a decisive hand and can be cornered, so it can always be caught.
- When it slips away it mocks you in a comic bubble: `Ha-ha-ha!` or `are you a cat or no?`
- Every catch earns a star and a pleased meow with a purr (synthesised), makes the hole a little quicker and the break clearly louder and dirtier.
- Cat ghosts drift up through the background: whole cats seen from the side, with ears, whiskers, a swaying tail and four stepping paws.
- Fail to catch the hole for 6 seconds and a giant cat-ghost silhouette looms up, strobing, with a cackle: `you are not a cat!!!!!!` (No strobe for visitors who ask their system for reduced motion.)
- Five stars: ten cats meow at once, `YOU WON!` comes back out of the hole and grows into `cats thank you`. Click to play again.
- Add `?runs=3` to the address to let the phrase grow three times (27 s) before the hole.

## Structure

- `index.html` — the whole site, a single static file with no build step
- `.nojekyll` — tells GitHub Pages to serve files as-is

## Deploy

The site is served by GitHub Pages from the `gh-pages` branch. To publish a change, push it to both branches:

```sh
git push origin main
git push origin main:gh-pages
```
