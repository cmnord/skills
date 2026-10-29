# skills

Agent skills I use. Each folder under `skills/` is a standard
[Agent Skills](https://agentskills.io) `SKILL.md` skill, and the repo is also a
plugin marketplace for Claude Code and Codex.

## Install

**ChatGPT:** paste this into a chat:

> @skill-creator Create a skill exactly from https://raw.githubusercontent.com/cmnord/skills/main/skills/help-me-do-this/SKILL.md, keeping the name, description, and text unchanged.

**Claude Code:** run this in Claude Code:

```
/plugin install cmnord-skills --marketplace cmnord/skills
```

**Codex:**

```sh
codex plugin marketplace add cmnord/skills && codex plugin add cmnord-skills@cmnord
```

**Any other agent (Cursor, Copilot, Gemini CLI, ...):**

```sh
npx skills add cmnord/skills
```

## Skills

- [`help-me-do-this`](skills/help-me-do-this/SKILL.md): do as much of a task as possible, then hand back only the remaining steps with exact links, commands, and ready-to-send messages.

## Adding a skill

Add `skills/<name>/SKILL.md` with `name` (matching the folder) and
`description` frontmatter. Both marketplaces pick up everything under `skills/`.
Bump `version` in `.codex-plugin/plugin.json` so Codex installs refresh.
