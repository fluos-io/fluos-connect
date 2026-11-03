# Fluos Connect

Fluos Connect lets [Fluos](https://www.fluos.io) use your own Claude Code, Codex or Cursor. It's a small menu-bar app that pairs your computer with your Fluos account, so chats in Fluos can use the coding agent you already have installed and signed in to.

## Download

Get the latest version from the [Releases](https://github.com/fluos-io/fluos-connect/releases/latest) page, or from Fluos itself: pick Claude Code, Codex or Cursor in the chat composer and choose "Set up on your computer".

- **macOS** 12 or later, Apple silicon and Intel. Signed and notarized by Apple.
- **Windows**: coming soon.

The app updates itself.

## Setup

1. Install [Claude Code](https://docs.anthropic.com/en/docs/claude-code), [Codex](https://github.com/openai/codex) or [Cursor's CLI](https://cursor.com/cli) and sign in to it. Fluos Connect can also install, update and sign in to them for you.
2. Open the `.dmg` and drag Fluos Connect to Applications.
3. In Fluos, pick your agent in the chat composer and follow the setup steps. Fluos shows a pairing code, and the app asks you to confirm which Fluos account you're pairing with.

## What it does on your computer

- **Runs only when needed.** Fluos opens the app when a chat uses your agent, and the app quits about 3 minutes after no Fluos tab or build needs it. "Start at login and stay open" in the menu keeps it running instead.
- **Uses your own login.** Your agent runs with your existing subscription or API key, on your computer. Fluos never sees your agent's credentials.
- **Keeps a local copy of each project** in `~/.fluos/projects`, so your agent can edit the files. Deleting a project in Fluos removes its copy.
- **Starts your agent only for a turn.** Between turns the app only keeps a connection to Fluos open. The agent stops when the turn ends, when you press Stop, or after 15 minutes without output.

## Uninstall

1. In Fluos, open Settings → Your own agent and remove the computer.
2. Quit Fluos Connect from the menu bar and move it from Applications to the Trash.
3. To remove its data, delete `~/Library/Application Support/Fluos Connect` and `~/.fluos/projects`.

## About this repository

This repository only hosts the signed installers and the update manifest (`latest.json`). The source code is not published here.

Use of Fluos Connect is covered by the [Fluos Terms](https://www.fluos.io/terms) and [Privacy Policy](https://www.fluos.io/privacy). See [LICENSE](LICENSE).

Questions or problems: ask@fluos.io. Security issues: see [SECURITY.md](SECURITY.md).
