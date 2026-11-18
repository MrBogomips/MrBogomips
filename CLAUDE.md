# CLAUDE.md

This file provides guidance to Claude Code when working with code in this repository.

## What this repository is

The GitHub profile repository of `MrBogomips`: `README.md` at the root is rendered on
https://github.com/MrBogomips. There is no code, build, lint or test suite. The only deliverable
is `README.md`, and it must keep that exact name and location to show on the profile.

The personal blog is not here: it lives in its own repository, `MrBogomips/blog`. The local
branches `blog-export` and `feature/quantum-blog-astro` are leftovers from before the move.

## README conventions

- **Voice**: geeky, terse, first person, link-led. The opener is a C# snippet, the OSS heading is
  `` `git log --author=me` ``, the closing section is a YAML "runtime config". Keep that register.
- **OSS list**: grouped by theme under bold, emoji-prefixed group titles. Each entry is
  `- <emoji> **[name](link)** — <one or two sentences>. MIT.` (licence stated only when verified).
- The `claude-plugins` marketplace (`mrbogomips`) leads the coding-agents group, with its install
  commands and the plugins it serves. Plugin descriptions follow the marketplace's own
  README and `marketplace.json` in `MrBogomips/claude-plugins`.
- English only. No client names, no badges, no GitHub-stats cards or widgets (a stats widget
  was removed as unreliable).
- Before committing, check every link in the README:
  ```bash
  grep -oE 'https://[^) ]+' README.md | sort -u | while read u; do
    printf "%s %s\n" "$(curl -s -o /dev/null -L -w '%{http_code}' "$u")" "$u"; done
  ```

## Revisions

`README.md` is revised in place (no versioned copies). Releases of the profile are marked with
semver git tags (`v1.0.0`, `v2.0.0`, `v2.1.0`): major for a restructuring, minor for new or
clarified content, patch for form and formatting.

## Working documents

- `README.md` is the only authoritative document.
- New drafts, specs and plans stay in the session scratchpad; do not create repository folders
  for them.
- `.aidocs/` (gitignored) holds the April 2026 profile redesign spec and plan. It is historical:
  the README has since moved to the current emoji/snippet style, so it never overrides `README.md`.

## Git / PR Working Policy

- Worktree usage: disabled (topic branch from `main` in the main checkout)
- Worktree location: n/a
- Base branch: main
- Recorded on: 2026-11-18
