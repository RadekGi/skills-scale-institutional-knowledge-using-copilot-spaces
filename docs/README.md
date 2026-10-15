# OctoAcme Project Management Docs

This folder contains OctoAcme's project management process documents. Use this README as the single entry point to understand how we initiate, plan, execute, release, and improve work across teams.

Quick links
- Overview: ./octoacme-project-management-overview.md
- Initiation: ./octoacme-project-initiation.md
- Planning: ./octoacme-project-planning.md
- Execution & Tracking: ./octoacme-execution-and-tracking.md
- Risks & Communication: ./octoacme-risks-and-communication.md
- Release & Deployment: ./octoacme-release-and-deployment.md
- Retrospective & Continuous Improvement: ./octoacme-retrospective-and-continuous-improvement.md
- Roles & Personas: ./octoacme-roles-and-personas.md

## Overview
- Purpose: Capture and publish a consistent set of program-level processes so contributors and stakeholders can find, use, and improve how OctoAcme delivers work.
- Scope: Applies to cross-functional projects that deliver product features, services, or integrations.

## End-to-end workflow stages & handoffs

1. Initiation (see ./octoacme-project-initiation.md)
   - Purpose: Surface the problem, define success metrics, identify stakeholders and initial risks.
   - Handoff: Move to Planning when the Project One-pager is complete, stakeholders agree, and team availability is confirmed (Decision Gate).
2. Planning (see ./octoacme-project-planning.md)
   - Purpose: Break approved initiatives into a prioritized backlog, define acceptance criteria and the Definition of Done (DoD), estimate scope, and map milestones.
   - Handoff: Work is handed to the delivery team when backlog items meet DoD and have clear acceptance criteria.
3. Execution & Tracking (see ./octoacme-execution-and-tracking.md)
   - Purpose: Deliver work iteratively, using the project board to track status and run the PR workflow, automated checks, and manual QA as required.
   - Handoff: Items move to Release when acceptance criteria are met, PRs are approved, and QA/sign-off completed.
4. Release & Deployment (see ./octoacme-release-and-deployment.md)
   - Purpose: Perform checklist-driven deployments with smoke tests, monitoring, and rollback/mitigation plans.
   - Handoff: After a successful release, capture release notes and transition to Retrospective.
5. Retrospective & Continuous Improvement (see ./octoacme-retrospective-and-continuous-improvement.md)
   - Purpose: Capture learnings, create action items, and feed improvements back into backlog and process docs.

## Roles & responsibilities (summary)
- Project Manager (PM): coordinates delivery, manages timelines, risk register, and stakeholder communication.
- Product Manager (PdM) / Product Lead: defines outcomes, prioritizes backlog, and owns success metrics.
- Developers: implement features, write tests, and participate in reviews and estimation.
- QA/Testing: validate acceptance criteria and support release verification.
- Stakeholders / Sponsor: provide inputs, approve gates, and resolve priority decisions.

## Decision points & escalation paths
- Initiation Decision Gate: move from Initiation → Planning when one-pager, success metrics, stakeholders, and team availability are confirmed (see Initiation doc).
- Release Gate: Ready-to-release requires acceptance criteria met, CI/security scans green, and release notes/rollback plan prepared (see Release doc).
- Escalation path for blockers (see Execution & Risks docs):
  - Level 1: Team triage (daily standup)
  - Level 2: PM escalates to Product Lead and dependent teams
  - Level 3: Sponsor-level escalation for business-impacting issues
  - Security incidents: follow the security incident runbook and notify Security on-call per Risks & Communication guidance

## Communication cadences & channels
- Daily / short-cycle: Daily standups for the delivery team (Execution & Tracking).
- Regular planning and alignment:
  - Weekly delivery sync and PM + PdM weekly sync (Project Management Overview & Execution).
  - Twice-weekly standups for the delivery team (or as agreed) (Overview).
  - Monthly stakeholder updates (Overview).
- Channels / artefacts:
  - Project board (GitHub Projects or equivalent) for workflow tracking (Execution & Tracking).
  - Project README and Project One-pager in the repo as single source-of-truth (Overview / Initiation).
  - Use issue/PR descriptions to capture acceptance criteria and link to relevant artifacts.

## Quality gates, reviews, and acceptance criteria
- Pull Request requirements (Execution & Tracking):
  - Keep PRs small when possible.
  - Include the issue link and clear acceptance criteria in the PR description.
  - Automated tests and linting must pass in CI before requesting review.
  - Require at least one approval before merging (or team-defined policy).
- Testing expectations:
  - Unit tests for new logic.
  - Integration tests where applicable.
  - End-to-end smoke tests for critical flows before release.
  - Security scanning in CI and manual QA / acceptance testing as needed.
- Definition of Done: documented during Planning and used to confirm an item is ready for the next stage (see Planning doc).

## How to contribute / update these docs
- Edit the appropriate file in docs/ and open a PR describing the change.
- If you are proposing a process change, link or reference the relevant issue and include rationale and acceptance criteria for the update.
- Use the repository's ISSUE_TEMPLATE for process-doc updates when appropriate.

## Files in this folder (verified)
- ./octoacme-project-management-overview.md
- ./octoacme-project-initiation.md
- ./octoacme-project-planning.md
- ./octoacme-execution-and-tracking.md
- ./octoacme-risks-and-communication.md
- ./octoacme-release-and-deployment.md
- ./octoacme-retrospective-and-continuous-improvement.md
- ./octoacme-roles-and-personas.md

## Reference
- This README and the summaries above are derived directly from the linked documents in this folder. See each file for full details and templates.
