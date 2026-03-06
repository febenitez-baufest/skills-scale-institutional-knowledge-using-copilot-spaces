# OctoAcme Project Management Docs

This README is the entry point to OctoAcme's project management process documentation. It provides a brief overview of how OctoAcme runs projects and links to the detailed guides for each phase and topic.

---

## Table of Contents

- [Overview](#overview)
- [Key Workflows](#key-workflows)
- [Personas & Roles](#personas--roles)
- [Communication Strategies](#communication-strategies)
- [Quality Assurance Practices](#quality-assurance-practices)
- [Process Documentation](#process-documentation)

---

## Overview

OctoAcme uses a structured, iterative approach to project management that prioritizes customer value, clear ownership, and continuous improvement. Projects move through well-defined phases — from initiation through retrospective — with consistent artifacts, communication cadences, and quality gates at every stage. The goal is to deliver reliable software incrementally, with full transparency for stakeholders and minimal unplanned work for the team.

Across all phases, a single source of truth (the project README or release doc) keeps everyone aligned, and escalation paths ensure that blockers are resolved quickly. Retrospectives close each project cycle, feeding learnings back into the next iteration.

---

## Key Workflows

OctoAcme projects follow this lifecycle:

1. **Initiation** — Define the problem statement, identify stakeholders, and establish a high-level timeline via a Project Charter.
2. **Planning** — Scope the work, define milestones and dependencies, build the backlog, and assess initial risks.
3. **Execution & Tracking** — Build and test in iterative sprints, using daily standups, PR reviews, and continuous integration to maintain quality and visibility.
4. **Release & Deployment** — Validate acceptance criteria, run CI and security scans, deploy through a checklist-driven process (staging → production), and announce the release to stakeholders.
5. **Retrospective & Continuous Improvement** — Capture learnings, define action items, and feed improvements back into future project cycles.

---

## Personas & Roles

| Role | Primary Responsibility |
|---|---|
| **Project Manager (PM)** | Coordinates delivery, schedules, risks, and cross-team communication |
| **Product Manager (PdM) / Product Lead** | Defines outcomes, owns the roadmap and backlog, measures success |
| **Developers** | Implement features, write tests, participate in design and code reviews |
| **QA / Testing** | Validate quality and acceptance criteria across all delivery stages |
| **Stakeholders** | Provide inputs, approvals, and receive regular status updates |

See [Roles & Personas](octoacme-roles-and-personas.md) for detailed responsibilities and communication patterns for each role.

---

## Communication Strategies

OctoAcme maintains regular, predictable communication across all stakeholder groups:

- **Cadences:** twice-weekly standups for the delivery team, weekly PM + PdM sync, and monthly stakeholder updates.
- **Single source of truth:** the project README or release document holds current status; all updates flow there first.
- **Stakeholder updates:** milestone-based or weekly summaries using a consistent status template (progress, next steps, risks/blockers, decisions needed).
- **Escalation paths:** issues escalate from the team level → PM → Product Lead → Sponsor; security incidents follow the security incident runbook and notify the Security on-call team directly.

See [Risk Management & Communication](octoacme-risks-and-communication.md) for templates and escalation details.

---

## Quality Assurance Practices

Quality is built into every phase of delivery:

- **PR workflow:** all changes go through pull request review before merging; acceptance criteria are defined upfront and validated before a PR is closed.
- **Continuous integration (CI):** automated pipelines run tests and security scans on every PR; releases require passing CI and security scans as a pre-release gate.
- **Testing expectations:** developers write and maintain tests; QA validates acceptance criteria; smoke tests are run in staging before each production deployment.
- **Security scanning:** included as part of the CI pipeline and required before any release is approved.
- **Release checklist & rollback/incident approach:** deployments follow a structured checklist (staging smoke tests → production deploy → post-deploy verification → stakeholder announcement); if a deployment fails, the team triggers incident response, rolls back to the last known-good release, and schedules a blameless retrospective.

See [Release & Deployment Guide](octoacme-release-and-deployment.md) for the full checklist and rollback playbook.

---

## Process Documentation

| Document | Description |
|---|---|
| [Project Management Overview](octoacme-project-management-overview.md) | High-level principles, roles, artifacts, and lifecycle summary |
| [Project Initiation Guide](octoacme-project-initiation.md) | Problem statement, stakeholder identification, project charter |
| [Project Planning Guide](octoacme-project-planning.md) | Scope, milestones, backlog, risk assessment |
| [Execution & Tracking Guide](octoacme-execution-and-tracking.md) | Sprints, standups, PR flow, progress tracking |
| [Risk Management & Communication Guide](octoacme-risks-and-communication.md) | Risk register, communication templates, escalation paths |
| [Release & Deployment Guide](octoacme-release-and-deployment.md) | Release types, pre-release requirements, deployment checklist, rollback playbook |
| [Retrospective & Continuous Improvement Guide](octoacme-retrospective-and-continuous-improvement.md) | Retrospective formats, action item tracking, improvement loops |
| [Roles & Personas](octoacme-roles-and-personas.md) | Detailed role definitions and communication patterns |
