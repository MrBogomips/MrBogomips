```csharp
Maybe<Architect> trade = "by trade";
Result<Builder>  habit = "by habit";
// partial to: DDD, event sourcing, and design that survives production
```

### 🛠️ `git log --author=me` — the OSS side

**🐑 Herding coding agents**

🛒 **[claude-plugins](https://github.com/MrBogomips/claude-plugins)** — the `mrbogomips` marketplace: every Claude Code plugin I ship, two commands away. Each plugin lives in its own repo; the marketplace only lists them, so fixes reach you as soon as a repo updates. MIT, all the way down.

```
/plugin marketplace add MrBogomips/claude-plugins
/plugin install harness-maker@mrbogomips
```

🎼 **Spotlight: [agent-orchestration](https://mrbogomips.github.io/agent-orchestration/)** — for when one agent session is no longer enough. Two plugins, one repo, and a [documentation site](https://mrbogomips.github.io/agent-orchestration/) in English and Italian with diagrams, real screenshots, and worked scenarios: parallel sessions, two hats at once, pair programming on a shared host, and a product team. MIT.

- 🕸️ **[session-hub](https://mrbogomips.github.io/agent-orchestration/en/session-hub/)** — One master session in a folder of repositories starts a child session in each, so every child loads that repo's own rules, skills, and agents. Each child gets a model, an effort level, and a written scope enforced by a fail-closed hook; children talk only to the master, which routes anything outside their scope and tracks them in a record and a panel.
- 🔀 **[model-router](https://mrbogomips.github.io/agent-orchestration/en/model-router/)** — One written grid picks the model and effort level for every subagent and child session, while a fast judge catches starts without a model. It then measures on your machine how often each choice was right on the first try and what each success cost, so the grid answers to real work.

```
/plugin install session-hub@mrbogomips
/plugin install model-router@mrbogomips
```

On the shelf:

- 🧰 **[harness-maker](https://github.com/MrBogomips/harness-maker)** — Stands up, assesses, and maintains a repo's agentic harness: project-specific agent teams and skills, an orchestrator that talks to your spec system and issue tracker, and a dual-tracker sync where the SaaS tracker is just a projection of the repo's source of truth. Formerly `agentic-harness`.
- 🎒 **[skills](https://github.com/MrBogomips/skills)** — A grab bag of general-purpose skills for whichever agent you herd (Claude Code, Codex, Cursor, and friends): hand off a task to another session, get a TLDR of a long reply, bootstrap an `AGENTS.md`, or generate an image. Install a single skill with `npx skills add MrBogomips/skills --skill <name>`.
- ✍️ **[eng-skills](https://github.com/MrBogomips/eng-skills)** — Technical writing for engineers: doc comments, API references, error messages, manuals, and release notes written for whoever actually reads them, with ticket IDs kept out of published text. Ships a writer agent and an independent reviewer.
- 📐 **[eng-artifacts](https://github.com/MrBogomips/eng-artifacts)** — Engineering artifacts as self-contained HTML pages, ERDs first: one visual language, light and dark modes, and swappable themes.
- 🔁 **[kaizen](https://github.com/MrBogomips/skills/tree/main/kaizen)** — Session retrospective: traces errors and rework back to the skills, rules, `CLAUDE.md`, and hooks behind them, applying only the fixes you sign off on.
- 🗣️ **[personal-voice](https://github.com/MrBogomips/skills/tree/main/personal-voice)** — Writes documents, emails, and messages in your tone and lexicon, and learns from every edit you make.

Also in the herd:

- 🐑 **[herdr-tools](https://mrbogomips.github.io/herdr-tools/)** — [Herdr](https://herdr.dev) plugins for people with more agents than tabs: tabs named after their folder, spaces sorted and colored per customer, and herdr-jump, a macOS picker that queues waiting agents in FIFO order, one key away from any app. MIT.
- ⚡ **[zsh-claude-oneshot](https://github.com/MrBogomips/zsh-claude-oneshot)** — One-shot Claude Code prompts from zsh: the model is the command and quotes are optional (`opus commit local changes`, `git diff | haiku summarize`). MIT.
- 🗄️ **[claude-code](https://github.com/MrBogomips/claude-code)** — The original marketplace, still serving PlantUML policy/lint/migrate, SOWs and PMI-PERT estimates, HR interview workflows, and context hygiene. New plugins land in `claude-plugins`.

**🎹 Making noise**

- 🎹 **[kb-fx](https://github.com/MrBogomips/kb-fx)** — Your keyboard, now an instrument: a synthesized tone per keystroke (melodies imported from MIDI) and backlight colors on VIA-compatible boards over raw HID. macOS CLI using a listen-only event tap; without a supported backlit board, it plays sound only. MIT.

**🧮 .NET, the functional way**

- 🧩 **[bogoware/Monads](https://bogoware.github.io/Monads/)** — `Maybe` and `Result` for C#, because `null` was a billion-dollar mistake. Multi-target (.NET Std 2.1 / 8 / 9 / 10) with 327 unit tests. MIT.
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