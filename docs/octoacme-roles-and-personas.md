# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

---

## Additional Personas (proposed)

The following personas are proposed additions to expand clarity and accountability across cross-functional delivery. For each persona we describe responsibilities, how they interact with existing roles, decision authority, and suggested success criteria.

---

## Technical Program Manager (TPM)

### Role Summary
The Technical Program Manager coordinates cross-team technical dependencies for larger initiatives, maintains program-level schedules, and drives risk mitigation where multiple teams are involved.

### Responsibilities
- Maintain program-level plans and milestone timelines for multi-team efforts
- Identify, track, and remove cross-team technical dependencies and blockers
- Facilitate technical alignment and architecture trade-off discussions
- Drive risk identification and mitigation across engineering teams
- Coordinate release readiness for complex initiatives

### Interactions with Existing Roles
- Works closely with Project Managers on scheduling, risks, and stakeholder communications
- Partners with Product Managers to align technical sequencing with product priorities
- Engages Engineering Leads and Developers to surface technical constraints and coordinate implementation
- Aligns with DevOps/SRE and Release Manager for deployment sequencing and rollout plans

### Decision Authority
- Can make tactical scheduling and dependency trade-off decisions within agreed program constraints
- Escalates scope or priority conflicts to Product or Project leadership when cross-team commitments conflict

### Suggested Success Criteria
- Reduction in cross-team blockers reported at weekly program syncs
- On-time delivery of program milestones
- Clear, updated dependency register with mitigations for high-risk items

---

## UX Researcher / Designer

### Role Summary
UX Researchers and Designers own user research, usability criteria, and design handoffs; they ensure user-centered outcomes and smooth collaboration between product and engineering.

### Responsibilities
- Plan and conduct user research and usability testing
- Produce wireframes, prototypes, and design specifications
- Define usability acceptance criteria and accessibility requirements
- Provide timely design handoffs and support during implementation
- Advocate for user needs in prioritization and trade-offs

### Interactions with Existing Roles
- Partners with Product Managers to translate user insights into product requirements and success metrics
- Works with Developers and QA to clarify UI/UX details and acceptance criteria
- Collaborates with Data Analysts to measure usability impact post-release

### Decision Authority
- Owns design direction and approves UI/UX deliverables for implementation
- Can approve minor design changes during implementation; major scope/design changes should involve the Product Manager

### Suggested Success Criteria
- Design artifacts delivered on schedule for sprint planning
- Positive usability test outcomes (e.g., task success rates)
- Lowered UI-related bug rate during QA and post-release

---

## Release Manager

### Role Summary
The Release Manager owns release coordination, deployment windows, rollback plans, and post-release verification to ensure deployments are predictable and low-risk.

### Responsibilities
- Schedule and coordinate release windows across teams
- Ensure deployment checklists, rollback plans, and runbooks are in place
- Orchestrate pre-release smoke tests and post-release verification
- Communicate release status to stakeholders and support teams
- Capture release retrospectives and improvement actions

### Interactions with Existing Roles
- Coordinates with Project Managers and Product Managers on release timing and stakeholder communication
- Works with DevOps/SRE and Developers to validate CI/CD, runbooks, and rollback strategies
- Partners with QA to verify test coverage for release-critical flows
- Notifies Support and Stakeholders about release plans and potential impacts

### Decision Authority
- Can approve go/no-go decisions for scheduled releases based on checklist and risk criteria
- Escalates to Project or Product leadership if release risks are unresolved

### Suggested Success Criteria
- Releases executed without critical post-release incidents
- Rollback procedures tested and effective when used
- Clear release communications sent on schedule

---

## DevOps / SRE Engineer

### Role Summary
DevOps and SRE Engineers maintain CI/CD pipelines, observability, and incident readiness. They ensure the platform is reliable, performant, and secure for deployments.

### Responsibilities
- Maintain and improve CI/CD pipelines and deployment automation
- Implement and maintain observability, monitoring, and alerting
- Define and maintain runbooks and incident playbooks
- Support performance, scalability testing, and production troubleshooting
- Collaborate on infrastructure-as-code and environment provisioning

### Interactions with Existing Roles
- Works closely with Developers to enable safe, repeatable deployments
- Partners with Release Manager to validate deployment plans and rollback strategies
- Coordinates with Project Managers and TPMs to understand release timelines and environment needs
- Engages Security Engineers to implement platform hardening and scans

### Decision Authority
- Can enforce platform-level constraints (e.g., deployment windows, rate limits) to protect stability
- Can pause or revert deployments when platform health indicates severe risk

### Suggested Success Criteria
- High availability and low mean time to recovery (MTTR) for incidents
- Automated CI/CD success rates meeting target thresholds
- Monitoring coverage aligned to critical business and technical metrics

---

## Data Analyst / Insights Owner

### Role Summary
The Data Analyst or Insights Owner defines measurement plans, tracks success metrics, and provides data-driven insights to inform product and project decisions.

### Responsibilities
- Define event/instrumentation requirements and measurement plans tied to success metrics
- Produce dashboards and reports for product and project stakeholders
- Analyze experiments, feature impact, and usage trends
- Support prioritization with quantitative evidence and recommendations

### Interactions with Existing Roles
- Works with Product Managers to define success metrics and measurement approaches
- Partners with Developers and DevOps to ensure instrumentation and data pipelines are implemented
- Shares findings with Project Managers, PMs, and UX Researchers to influence scope and prioritization

### Decision Authority
- Owns analytic interpretations and recommended actions based on data; decisions on scope or priority remain with Product/Project leadership
- Can gate releases that lack required instrumentation for validating success criteria

### Suggested Success Criteria
- Measurement plans in place before feature launch
- Timely, accurate dashboards for key success metrics
- Data-driven decisions reflected in roadmap adjustments

---

## Security Engineer

### Role Summary
The Security Engineer evaluates security risks, performs threat assessments, and ensures security controls are integrated into development and release processes.

### Responsibilities
- Conduct security reviews and threat modelling for features
- Define and validate security requirements and acceptance criteria
- Run or coordinate security scans, vulnerability assessments, and remediation
- Collaborate on incident response and compliance obligations

### Interactions with Existing Roles
- Works with Developers to remediate vulnerabilities and implement secure coding practices
- Partners with Product Managers and Project Managers to prioritize security work and communicate risks
- Coordinates with DevOps/SRE for secure deployment and environment hardening

### Decision Authority
- Can block releases for known critical vulnerabilities until mitigations are in place
- Advises on acceptable risk levels; final trade-offs are made by Product/Project leadership in partnership with Security

### Suggested Success Criteria
- Critical vulnerabilities remediated within SLA
- Security checks included in CI and pass for release
- No high-severity incidents attributable to known gaps post-release

---

## How to add these personas into project docs and workflows
- Add a short persona summary to `docs/octoacme-roles-and-personas.md` (as above).
- For each active project, document which of these personas are assigned or consulted and list primary points of contact.
- Include handoff checklists in relevant process docs (planning, release, incident response) that reference the responsible persona.
- Capture success criteria in the project one-pager or acceptance criteria section so measurement ownership is clear.

---
