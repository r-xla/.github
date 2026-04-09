# Contributing

We welcome any feedback in the form of issues or feature requests — please don't hesitate to open one.

If you'd like to contribute a pull request, please:

- Format your R code with [air](https://posit-dev.github.io/air/).
- Use [jarl](https://github.com/r-xla/jarl) for linting.

## Setup for Agentic Coding tools

When contributing to r-xla and when working with coding AGENTS, it is important to have the following file structure:

```
<parent-dir>/
  anvil/
  claude-config/
  pjrt/
  stablehlo/
  tengen/
  xlamisc/
```

This is, because each repository's AGENTS.md loads @../claude-config/CLAUDE.md for some common information about r-xla.
Furthermore, because the packages are interdependent, it's useful for the LLM to be able to easily read relevant
code across the repositories.

Note that claude-config is also a skill marketplace (WIP), so you might want to register it with your coding tool.
In addition to these r-xla skills, repositories can also have their own, project-specific, skills (also WIP).

