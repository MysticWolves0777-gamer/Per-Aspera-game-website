# Pocket Arcade

An installable mobile game hub (Progressive Web App). No build step, no dependencies.

## Put it online with GitHub Pages
1. Create a GitHub repo and push these files to the `main` branch.
2. In the repo go to Settings > Pages and set Source to "GitHub Actions".
3. After the workflow finishes, open `https://YOUR-NAME.github.io/YOUR-REPO/` on your phone.
4. Android Chrome: tap "Install on this phone". iPhone Safari: Share > Add to Home Screen.

## Add a new game
In `app.js`, write a function `startMyGame(api)` that draws on the canvas, calls `api.setScore(n)` and `api.over(finalScore)`, and returns a cleanup function. Then add one entry to the `GAMES` list. Bump `VERSION` in `sw.js` so phones update.

## Test locally
`python3 -m http.server 8000`, then open http://localhost:8000
