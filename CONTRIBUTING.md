# Setup for Agentic Coding tools

When contributing to r-xla and when working with coding AGENTS, it is important to have the following file structure:

```
<parent-dir>/
  pjrt/
  stablehlo/
  anvil/
  tengen/
  xlamisc/
  claude-config/
```

This is, because each repository's AGENTS.md loads @../claude-config/CLAUDE.md for some common information about r-xla.
Note that claude-config is also a skill marketplace (WIP), so you might want to register it with your coding tool.
In addition to these r-xla skills, repositories can also have their own, project-specific, skills.

