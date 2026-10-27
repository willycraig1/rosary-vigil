# Rosary Vigil

A paced Rosary companion: spoken prayers synced to the text, a 59-bead loop, and an intention log. It's a single `index.html` with no build step. `README.md` describes every card and decision.

## Rules
- Keep it one self-contained file. The log stays in browser localStorage, with no accounts.
- Prayer texts come from catholicity.com. Keep the sourcing, and don't paraphrase prayers.
- The Jesus Prayer card stays clearly separate from the Rosary cards (Eastern Christian practice), and patron-saint prayers aren't logged as sessions.
- Voice: local system voices give word-boundary events. Chrome's "Google" voices don't, so their highlight is an estimate. Don't try to "fix" that.

## Where it lives
- GitHub Pages: https://willycraig1.github.io/rosary-vigil/ (pushing to `main` redeploys)
- claude.ai artifact (the day-to-day copy): https://claude.ai/code/artifact/9f8a8392-4e41-4b52-a07f-b32eb576b3e3
- After a change, update both so they stay identical (ask before pushing).
