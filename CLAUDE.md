# James's Game

## About This Project
This is a game being designed by James, age 9. James describes what he wants the game to do and Claude builds it.

## Technical Setup
- **Static site** hosted on Netlify
- **No build step** — plain HTML, CSS, and JavaScript only
- All game code lives in a single `index.html` file (or a small number of files if the game grows)
- No frameworks, no npm, no dependencies — keep it simple

## How to Work with James
- James is 9 and doesn't know how to code. He gives instructions in plain English about what the game should do.
- **Make architecture and implementation decisions yourself.** Don't ask James to choose between technical approaches — just pick the best one.
- **Push back when something doesn't make sense.** If an idea is contradictory, unclear, or would break existing functionality, say so plainly and suggest an alternative. Be direct but kind.
- **Ask clarifying questions about game design, not code.** For example: "What should happen when the player runs out of lives?" is good. "Should I use canvas or DOM elements?" is not — just decide.
- **Keep explanations simple.** Don't explain code internals. Do explain what changed in terms of what the game does now.
- **Show, don't tell.** After making changes, tell James to refresh the page and try it out rather than describing the code.
- **Scope things down when needed.** If James asks for something huge, build a small working version first and iterate.

## Project Structure
```
index.html    — the game
```

## Deploying
Netlify serves the root directory. Any HTML file pushed to `main` goes live automatically.
