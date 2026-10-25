# SDD Starter Kit (Basic)

A free starter kit for Spec-Driven Development (SDD): it turns an idea into requirements, functional requirements, recorded decisions, user stories and a first sprint plan, before any code is written.

## What it covers

1. **Idea and discovery:** a structured conversation that collects the goal, audience, scope, data and constraints.
2. **Requirements:** `docs/specs/PROJECT_SPEC.md`, the product-level requirements.
3. **Functional requirements:** `docs/specs/FEATURE_SPEC_<name>.md`, one per feature that needs detail.
4. **Decisions:** `docs/decisions/ADR-<NNN>_<TITLE>.md`, one per decision with real alternatives.
5. **User stories:** `docs/specs/USER_STORIES.md`, with testable acceptance criteria.
6. **Sprint plan:** `docs/sprints/SPRINT_001.md`, the first sprint: goal, selected stories and a demonstrable deliverable.

The rules are in [`AGENTS.md`](AGENTS.md). The project's document list lives in [`PROJECT_CONTEXT.md`](PROJECT_CONTEXT.md).

## How to start

1. Create a repository from this one (**Use this template**, or copy the files).
2. Open a Claude Code session on it and run **`/project-kickoff`**. The skill runs discovery with you and proposes each document in order, ending with the Sprint 001 plan. It writes no code.
3. Review and approve each document before the next one is written.

Without Claude Code, follow the same order by hand with the templates in [`docs/`](docs/) (files ending in `_TEMPLATE.md`).

## Templates

| Template | Becomes |
|---|---|
| [`PROJECT_CONTEXT.md`](PROJECT_CONTEXT.md) | Filled in place |
| [`docs/specs/PROJECT_SPEC_TEMPLATE.md`](docs/specs/PROJECT_SPEC_TEMPLATE.md) | `docs/specs/PROJECT_SPEC.md` |
| [`docs/specs/FEATURE_SPEC_TEMPLATE.md`](docs/specs/FEATURE_SPEC_TEMPLATE.md) | `docs/specs/FEATURE_SPEC_<name>.md` |
| `docs/decisions/ADR_TEMPLATE.md` | `docs/decisions/ADR-<NNN>_<TITLE>.md` |
| [`docs/specs/USER_STORIES_TEMPLATE.md`](docs/specs/USER_STORIES_TEMPLATE.md) | `docs/specs/USER_STORIES.md` |
| [`docs/sprints/SPRINT_PLAN_TEMPLATE.md`](docs/sprints/SPRINT_PLAN_TEMPLATE.md) | `docs/sprints/SPRINT_001.md` |

## License and attribution

© 2026 DigitalStrike Solutions. Licensed under CC BY 4.0.

This edition is licensed under the Creative Commons Attribution 4.0 International License (CC BY 4.0): see `LICENSE`. You may use, share and adapt it, including commercially, as long as you give appropriate credit.

Ready-to-copy attribution line:

> Based on the SDD Starter Kit (Basic) by DigitalStrike - https://digitalstrike-solutions.com

When you share the kit itself or material adapted from it, CC BY 4.0 also asks for the license and a link to the source, and for saying whether you changed it. Copy this complete block:

> Based on the SDD Starter Kit (Basic) by DigitalStrike - https://digitalstrike-solutions.com
> © 2026 DigitalStrike Solutions
> Source: https://github.com/Raulc87/sdd-starter-kit-basic
> Licensed under CC BY 4.0: https://creativecommons.org/licenses/by/4.0/
> Changes: <none, or a short description of what you changed>

## Full edition by DigitalStrike

This basic edition stops at the plan. The full SDD Starter Kit by DigitalStrike takes the project from the Sprint 001 plan to delivery: implementation with agents, independent review, security, and releases. To learn more or work with DigitalStrike: https://digitalstrike-solutions.com

## Versions

This repository is published from DigitalStrike's full kit, so changes are made there, not in this repository. Each version carries the same tag as the full kit release it comes from.
