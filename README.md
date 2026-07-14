<div align="center">

# 🐦 Perch

**Watch every Claude Code and Codex session from your menu bar.**

Running several agents across terminals and projects? Perch shows which are working, which are waiting on you, and which are idle — so you stop shuffling between windows to find the one that's blocked.

[**⬇ Download for macOS**](https://github.com/ik-labs/perch/releases/latest) · macOS 13+ · Apple silicon

</div>

---

## Screenshots

<!--
Drop the images into assets/ and uncomment. Capture them with the demo fleet
(scripts/demo-fleet.sh) — it runs Perch against a sandboxed HOME with a fake fleet, so
no real project names, commands, costs, or usage end up in a public image.

| | |
|:--:|:--:|
| ![The fleet](assets/panel.png) | ![Needs you](assets/menubar.png) |
| **Every session, grouped by what needs you** | **The menu bar tells you without opening anything** |
| ![Approve from a notification](assets/notification.png) | ![On your phone](assets/ios-approve.png) |
| **Approve a tool call without leaving your editor** | **…or from the couch** |
-->

> _Screenshots landing shortly._

---

## What it does

**Sees everything, without setup.** Every Claude Code and Codex session — running, waiting on you, idle, done — sorted so whatever's blocked floats to the top. Subagents nest under their parent. Task checklists show what the agent is actually working through.

**Tells you what each agent is doing.** The live command, the in-progress task, the model (including 1M-context), reasoning effort, live context %, and cost.

**Answers agents without switching windows.** When an agent asks to run something, Perch's notification carries **Allow / Deny** — approve it without leaving what you're doing. Ignore it and your terminal prompts as usual; Perch never acts on its own.

**Follows you to your phone.** The [iOS companion](#iphone-companion) mirrors the fleet and alerts you when an agent needs you — on the same Wi-Fi, or across the world over Tailscale.

**Shows your limits.** Your 5-hour and 7-day usage, with reset timers — the numbers Claude Code only reports to its status line.

**Jumps to the terminal.** Click a session to bring its terminal to the front.

**Gets out of the way.** Launch at login, pick your icon (bird, spark, the Claude logo, or the crab — mono or Claude orange), and a one-click **Remove Perch integration** when you're done.

## iPhone companion

Pair once by scanning a QR code. Then:

- **The whole fleet in your pocket** — who's waiting, who's working, what each agent is doing.
- **Push alerts when an agent needs you**, even with the app closed.
- **Works away from home.** On your Wi-Fi it connects directly. Off it, Perch reaches your Mac over [Tailscale](https://tailscale.com) — your devices talk to each other, not through anyone's server.

The companion is in TestFlight. [Ask for an invite](https://github.com/ik-labs/perch/discussions).

## Requirements

- macOS 13 (Ventura) or later, **Apple silicon**
- [Claude Code](https://claude.com/claude-code) and/or [Codex](https://developers.openai.com/codex/cli/)

## Install

1. Download the latest **`Perch.dmg`** from [Releases](https://github.com/ik-labs/perch/releases/latest).
2. Open it, drag **Perch** to **Applications**.
3. Launch it. On first run it explains what it sets up.

Signed and notarized by Apple (Developer ID: Inkryptis Labs LLP), so it opens with no Gatekeeper warnings. Perch keeps itself up to date after that — updates are signed and verified before they install.

Perch is a paid app; you'll be asked for a licence key on first launch.

## Privacy

Your sessions stay on your Mac. Specifically:

| | |
|---|---|
| **Session data** (projects, commands, tasks, costs) | Stays local. Never sent anywhere, unless you turn on the iPhone companion. |
| **iPhone companion** (optional) | Your Mac talks **directly to your phone** — encrypted, device to device, over your own network or your own Tailscale network. It does not pass through us. |
| **Push alerts** (optional) | To reach your phone when the app is closed, Apple requires a server. The alert text (project name, what the agent is asking) passes through our relay to Apple's push service. Turn the toggle off and nothing is sent. |
| **Licence check** | Your licence key is verified with our payments provider. |
| **Update check** | Perch asks for a version file. Nothing about you is sent. |
| **Analytics / telemetry** | **None.** There is no tracking in Perch, of any kind. |

## Uninstall

⚙︎ → **Remove Perch integration** (restores your previous `settings.json`), then drag Perch to the Trash.

## Feedback

- 🐛 [Report a bug](https://github.com/ik-labs/perch/issues/new/choose) — or use ⚙︎ → **Report an Issue…** in the app, which fills in your version for you
- 💬 [Discussions](https://github.com/ik-labs/perch/discussions) for questions and ideas

---

<div align="center">
<sub>© 2026 Inkryptis Labs LLP · <em>Claude</em> and the Claude mark are trademarks of Anthropic, used to identify Claude Code sessions.</sub>
</div>
