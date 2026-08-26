# Agent Notes

- Pure HTML5 Canvas game; **no build, no dependencies, no bundler, no package manager**.
- All game logic lives in `game.js`; `index.html` loads it directly via `<script src="game.js">`.
- To run: open `index.html` in a browser, or serve locally with `npx serve .` and visit `http://localhost:3000`.
- No tests, no lint config, no CI. Verify by running in a browser.
