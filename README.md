# SkillSet by Me

82 portable agent skills in the open `SKILL.md` format: engineering workflow, game development, UI/UX design, browser testing, codebase understanding, and token and context efficiency.

**[SKILLS.md](SKILLS.md)** is the full list: one line per skill saying when to use it, with a direct link.

## Using it

| Agent | How |
|---|---|
| Claude Code | Copy the folders: `cp -r skills/* ~/.claude/skills/` (all projects) or into `.claude/skills/` (one project). |
| Replit Agent | Copy the folders into `.agents/skills/` in the Repl. |
| Codex, Cursor, Copilot, Windsurf, Gemini CLI and other repo-aware agents | Clone or add this repo to the workspace. They read `AGENTS.md`, which points them at `SKILLS.md`. |
| Web chat agents (ChatGPT, Claude.ai, Gemini, etc.) | Paste the link to `SKILLS.md` (or the file itself) and tell the agent: "Use these skills. Fetch a skill's SKILL.md link only when its description fits the task." |

## Layout

```
skills/<skill-name>/SKILL.md      # instructions (frontmatter: name, description)
skills/<skill-name>/references/   # optional docs the skill loads on demand
skills/<skill-name>/scripts/      # optional helper scripts
SKILLS.md                         # the index
AGENTS.md                         # entry point for agents that auto-read it
```

Some skills mention tools a given agent may not have (for example Chrome DevTools MCP). Where a tool is missing, the agent should follow the skill's fallback or skip that step.
