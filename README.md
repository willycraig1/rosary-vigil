# Rosary Vigil

A paced companion for praying the Rosary — spoken aloud in sync with the on-screen text, tracked bead by bead on a 59-bead loop shaped like a real rosary, with a log of every intention and every run.

- Selects today's Mystery set (Joyful / Sorrowful / Glorious / Luminous) automatically by day of week.
- Speaks each prayer via the browser's text-to-speech, advancing the text exactly when the spoken line ends.
- Pauses for a few seconds after each Mystery's meditation before moving on, so it has room to land.
- Sets an intention once, then runs on its own — pause, resume, or step through manually at any point.
- Keeps a log (date, Mystery set, intention, completion) in the browser's own local storage — no account or login involved. Deliberate tradeoff: the log stays with whichever browser you used, not shared across browsers or devices.
- A second card below the Rosary plays any single prayer on its own — Sign of the Cross, Apostles' Creed, Our Father, Hail Mary, Glory Be, O My Jesus, Hail Holy Queen, or the Closing Prayer — spoken and word-highlighted the same way.

## Where this lives

- **[claude.ai Artifact](https://claude.ai/code/artifact/9f8a8392-4e41-4b52-a07f-b32eb576b3e3)** — the day-to-day one.
- **[GitHub Pages](https://willycraig1.github.io/rosary-vigil/)** — the same app, served straight from this repo's `main` branch.
- `index.html` here is also the source, kept for backup and version history.

All three run identical code and behave the same — the log is always local to whichever browser opened it, not tied to the hosting, so there's no sync between them.

## Voice quality

Voice output uses the browser/OS's built-in speech synthesis. The page scores and sorts available voices, surfacing any Enhanced/Premium/Neural voice (and Chrome's free "Google" network voices) under "Recommended," with a search box to find a specific one in a long list. For a noticeably better voice on macOS, install one via **System Settings → Accessibility → Spoken Content → System Voice → Manage Voices**, then reload — Safari in particular can take a few seconds to notice a newly-installed voice, which the page now polls for automatically. Note: Siri's own voices aren't reachable by any browser or app — Apple keeps that engine private, separate from the public voice APIs every browser uses.

---

Built collaboratively with Claude.

🤖 Generated with [Claude Code](https://claude.com/claude-code)
