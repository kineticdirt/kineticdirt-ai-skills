# kineticdirt-ai-skills

Personal library of **Cursor / Claude skills**, **subagent specs**, and related playbooks. This repo is **separate** from [Blackwall](https://github.com/kineticdirt) workshop projects (agents, MCP servers, retrieval eval, etc.).

## Layout

| Path | Purpose |
|------|---------|
| `skills/` | One folder per skill; each contains `SKILL.md` (Cursor skill format). |
| `subagents/` | Markdown (or JSON) definitions: role, tools, boundaries, handoff rules. |
| `registry.yaml` | Machine-readable index: id, title, tags, path. |

## Using skills in Cursor

Point Cursor at a skill folder, or symlink/copy `skills/<name>/` into your Cursor skills directory. See [Cursor Agent Skills](https://cursor.com/docs) for the current install path on your OS.

## Relation to Blackwall

- **Blackwall** = runnable code (agents, gateways, MCP, eval harnesses), often published as its own repos per folder.
- **This repo** = portable **instructions and patterns** for AI assistants, not application code.

## Contributing (you)

Keep secrets out of git. Prefer tags in `registry.yaml` over deep coupling between skills.
