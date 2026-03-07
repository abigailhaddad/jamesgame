# James's Game

## About This Project
This is a game being designed by James, age 9. James describes what he wants the game to do and Claude builds it.

## Technical Setup
- **Static site** hosted on Netlify at https://gamejames.netlify.app/
- The `web/` directory is what Netlify serves (configured in `netlify.toml`)
- All game code lives in `web/index.html` (or a small number of files in `web/` if the game grows)
- If Python scripts are needed (e.g. to generate game data or assets), they live in the repo root and output into `web/`
- No frameworks, no npm, no dependencies in the frontend — keep it simple

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
web/index.html    — the game (served by Netlify)
netlify.toml      — tells Netlify to serve from web/
```

## Workflow
- **Commit and push frequently.** After every meaningful change, commit and push to `main` so James can see it live.
- **Tell James to check the site.** After pushing, tell him to go to https://gamejames.netlify.app/ and refresh. Give it a minute to deploy.
- **Don't ask James to preview locally.** Always push to see changes live on the Netlify URL.

## Deploying
Netlify serves the `web/` directory. Any changes pushed to `main` go live automatically.
