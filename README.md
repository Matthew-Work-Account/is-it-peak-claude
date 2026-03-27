# Is It Peak Claude Hours?

A tiny site with one purpose: quickly show whether we're in the peak Claude window.

## Why this exists

I wanted a fast, no-nonsense reference for peak hours instead of repeatedly doing timezone math.

Context that motivated it:

- Reddit: https://www.reddit.com/r/ClaudeAI/comments/1s4idaq/update_on_session_limits/
- X/Twitter: https://x.com/trq212/status/2037254607001559305

## What "peak" means here

- **Weekdays (Mon–Fri)**
- **5:00 AM – 11:00 AM PT**
- Often written as **1:00 PM – 7:00 PM GMT**

## Live URL

- https://Matthew-Work-Account.github.io/is-it-peak-claude/

## What the page shows

- `PEAK` vs `OFF-PEAK`
- Live countdown to the next boundary
- Timeline marker for current PT time

## Scope

- `index.html` contains all UI + logic.
- `.github/workflows/pages.yml` deploys to GitHub Pages.
- No framework, no build step, no backend.
