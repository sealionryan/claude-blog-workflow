# Test Files Not Included

The `agents/tests/` directory containing sample workflow runs has been excluded from this repository to keep the codebase clean and focused on the core system.

## What Was Here

This directory previously contained:
- Sample brainstorm outputs
- Draft outlines
- H3 suggestions
- Final outlines
- Complete draft articles
- Reviewer feedback

## Running Your Own Tests

To see the system in action:

```bash
# Install the Claude Sub-Agents CLI
npm install -g @webdevtoday/claude-agents
claude-agents install --project

# Run the complete workflow
> /blog-orchestrate
```

This will generate your own test outputs that you can examine locally.