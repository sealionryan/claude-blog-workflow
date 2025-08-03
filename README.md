# 📰 Claude-Powered Blog Workflow

An automated, multi-agent system that transforms a single keyword into a fully-written, SEO-optimized Markdown article. Built on the [Claude Sub-Agents](https://github.com/webdevtoday/claude-agents) framework with a master-sub-agent architecture.

## 🚀 Quick Start

```bash
# Install the Claude Sub-Agents CLI (once per machine)
npm install -g @webdevtoday/claude-agents
claude-agents install --project

# Run the complete workflow
> /blog-orchestrate

# Provide your brief:
# - search_term: keyword or working title
# - context: background, tone, audience
# - keywords: optional CSV of target SEO terms
# - allow_web: true to sample SERPs for research
```

The master **Blog Workflow Orchestrator** coordinates all sub-agents and returns a finished article plus metadata files.

## 🧩 Agent Architecture

| Agent | Command | Purpose |
|-------|---------|---------|
| **Orchestrator** | `/blog-orchestrate` | Master agent - manages complete workflow |
| SEO Data Researcher | `/seo` | Research keywords and competitive landscape |
| Outline Maker | `/outline` | Create structured content outlines |
| Blog Writer | `/blog` | Write engaging, SEO-optimized content |
| Content Reviewer | `/blog-review` | Edit, polish, and optimize final drafts |

## 📁 Project Structure

```
blog-writer/
├── README.md                    # This file
├── CLAUDE.md                    # Project rules and instructions
├── .gitignore                   # Git ignore patterns
├── workflow.jpg                 # Visual workflow diagram
└── agents/                      # Agent documentation and configs
    ├── AGENTS.md               # Comprehensive agent reference
    ├── README.md               # Quick agent overview
    ├── PRD_blog_workflow.md    # Product requirements
    ├── WORKFLOW_QUICK_REFERENCE.md
    ├── TASKS_blog_workflow.md
    └── .claude/                # Agent prompt files and commands
```

## ✨ Key Features

- **Master-Sub-Agent Architecture**: Clear separation of duties with quality gates
- **Flexible Content Structure**: Adaptive H2/H3 hierarchy based on content needs
- **Human-in-the-Loop**: Optional review points for editorial control
- **SEO Optimization**: Built-in keyword research and optimization
- **Extensible Design**: Easy to add new agents and capabilities

## 🛠️ Requirements

- Node.js and npm
- Claude Sub-Agents CLI (`@webdevtoday/claude-agents`)
- Claude API access

## 📖 Documentation

- **[AGENTS.md](agents/AGENTS.md)** - Complete agent documentation and usage guide
- **[WORKFLOW_QUICK_REFERENCE.md](agents/WORKFLOW_QUICK_REFERENCE.md)** - One-page workflow cheat sheet
- **[PRD_blog_workflow.md](agents/PRD_blog_workflow.md)** - Product requirements document

## 🎯 Success Metrics

- **Efficiency**: < 10 minutes from keyword to publication-ready article
- **Quality**: ≥ 80% reviewer approval rate on first draft
- **SEO Performance**: Target 1,500-2,500 word articles with 1-2% keyword density

## 📈 Future Enhancements

- Automated image generation and suggestions
- Social media content generation
- Performance metrics collection
- CMS integration capabilities

## 📄 License

MIT © 2025

---

Made with ❤️ and Claude AI