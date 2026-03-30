# Subagent specs

Place one file per subagent (e.g. `reviewer.md`, `test-runner.md`).

Suggested front matter (optional):

```yaml
---
name: reviewer
tools: [read_file, grep, run_terminal_cmd]
---
```

Body: role, inputs, outputs, escalation rules, and how this differs from **Blackwall runtime agents** (detection/protection/MCP tools in separate repos).
