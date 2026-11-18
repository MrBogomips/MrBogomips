```csharp
Maybe<Architect> trade = "by trade";
Result<Builder>  habit = "by habit";
// partial to: DDD, event sourcing, and design that survives production
```

### 🛠️ `git log --author=me` — the OSS side

**🐑 Herding coding agents**

🛒 **[claude-plugins](https://github.com/MrBogomips/claude-plugins)** — the `mrbogomips` marketplace: every Claude Code plugin I ship, two commands away. Each plugin lives in its own repo and the marketplace only lists them, so a fix reaches you as soon as its repo moves. MIT, all the way down.

```
/plugin marketplace add MrBogomips/claude-plugins
/plugin install harness-maker@mrbogomips
```

On the shelf:

- 🧰 **[harness-maker](https://github.com/MrBogomips/harness-maker)** — Stands up, assesses and maintains a repo's agentic harness: project-specific agent teams and skills, an orchestrator that talks to your spec system and issue tracker, and a dual-tracker sync where the SaaS tracker is just a projection of the repo's source of truth. Formerly `agentic-harness`.
- 🎒 **[skills](https://github.com/MrBogomips/skills)** — A grab bag of generic skills for general-purpose tasks, for whichever agent you herd: Claude Code, Codex, Cursor and friends. A few examples: hand a task over to another session, get a TLDR of a long reply, bootstrap an `AGENTS.md`, generate an image. Want just one? `npx skills add MrBogomips/skills --skill <name>`.
- ✍️ **[eng-skills](https://github.com/MrBogomips/eng-skills)** — Technical writing for engineers: doc comments, API references, error messages, manuals and release notes written for whoever actually reads them, with ticket IDs kept out of published text. Ships a writer agent and an independent reviewer.
- 📐 **[eng-artifacts](https://github.com/MrBogomips/eng-artifacts)** — Engineering artifacts as self-contained HTML pages, ERDs first: one visual language, light/dark, swappable themes.
- 🔁 **[kaizen](https://github.com/MrBogomips/skills/tree/main/kaizen)** — Session retrospective: traces the errors and reworks of a session back to the skills, rules, `CLAUDE.md` and hooks behind them, and applies only the fixes you sign off.
- 🗣️ **[personal-voice](https://github.com/MrBogomips/skills/tree/main/personal-voice)** — Writes documents, emails and messages in your tone and lexicon, and learns from every edit you make to them.

Also in the herd:

- 🐑 **[herdr-tools](https://mrbogomips.github.io/herdr-tools/)** — [Herdr](https://herdr.dev) plugins for people with more agents than tabs: tabs named after their folder, spaces sorted and coloured per customer, and herdr-jump, a macOS picker that queues the agents waiting for you, FIFO, one key away from any app. MIT.
- ⚡ **[zsh-claude-oneshot](https://github.com/MrBogomips/zsh-claude-oneshot)** — The model is the command, quotes are optional: `opus commit local changes`, `git diff | haiku summarize`. One-shot Claude Code prompts from zsh. MIT.
- 🗄️ **[claude-code](https://github.com/MrBogomips/claude-code)** — The first marketplace, still serving PlantUML policy/lint/migrate, SOWs and PMI-PERT estimates, HR interview workflows and context hygiene. New plugins land in `claude-plugins`.

**🎹 Making noise**

- 🎹 **[kb-fx](https://github.com/MrBogomips/kb-fx)** — Your keyboard, now an instrument: a synthesized tone per keystroke (melodies imported from MIDI) and backlight colors on VIA-compatible boards over raw HID. Listen-only event tap; no lights-capable board, just sound. macOS CLI, MIT.

**🧮 .NET, the functional way**

- 🧩 **[bogoware/Monads](https://bogoware.github.io/Monads/)** — `Maybe` & `Result` for C#, because `null` was a billion-dollar mistake. Multi-target (.NET Std 2.1 / 8 / 9 / 10), 327 unit tests, MIT.
- 🌍 **[bogoware/Localization](https://bogoware.github.io/Localization)** — FQDN-keyed localization for .NET with first-class DI: every string has an address.
- 💶 **[bogoware/Moneta](https://github.com/bogoware/Moneta)** — Money math under the *Monetary Value Conservation Principle*: rounding error is tracked, never silently discarded. No cent left behind.

### ⚙️ Runtime config

```yaml
ddd: when the domain has real complexity
event_sourcing: where auditability is non-negotiable
architecture: governance, not gatekeeping
hands_on: true
prefer: tools that encode taste > prose that describes it
```

*📡 [Bogoware org](https://github.com/bogoware) · [LinkedIn](https://linkedin.com/in/giovannicostagliola) · giovanni.costagliola@gmail.com*
