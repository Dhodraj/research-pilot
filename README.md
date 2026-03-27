# ResearchPilot

AI-powered research automation agent that orchestrates multi-step research workflows — from topic intake and intelligent web sourcing to insight synthesis and structured output generation.

## What It Does

ResearchPilot automates the tedious parts of research by chaining specialized AI agents together in a pipeline. Given a topic or question, it searches across multiple sources, synthesizes findings using Claude, and produces structured deliverables with human-in-the-loop approval.

## Features

- **Agent Orchestration** — Coordinates multiple research agents working in parallel across different sources
- **Multi-Source Search** — Searches technical docs, academic papers, forums, blogs, and MCP-connected data sources simultaneously
- **Research Tracking** — Creates and maintains Google Sheets trackers with deduplication and source validation
- **Insight Synthesis** — Uses Claude to synthesize raw findings into actionable insights with citations
- **Human Approval Gate** — Keeps a human in the loop before finalizing outputs
- **Structured Output** — Generates research reports, comparison matrices, and presentation-ready outlines

## Architecture

```
Research Topic / Question
        |
  Agent Orchestrator
        |
  Multi-Source Search Agents  (parallel)
        |
  Insight Synthesis (Claude)
        |
  Human Approval Gate
        |
  Structured Output Gen
```

## Tech Stack

- **LLM Integration** — Claude (Anthropic) for synthesis and reasoning
- **Agent Framework** — MCP (Model Context Protocol) connectors for tool integration
- **Data Sources** — Web search, academic sources, documentation, Google Drive, Google Sheets
- **Output Formats** — Markdown reports, spreadsheet trackers, presentation outlines

## Modules

| File | Purpose |
|------|---------|
| `searcher.txt` | Core research agent prompt — multi-source search with automated tracking |
| `claude_cowork.json` | Excalidraw architecture diagram of the agent pipeline |

## Status

Early-stage. Core prompt engineering and architecture design complete. Full agent pipeline implementation in progress.

## License

MIT
