# OpsForge Architecture

## Purpose

This document explains how OpsForge is organized and how its components work together.

OpsForge is designed as a collection of focused documents rather than one large prompt. Each document has a single responsibility, making the project easier to understand, maintain, and extend.

---

# Repository Structure

```
opsforge-agent/
│
├── README.md
├── agent/
│   ├── operating-principles.md
│   ├── guardrails.md
│   ├── capabilities.md
│   ├── response-template.md
│   └── system-prompt.md
│
├── docs/
│   └── architecture.md
│
├── playbooks/
│
└── tests/
```

---

# Component Overview

## README.md

Purpose:

Describes the project, its goals, and its intended audience.

Question it answers:

> "What is OpsForge?"

---

## operating-principles.md

Purpose:

Defines the engineering philosophy behind OpsForge.

Question it answers:

> "How should OpsForge think?"

Examples include:

- Evidence before assumptions
- Lowest-risk-first
- Verification before resolution

---

## guardrails.md

Purpose:

Defines the safety boundaries.

Question it answers:

> "What should OpsForge never do?"

Examples include:

- Avoid destructive recommendations
- Protect sensitive information
- Respect enterprise policies

---

## capabilities.md

Purpose:

Defines what OpsForge currently supports.

Question it answers:

> "What can OpsForge help with?"

This document also defines future capabilities and current limitations.

---

## response-template.md

Purpose:

Defines the standard structure for troubleshooting responses.

Question it answers:

> "How should OpsForge communicate?"

This ensures responses remain consistent regardless of the topic.

---

## system-prompt.md

Purpose:

Combines the principles, guardrails, capabilities, and response standards into a single set of operating instructions.

Question it answers:

> "How should OpsForge behave during every interaction?"

This is the primary document used when configuring the AI agent.

---

# Future Components

## playbooks/

The playbooks folder will contain detailed troubleshooting guides for specific technologies.

Examples:

- Windows Update
- Networking
- Printing
- Active Directory
- Entra ID
- Hardware diagnostics

Playbooks provide domain-specific knowledge while the system prompt provides general behavior.

---

## tests/

The tests folder will contain realistic troubleshooting scenarios used to evaluate OpsForge.

Each test should verify that the agent:

- Follows the troubleshooting workflow
- Applies the decision-making framework
- Uses the correct response template
- Produces accurate documentation
- Respects the defined guardrails

---

# Design Principles

OpsForge follows several architectural principles.

## Separation of Concerns

Each document has one clear responsibility.

This keeps the project organized and easier to maintain.

---

## Reusability

Individual components should be reusable across future versions of OpsForge.

---

## Maintainability

Updates should affect only the relevant component whenever possible.

---

## Scalability

New technologies and troubleshooting playbooks should be added without requiring major changes to the existing architecture.

---

# Summary

OpsForge is built as a modular AI engineering project.

Rather than relying on one large prompt, it separates behavior, safety, capabilities, communication, and documentation into independent components that work together to produce consistent and professional technical assistance.
