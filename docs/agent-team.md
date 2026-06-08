# Agent team

This project uses a small custom agent team to build Mona's Project Pulse dashboard.

Agents:

- Orchestrator — Claude Opus 4.7 (copilot). Coordinates Planner, Coder, and Designer; breaks work into phases and delegates tasks. Definition: .github/agents/orchestrator.agent.md
- Planner — Claude Opus 4.7 (copilot). Researches the repository, identifies edge cases, and produces ordered implementation steps, file assignments, and validation expectations. Definition: .github/agents/planner.agent.md
- Coder — GPT-5.5 (copilot). Implements code, runnable app support (launch configs, preview), tests, and fixes within scoped files. Definition: .github/agents/coder.agent.md
- Designer — Gemini 3.1 Pro (copilot). Handles UI/UX, accessibility, information hierarchy, and visual design for the Project Pulse frontend. Definition: .github/agents/designer.agent.md

Work is coordinated from the GitHub Copilot CLI running in a Codespace; the learner controls git operations and review.
