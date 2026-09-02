# Rosary Vigil

A paced companion for praying the Rosary — spoken aloud in sync with the on-screen text, tracked bead by bead on a 59-bead loop shaped like a real rosary, with a log of every intention and every run.

- Selects today's Mystery set (Joyful / Sorrowful / Glorious / Luminous) automatically by day of week.
- Speaks each prayer via the browser's text-to-speech, advancing the text exactly when the spoken line ends.
- Pauses for a few seconds after each Mystery's meditation before moving on, so it has room to land.
- Sets an intention once, then runs on its own — pause, resume, or step through manually at any point.
- Keeps a durable log (date, Mystery set, intention, completion) — server-side when hosted as a Claude Artifact, falling back to the browser's local storage when run standalone (as this file does).

## This repo vs. the live version

`index.html` here is the source, kept for backup and version history. The version actually in daily use is published as a [Claude Artifact](https://claude.ai/code/artifact/9f8a8392-4e41-4b52-a07f-b32eb576b3e3), which additionally persists the log across devices. Opening `index.html` directly (or via GitHub Pages) works too — it just keeps its log locally to that browser instead.

## Voice quality

Voice output uses the browser/OS's built-in speech synthesis. The page scores and sorts available voices, surfacing any Enhanced/Premium/Neural voice under "Recommended." For a noticeably better voice on macOS, install one via **System Settings → Accessibility → Spoken Content → System Voice → Manage Voices**, then reload.

---

Built collaboratively with Claude.

🤖 Generated with [Claude Code](https://claude.com/claude-code)
