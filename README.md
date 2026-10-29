# skills

Agent skills I use. Each folder under `skills/` is a standard `SKILL.md` skill.

## Install

Paste this into ChatGPT (use `$skill-creator` in Codex):

> @skill-creator Create a skill exactly from https://raw.githubusercontent.com/cmnord/skills/main/skills/help-me-do-this/SKILL.md, keeping the name, description, and text unchanged.

Or from a terminal, for Codex, Claude Code, Cursor, and other agents:

```sh
npx skills add cmnord/skills
```

## Skills

- [`help-me-do-this`](skills/help-me-do-this/SKILL.md): do as much of a task as possible, then hand back only the remaining steps with exact links, commands, and ready-to-send messages.
