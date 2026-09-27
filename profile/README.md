# harnsy

<img width="1452" height="563" alt="image 27" src="https://github.com/user-attachments/assets/07e62ad8-0f64-40c3-9907-0ceacd19276d" />

harnsy turns Claude Code, Codex and OpenCode into a development team. You talk to one lead agent; it hires the roles it needs — an analyst, developers, a tester — hands out the tasks, and brings back questions and finished work.

→ **[harnsy.dev](https://harnsy.dev)**

## Why

With several agents, you end up in five chats, copying answers between windows. harnsy gives every agent one role, lets them talk to each other directly, and gives you one way in.

- **One way in: the lead. Even from your phone.** You talk to one lead agent; it hands out tasks and brings back only questions and finished work. From your phone, through Claude Code's Remote Control.
- **Messages land right in the session.** Each harness's own delivery mechanism: no inbox polling, no fake keystrokes.
- **The best from every model.** Let Codex review what Claude wrote. Hand routine work to a local or low-cost model through OpenCode.
- **The company stays. The agents change.** When an agent's context runs low, it writes a handover note and a fresh agent takes the same role. The old one stays on as a consultant.
- **You're called in only when you're needed.** A dashboard and a tray show what waits for you: a task to accept, a permission to grant.
- **Every agent's terminal in one place.** Agents run in real terminals under tmux (or WezTerm). The dashboard shows each one live: open an agent's terminal from any page, watch it work, type into it when you need to. Agents on a server show up in your laptop's dashboard too (full edition).
- **See how they work together.** The Links graph shows who talks to whom: the lead in the centre, teams as boxes, lines for every conversation, projects that ask each other for help. Open any line to read the messages behind it, and spot the chatter that shouldn't be there.
- **Nothing new to learn.** harnsy connects the harnesses you already use; your settings, skills and subscriptions stay as they are. It runs on your machine.

## Your AI company

harnsy organises agents the way a company organises people.

- **Agents organise into teams.** Each project gets its own team: the lead at the top, the roles under it, every seat held by a live agent. A team opens together, in its own terminal tab, and comes back together after a reboot. Teams of different projects can ask each other for help.
- **A company, projects, roles.** The company keeps a catalog of roles — lead, analyst, developer, tester, anything you need. Each project adds its own instructions to a role: the repository, the stack, how to build and test, which skills to use.
- **Every role has its own prompt, versioned.** A role is a document: duties, deliverable, goals with a *why*, project instructions. Change it and a new version is saved; the agent holding the role is told to re-read it.
- **Starting from zero is a conversation.** Point an agent at your project and ask it to set harnsy up. It interviews you about how you work, reads the project's rules, drafts the roles and goals, and hands you the lead's invite.
- **A new session joins by invite.** One message with a one-time link seats an agent in a role. It reads its role document and starts already briefed. The lead opens new sessions for its roles itself (in WezTerm or tmux) and replaces an agent whose context runs low.

## Install

Tell your agent:

```text
Install harnsy following https://harnsy.dev/llms.txt
```

Or run it yourself — Linux and macOS:

```sh
curl -fsSL https://harnsy.dev/install.sh | sh
```

Windows (PowerShell):

```powershell
irm https://harnsy.dev/install.ps1 | iex
```

The installer shows every change to your settings files and asks before each one. `harnsy uninstall` puts everything back.

This installs the free demo build: 1 project, up to 10 agents at once, one machine. The full build has no limits.

## Repositories

- **[app](https://github.com/harnesy/app)** — downloadable builds for Linux, macOS and Windows, with checksums. The installers above take the latest release from here.
