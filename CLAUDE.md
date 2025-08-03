# Claude Agents Project Rules

This project uses the Claude Agents pattern.  **Every time you (or any automated process) do work that involves agents or sub-agents, you must first load and reference the canonical rules file located at:

```
agents/AGENTS.md
```

That file defines the conventions, code snippets, and best-practice guidelines that govern how all agents and sub-agents in this repository are authored, named, documented, and tested.

## Mandatory Rule

> **Always load and follow the rules in `agents/AGENTS.md` for every request that touches agents or sub-agents.**

Failing to do so will result in agents that do not conform to the required standards.

## Next Steps

The upcoming work will create three sub-agents ("SEO Data Researcher", "Outline Maker", and "Blog Writer") that follow the workflow diagram provided.  When implementing them, remember to:

1. Re-read `agents/AGENTS.md` for the correct folder structure, metadata format, and implementation details.
2. Keep this CLAUDE.md file in the repository root so that any toolchain or CI step can quickly verify that the rule is acknowledged.