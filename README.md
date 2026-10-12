# Project Discovery & Delivery

**A general-purpose Agent Skill for clarifying project goals, asking adaptive follow-up questions, building a shared project brief, and deciding when to plan or execute.**

[简体中文说明](README.zh-CN.md)

## Why this Skill?
Many project requests begin with an idea rather than a complete specification. Starting too early can lead to avoidable rework; asking too many questions can make the process feel like paperwork.

Project Discovery & Delivery aims for a better balance: **ask the fewest useful questions needed to understand the direction, then move forward with confidence.**

## What it does
- Discovers goals, audience, deliverables, constraints, and success criteria.
- Asks short, adaptive follow-up questions.
- Offers recommendations and sensible defaults when the user is unsure.
- Respects delegation such as “you decide” or “just do it.”
- Separates confirmed decisions, assistant assumptions, and open questions.
- Maintains a lightweight brief for multi-step projects.
- Knows when to stop asking and start executing.
- Supports many project types rather than one narrow workflow.

## Example use cases
- “Help me make a presentation about online safety.”
- “I want to build a portfolio website.”
- “Design a poster for a school competition.”
- “Help me write a research report.”
- “Analyze this dataset and explain what it means.”

## Design principle
> Project Discovery does not aim to maximize the number of questions. It aims to minimize avoidable misunderstanding before execution.

## Package contents
```text
project-discovery-skill/
├── SKILL.md
├── README.md
├── README.zh-CN.md
├── LICENSE
├── CHANGELOG.md
├── CONTRIBUTING.md
├── CODE_OF_CONDUCT.md
├── references/
├── tests/
└── docs/
```

## Installation
This repository follows a common Agent Skill pattern: instructions in `SKILL.md`, supporting guidance in `references/`. Exact installation paths and discovery behavior depend on the host platform. See [Installation guide](docs/installation.md) and [Compatibility notes](docs/compatibility.md).

## Testing
Manual behavioral test scenarios cover vague requests, delegation, skipped questions, conflicts, clear specifications, and scope changes. See [`tests/test-cases.md`](tests/test-cases.md). These are scenario-based checks, not an automated benchmark; behavior can vary by model and host platform.

## Limitations
- This is an instruction-based Skill, not a guarantee that every platform will discover or follow it identically.
- It does not itself provide tools, integrations, deployment, or persistent storage; these depend on the host agent.
- Autonomous execution remains subject to user authorization, safety requirements, platform rules, and actual capabilities.

## Contributing
Bug reports, examples, and improvements are welcome. See [`CONTRIBUTING.md`](CONTRIBUTING.md).

## License
Released under the MIT License. See [`LICENSE`](LICENSE). Before publishing, replace the copyright-holder placeholder with the name or organization you want to use.

## Language
The Skill is written in English for broad reuse and includes a Simplified Chinese README. Contributions in either English or Chinese are welcome.
