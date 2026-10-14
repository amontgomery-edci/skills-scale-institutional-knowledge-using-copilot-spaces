# OctoAcme Project Management Docs

This folder describes how OctoAcme manages projects. Below is a brief overview; see the linked documents for details.

## Overview

**Lifecycle.** Projects move through five stages:

- **Initiation:** a one-pager, identified stakeholders, and a go/no-go decision gate.
- **Planning:** a prioritized backlog with estimates, a Definition of Done, a release plan, and a risk register.
- **Execution:** daily standups, a weekly delivery sync, and a project board. Pull requests are small (about 400 lines or fewer), pass CI, and need one approval.
- **Release:** patch, minor, or major releases, with a checklist, staging smoke tests, and a rollback plan.
- **Close & Retrospective:** capture learnings and action items.

**Roles and personas.** The Project Manager coordinates schedules, risks, dependencies, and communication. The Product Manager / Product Lead defines problems and success metrics and prioritizes the backlog. Developers build, test, and document features. QA validates quality and acceptance criteria. Stakeholders provide input and approvals.

**Communication.** Teams use a weekly status template, a weekly PM and PdM sync, and monthly stakeholder updates. Status lives in a single source of truth. Blockers escalate Team -> PM -> Product Lead -> Sponsor.

**Quality assurance.** Practices include unit, integration, and end-to-end smoke tests, security scanning in CI, and manual QA when needed. Teams track metrics such as velocity, burndown, and dashboards.

**Risk management.** Risks are tracked in a risk register that is reviewed weekly.

## Documents

- [Project Management Overview](octoacme-project-management-overview.md)
- [Project Initiation](octoacme-project-initiation.md)
- [Project Planning](octoacme-project-planning.md)
- [Execution and Tracking](octoacme-execution-and-tracking.md)
- [Risks and Communication](octoacme-risks-and-communication.md)
- [Release and Deployment](octoacme-release-and-deployment.md)
- [Retrospective and Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)
- [Roles and Personas](octoacme-roles-and-personas.md)
