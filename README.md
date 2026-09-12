# Rosary Vigil

A paced companion for praying the Rosary — spoken aloud in sync with the on-screen text, tracked bead by bead on a 59-bead loop shaped like a real rosary, with a log of every intention and every run.

- Selects today's Mystery set (Joyful / Sorrowful / Glorious / Luminous) automatically by day of week.
- Speaks each prayer via the browser's text-to-speech, advancing the text exactly when the spoken line ends.
- Pauses for a few seconds after each Mystery's meditation before moving on, so it has room to land.
- Keeps that Mystery's name and its "Consider…" line visible as a subtitle for the whole decade that follows — Our Father through the Fatima Prayer — as a meditation aid, not just while it's first announced.
- Sets an intention once, then runs on its own — pause, resume, or step through manually at any point.
- Keeps a log (date, Mystery set, intention, completion, duration) in the browser's own local storage — no account or login involved. Deliberate tradeoff: the log stays with whichever browser you used, not shared across browsers or devices. Each entry can carry its own note, added or edited any time, to journal whether the intention was answered.
- A second card below the Rosary plays any single prayer on its own, spoken and word-highlighted the same way: the eight Rosary components, plus the Peace Prayer of St. Francis, Act of Contrition, Anima Christi, Memorare, the Angelus, and the Saint Michael Prayer (texts from [catholicity.com](https://www.catholicity.com/prayer/prayers.html)).
- A third card offers ten patron saints recognized for a particular need — St. Jude for hopeless causes, St. Anthony for lost articles, St. Lucy for eyesight, and so on — each with their traditional prayer, played the same way. Kept separate from the Rosary log: a patron's prayer carries no intention or Mystery, so it isn't logged as a session. Prayers that traditionally leave room for a personal petition (St. Jude, St. John Bosco) get an intention field that's spoken in place of the placeholder.
- A sidebar panel names the day's principal saint or feast from the General Roman Calendar — the Church's own official universal calendar — with a short blurb, and says so plainly on days that calendar doesn't cover (most saints are only locally venerated, without a fixed universal date).
- A fourth card offers the Jesus Prayer ("Lord Jesus Christ, Son of God, have mercy on me, a sinner," in full, shorter, and shortest traditional forms). Deliberately kept distinct from the Rosary cards above it: this is Eastern Christian (Orthodox and Eastern Catholic) hesychast practice, traditionally kept on a knotted prayer rope — a komboskini or chotki — not a rosary, and traditionally received from a spiritual father rather than picked up solo from an app. The card's own text says as much.

## Where this lives

- **[claude.ai Artifact](https://claude.ai/code/artifact/9f8a8392-4e41-4b52-a07f-b32eb576b3e3)** — the day-to-day one.
- **[GitHub Pages](https://willycraig1.github.io/rosary-vigil/)** — the same app, served straight from this repo's `main` branch.
- `index.html` here is also the source, kept for backup and version history.

All three run identical code and behave the same — the log is always local to whichever browser opened it, not tied to the hosting, so there's no sync between them.

## Voice quality

Voice output uses the browser/OS's built-in speech synthesis. The page scores and sorts available voices, surfacing any Enhanced/Premium/Neural voice (and Chrome's free "Google" network voices) under "Recommended," with a search box to find a specific one in a long list. For a noticeably better voice on macOS, install one via **System Settings → Accessibility → Spoken Content → System Voice → Manage Voices**, then reload — Safari in particular can take a few seconds to notice a newly-installed voice, which the page now polls for automatically. Note: Siri's own voices aren't reachable by any browser or app — Apple keeps that engine private, separate from the public voice APIs every browser uses.

Word-by-word highlighting tracks the voice engine's own word-boundary events when a voice reports them — confirmed working for every local system voice tested (Enhanced ones included, not just Ava). Chrome's free network "Google" voices never report boundaries at all — a Chromium limitation, not something a page can ask around — so for those the highlight instead paces itself across an estimate of the utterance's length. It's a deliberate approximation, not a real sync, for the one class of voice that gives the page nothing to sync to.

---

Built collaboratively with Claude.

🤖 Generated with [Claude Code](https://claude.com/claude-code)
