<div align="center">

# 🐦 Perch

**A native macOS menu bar app that watches all your Claude Code sessions at a glance.**

Running many Claude Code agents across terminals and projects? Perch shows — right in your menu bar — which ones are working, which are waiting on you, and which are idle, so you stop shuffling between windows.

[**⬇ Download the latest release**](https://github.com/ik-labs/perch/releases/latest)

</div>

---

## Screenshots

<!-- TODO: drop real screenshots/GIF into assets/ and reference them here, e.g.:
![Perch dropdown](assets/panel.png)
![Menu bar](assets/menubar.png)
-->

---

## What it shows

- **Every session at a glance** — running / waiting-for-you / idle / done, sorted so anything needing you floats to the top.
- **What each agent is doing** — the live command it's running, or its in-progress task.
- **Task checklists** — the session's task list, with an in-progress summary that expands to the full checklist (✓ / ◐ / ◻), including dependencies.
- **Account usage** — your 5-hour and 7-day limits with reset timers.
- **Per-session detail** — model (incl. 1M-context), reasoning effort, live context %, and cost.
- **Rich notifications** — when an agent finishes, the banner shows *what it did*; when it needs you, it shows *what it's asking* (e.g. a command to approve).
- **Jump to the terminal** — click a session to bring its terminal app to the front.
- **Choose your icon** — Bird, Spark, the Claude logo, or the Claude crab — in monochrome or Claude orange.
- **Launch at login**, and a one-click **Remove Perch integration** when you're done.

## Requirements

- macOS 13 (Ventura) or later
- [Claude Code](https://claude.com/claude-code)

## Install

1. Download the latest `Perch.dmg` from [**Releases**](https://github.com/ik-labs/perch/releases/latest).
2. Open it and drag **Perch** to your **Applications** folder.
3. Launch Perch. On first run it explains what it sets up and offers notifications.

The app is **signed and notarized by Apple** (Developer ID: Inkryptis Labs LLP), so it opens without Gatekeeper warnings.

## How it works

Perch reads Claude Code's own local state. On first launch it adds two things to `~/.claude/settings.json`, **non-destructively** (it preserves anything you already had):

- **Hooks** — so Perch sees each session's live state as it changes.
- **A status line** — the only place Claude Code reports your 5h / 7d usage.

Everything runs **locally on your Mac** — Perch makes **no network calls**, has **no telemetry**, and nothing about your sessions ever leaves your machine.

## Uninstall

- **Detach the integration:** ⚙︎ menu → **Remove Perch integration** (restores your previous settings), then drag Perch to the Trash.

## Feedback & bugs

- 🐛 [Open an issue](https://github.com/ik-labs/perch/issues/new/choose)
- 💬 [Discussions](https://github.com/ik-labs/perch/discussions) for questions & ideas

---

<div align="center">
<sub>© 2026 Inkryptis Labs LLP · <em>Claude</em> and the Claude mark are trademarks of Anthropic, used to identify Claude Code sessions.</sub>
</div>
