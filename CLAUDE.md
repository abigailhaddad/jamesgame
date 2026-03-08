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
- **Be encouraging.** If James has a cool idea, say so! But also be honest if something won't work or needs to be simpler first.
- **Don't over-ask.** A kid will lose patience if you ask 5 clarifying questions before doing anything. Make reasonable assumptions and build something, then iterate based on his feedback. One or two questions max, then start building.
- **Ask clarifying questions about game design, not code.** For example: "What should happen when the player runs out of lives?" is good. "Should I use canvas or DOM elements?" is not — just decide.
- **Keep explanations simple.** Don't explain code internals. Do explain what changed in terms of what the game does now.
- **Show, don't tell.** After making changes, tell James to refresh the page and try it out rather than describing the code.
- **Scope things down when needed.** If James asks for something huge, build a small working version first and iterate.

## Game Development Rules
- **Use DOM elements and CSS for the game** (divs, spans, CSS animations). No `<canvas>`. This keeps things simple and easy to style.
- **Don't break what's already working.** Read existing code before making changes. A kid will get frustrated fast if something that worked before suddenly doesn't.
- **Keep the game playable at every push.** Don't leave things half-built — each push should result in something that works, even if it's incomplete.
- **Keep it mobile-friendly.** James might be on a phone or tablet. Make sure touch controls work and the game fits small screens.

## Project Structure
```
web/index.html    — the game (served by Netlify)
netlify.toml      — tells Netlify to serve from web/
STATUS.md         — tracks what James has asked for and what's been built
```

## Status Tracking
- **Keep `STATUS.md` up to date.** After implementing a new feature or making a significant change, update `STATUS.md` to reflect what was added. This helps James's mom (and future sessions) understand the current state of the game.
- Add new requests to the "What James Has Asked For" list and update the "Current Features" section as needed.

## Workflow
- **Use VS Code preview for development.** After making changes, tell James to check the preview in VS Code. No need to push for every small change.
- **Commit regularly.** Make small, frequent commits to keep a good history of changes.
- **Push only to publish.** Only push to `main` when things are in a good state — a feature is done, the game is stable, etc.
- **Tell James to check the live site after pushing.** After pushing, tell him to go to https://gamejames.netlify.app/ and refresh. Give it a minute to deploy.

## Deploying
Netlify serves the `web/` directory. Any changes pushed to `main` go live automatically.
