# OctoAcme Project Management Docs

This README is the entry point to OctoAcme's project management processes. It summarizes our core workflows, roles, communication strategy, and quality assurance practices, and provides direct links to the detailed process documents stored in this repository's docs/ folder.

## Project Management Process Summary
OctoAcme runs projects with an iterative, customer-first approach that emphasizes small, testable increments and clear ownership across the project lifecycle (Initiation → Planning → Execution → Release → Retrospective). Work starts with a lightweight Project One‑pager to validate the problem, define success metrics, identify stakeholders, and confirm the go/no‑go decision. Approved initiatives move into planning where scope is decomposed into prioritized backlog items with acceptance criteria, estimates, and a release/milestone map.

Day-to-day delivery follows explicit workflows and a disciplined pull-request process: teams use a project board (Backlog → Ready → In Progress → In Review → QA → Done), create small PRs that reference issues and acceptance criteria, and require automated CI checks (tests, linting, security scans) plus at least one approval before merging. Risk and dependency management are tracked in a simple risk register and surfaced in regular syncs so cross-team dependencies are escalated promptly.

Roles and responsibilities are separated to reduce single-person risk and speed decisions: Product Managers (PdM) own outcomes and prioritization; Project Managers (PM) coordinate schedules, risks, and stakeholder communication; Developers implement and test; QA validates acceptance; stakeholders provide input and approvals. Each persona maps to concrete artifacts and handoffs so ownership is clear throughout the lifecycle.

Quality assurance and release rigor are layered to reduce production risk: unit and integration tests, end-to-end smoke checks for critical flows, CI security scanning, and manual QA where needed. Releases follow a checklisted approach (pre-release acceptance and CI passing, release notes, rollback/mitigation plan, staging smoke tests, automated deployment where possible, and post-deploy verifications). Retrospectives capture action items that feed back into the backlog for continuous improvement.

## Documentation Links
- [Project Management Overview](docs/octoacme-project-management-overview.md)
- [Project Initiation Guide](docs/octoacme-project-initiation.md)
- [Project Planning](docs/octoacme-project-planning.md)
- [Execution & Tracking](docs/octoacme-execution-and-tracking.md)
- [Risk Management & Communication](docs/octoacme-risks-and-communication.md)
- [Release & Deployment Guide](docs/octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](docs/octoacme-retrospective-and-continuous-improvement.md)
- [Roles and Personas](docs/octoacme-roles-and-personas.md)

## How to use these docs
- Keep the Project One-pager and key artifacts updated in the project repo.
- Use the project README here as the canonical, high-level entry point to process documentation.
- Suggest edits via pull requests; tag the relevant process document in the PR description.
