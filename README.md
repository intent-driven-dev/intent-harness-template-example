# Spec-Driven Development: Engineering with Intent (Manning Publications) Companion Code

This repository contains companion code for the book [_Spec-Driven Development: Engineering with Intent (Manning Publications)_](https://hubs.ly/Q04vSdlS0).

<img width="1584" height="396" alt="linkedin profile banner" src="https://github.com/user-attachments/assets/6e80ce16-4daa-454d-a685-83ec0e0a146f" />

# Intent Harness Template

This repository contains the companion code for the Chapter 6 in Intent-Driven Software Engineering book.

A spec-driven development (SDD) template using [Intent Harness Capabilities](https://github.com/intent-driven-dev/intent-harness-capabilities) and  **OpenSpec 1.14.0** (verified installed version).

## Workflow

The custom [`linear-driven` schema](openspec/schemas/linear-driven/schema.yaml), sourced from [intent-harness-capabilities](https://github.com/intent-driven-dev/intent-harness-capabilities), connects OpenSpec changes to Linear issues and requires Linear MCP access.

Proposal → specs/design → tasks → apply → verify/archive. Each proposal is associated with a Linear issue. Authoring tasks moves it to Todo; implementation moves it to In Progress and requests human review on completion.

## Skills and agent

- [`glossary`](.agents/skills/glossary/SKILL.md) guides proposal terminology; [`adrs`](.agents/skills/adrs/SKILL.md) guides architectural decisions during design.
- The [`senior-engineer` agent](.codex/agents/senior-engineer.toml) handles implementation, using the TypeScript best-practices and unit-testing skills when relevant.

[`openspec/config.yaml`](openspec/config.yaml) selects the schema and connects proposal, design, and apply to these capabilities.

Validate the installed schema with `openspec schema validate linear-driven`.
