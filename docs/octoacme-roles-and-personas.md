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

### Interactions with Other Roles
- Works with QA/Testing Engineers: fix reported defects and improve testability
- Works with Release/DevOps Engineers: maintain pipelines and coordinate releases
- Works with Product Managers and Project Managers: clarify acceptance criteria and raise blockers

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

### Interactions with Other Roles
- Works with Product Leads: align on priorities and trade-offs
- Works with QA/Testing Engineers and Developers: define and confirm acceptance criteria
- Works with Stakeholders: provide briefings

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

### Interactions with Other Roles
- Works with Product Leads and Sponsors: run decision gates and escalate (Team -> PM -> Product Lead -> Sponsor)
- Works with QA/Testing Engineers and Release/DevOps Engineers: confirm release readiness and deployment windows
- Works with Stakeholders: follow the communication plan

---

## QA/Testing Engineer

### Role Summary
QA/Testing Engineers validate that features meet acceptance criteria and quality standards. They own test plans and smoke tests and provide the quality signal used for release readiness.

### Responsibilities
- Create and maintain test plans aligned to acceptance criteria
- Own smoke tests for critical flows and run them in staging before release
- Report, triage, and verify defects
- Perform manual QA when automated coverage is insufficient

### Goals
- Catch defects before they reach production
- Make acceptance criteria testable and verifiable
- Provide a clear quality signal for release decisions

### Typical Communication
- Defect reports and test results in the project board
- Test plan and smoke test summaries in release checklists
- Daily standups when releases are near

### Interactions with Other Roles
- Works with Developers: report defects with reproduction steps, verify fixes, and advise on testability
- Works with Product Managers: clarify and confirm acceptance criteria before and during testing
- Works with Project Managers: report release readiness and escalate quality risks that threaten the schedule

---

## Product Lead

### Role Summary
The Product Lead owns product direction and ensures projects align with strategy. They review the Project One-pager and are the first escalation point above the Project Manager (Level 2).

### Responsibilities
- Set and communicate product direction and priorities
- Review the Project One-pager and participate in decision gates
- Resolve Level 2 escalations raised by the PM, coordinating with dependent teams
- Escalate business-impacting issues to the Sponsor (Level 3)

### Goals
- Keep work aligned with product strategy
- Make timely, well-informed decisions at gates and escalations
- Remove cross-team blockers quickly

### Typical Communication
- Weekly alignment with Product Managers
- Decision gate reviews and escalation discussions with PMs
- Monthly stakeholder updates

### Interactions with Other Roles
- Works with Product Managers: align on priorities, roadmap trade-offs, and success metrics
- Works with Project Managers: make go/no-go decisions at decision gates and take escalations (Team -> PM -> Product Lead)

---

## Sponsor / Executive Stakeholder

### Role Summary
The Sponsor approves initiatives and funding and is the Level 3 escalation point for business-impacting issues.

### Responsibilities
- Approve initiatives, funding, and major scope changes
- Provide direction at decision gates
- Resolve Level 3 escalations for business-impacting issues
- Remove organizational obstacles

### Goals
- Ensure investment delivers business value
- Maintain visibility into progress and risk at a high level
- Make decisive calls on escalated issues

### Typical Communication
- Monthly stakeholder updates
- Decision gate briefings
- Ad-hoc escalation briefings

### Interactions with Other Roles
- Works with Project Managers: receive monthly updates, approve at decision gates, and take Level 3 escalations (Team -> PM -> Product Lead -> Sponsor)
- Works with Product Leads: confirm strategic direction and funding, and receive escalations that exceed Product Lead authority

---

## Stakeholders (Engineering, Sales, Support)

### Role Summary
Stakeholders from Engineering, Sales, and Support provide inputs and approvals and consume status updates. They are identified during initiation and kept informed throughout the project.

### Responsibilities
- Provide requirements, constraints, and feedback
- Give approvals when requested
- Review status updates and raise concerns early
- Share relevant information with their own teams

### Goals
- Be informed and able to plan around project outcomes
- Have their needs reflected in scope and priorities
- Give timely, actionable feedback

### Typical Communication
- Weekly status updates and monthly stakeholder updates
- Roadmap updates and briefings
- Ad-hoc questions via the agreed channels

### Interactions with Other Roles
- Works with Project Managers: follow the communication plan, receive status updates, and provide approvals
- Works with Product Managers: receive briefings and provide input on priorities and trade-offs

---

## Release / DevOps Engineer

### Role Summary
Release / DevOps Engineers manage CI/CD pipelines, deployments, rollback, and security scanning so that releases are repeatable and safe.

### Responsibilities
- Maintain CI/CD pipelines, including security scanning
- Execute deployments to staging and production
- Maintain and exercise rollback and mitigation plans
- Coordinate deployment windows and release checklists

### Goals
- Make releases routine, fast, and low risk
- Restore service quickly using rollback to the last known-good release
- Catch vulnerabilities in CI before release

### Typical Communication
- Release checklists and deployment notices
- Pipeline and deployment status in the project board
- Incident channel updates during rollbacks

### Interactions with Other Roles
- Works with Developers: support pipelines, release branches, and fix failing builds or scans
- Works with QA/Testing Engineers: run staging deployments so smoke tests can be executed before release
- Works with Project Managers: agree on deployment windows and report release status

---

## Security On-call / Incident Responder

### Role Summary
Security On-call / Incident Responders handle security incidents following the security incident runbook and support incident response and blameless retrospectives.

### Responsibilities
- Respond to security incidents per the runbook
- Triage severity and coordinate containment and mitigation
- Support the post-incident blameless retrospective
- Recommend follow-up actions and preventive controls

### Goals
- Contain and resolve security incidents quickly
- Learn from incidents without blame
- Reduce repeat incidents

### Typical Communication
- Incident channel updates and notifications
- Runbook-based status reports
- Retrospective notes and action items

### Interactions with Other Roles
- Works with Release/DevOps Engineers: coordinate rollback, mitigation, and pipeline changes during incidents
- Works with Developers: investigate root causes and deliver fixes
- Works with Project Managers: be notified of incidents, communicate impact, and escalate (Team -> PM -> Product Lead -> Sponsor) as needed

---

## UX / Design (optional)

### Role Summary
UX / Design ensures solutions are usable and follow a customer-first approach. This role is optional and applies when a project has user-facing changes.

### Responsibilities
- Create wireframes, prototypes, and design specs
- Conduct usability reviews and research with Product Managers
- Review implemented designs for fidelity and accessibility

### Goals
- Deliver intuitive, accessible experiences
- Validate designs with customer feedback
- Reduce rework through early design clarity

### Typical Communication
- Design reviews and spec handoffs
- Feedback on PRs and prototypes
- Usability findings shared with the team

### Interactions with Other Roles
- Works with Product Managers: shape problem definitions, user research, and acceptance criteria
- Works with Developers: hand off designs, clarify behavior, and review implementation

---

## Support / Customer Success (optional)

### Role Summary
Support / Customer Success teams receive release announcements and relay customer feedback. This role is optional and typically overlaps with Support stakeholders.

### Responsibilities
- Review release announcements and prepare customers and support materials
- Relay customer feedback, issues, and trends
- Flag customer-impacting problems after release

### Goals
- Help customers adopt changes smoothly
- Close the loop between customers and the product team
- Reduce support load through clear communication

### Typical Communication
- Release announcements
- Customer feedback summaries
- Incident or customer impact notices

### Interactions with Other Roles
- Works with Product Managers: relay customer feedback and receive release announcements and briefings
- Works with Project Managers: receive release timing and incident communications and escalate customer-impacting issues

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- Use the Interactions with Other Roles subsections to model handoffs, decision gates, and the escalation path (Team -> PM -> Product Lead -> Sponsor).
- Optional personas (UX / Design, Support / Customer Success) can be included when a scenario needs them.

