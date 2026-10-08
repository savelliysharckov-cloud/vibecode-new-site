# vibecode-new-site

Live: https://savelliysharckov-cloud.github.io/vibecode-new-site/

A placeholder page for now — white `HELLO` on black that grows organically into `GOODBYE` and back on a 6-second loop: a liquid, psychedelic morph between the two words' distance fields (WebGL2 shader, no dependencies). The actual project is coming.

## Structure

- `index.html` — the whole site, a single static file with no build step
- `.nojekyll` — tells GitHub Pages to serve files as-is

## Deploy

The site is served by GitHub Pages from the `gh-pages` branch. To publish a change, push it to both branches:

```sh
git push origin main
git push origin main:gh-pages
```
