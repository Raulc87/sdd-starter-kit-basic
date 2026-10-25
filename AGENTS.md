# AGENTS.md

## Purpose

This repository follows Spec-Driven Development (SDD), basic edition.

The goal is to turn an idea into an approved, consistent plan: requirements, functional requirements, decisions, user stories and a first sprint plan. Code comes later and is not covered by this edition.

## Workflow

Idea -> Discovery -> Project spec (requirements) -> Feature specs (functional requirements) -> ADRs -> User stories -> Sprint 001 plan

Do not skip a stage. Each stage builds on the approved one before it.

## Source-of-truth priority

When sources conflict, use this order:

1. Approved project spec and feature specs
2. Approved ADRs
3. User stories and acceptance criteria
4. Sprint plan
5. Informal comments or assumptions

If a later document conflicts with an approved spec, the spec wins unless the spec is explicitly changed.

## Document map

[`PROJECT_CONTEXT.md`](PROJECT_CONTEXT.md) lists the project's documents and their paths. Standard locations:

| Document | Path | Required |
|---|---|---|
| Project context | [`PROJECT_CONTEXT.md`](PROJECT_CONTEXT.md) | Always |
| Project spec (requirements) | `docs/specs/PROJECT_SPEC.md` | Always |
| Feature specs (functional requirements) | `docs/specs/FEATURE_SPEC_<name>.md` | For each feature that needs more detail than the project spec |
| ADRs | `docs/decisions/ADR-<NNN>_<TITLE>.md` | When a decision has real alternatives |
| User stories | `docs/specs/USER_STORIES.md` | Always |
| Sprint plan | `docs/sprints/SPRINT_001.md` | Always |

Templates end in `_TEMPLATE.md`. To use one, copy it to the path above without the `_TEMPLATE` suffix. ADR templates become `docs/decisions/ADR-<NNN>_<TITLE>.md` with the next free number.

## Rules

- **Do not invent requirements.** Ask, or record the point as an open question. This includes copy, prices, legal terms and credentials.
- **Requirements first.** Every functional requirement traces to a goal in the project spec, every user story to a requirement, and every acceptance criterion is testable (Given / When / Then).
- **Decisions are recorded.** A choice with real alternatives (stack, hosting, data storage, integrations) gets an ADR with the options considered and the reason for the choice.
- **Changes go spec first.** If a requirement changes, update the spec first, then the stories, then the sprint plan.
- **The human owner approves.** Each document is proposed for review, and the owner approves it before the next stage builds on it.
- **Sprint 001 is a plan, not code.** It selects stories, sets a goal and a demonstrable deliverable, and lists the entry conditions. Implementing it is outside this edition.

## Full edition

Implementation with agents, review, security, and release are part of the full SDD Starter Kit by DigitalStrike: https://digitalstrike-solutions.com
