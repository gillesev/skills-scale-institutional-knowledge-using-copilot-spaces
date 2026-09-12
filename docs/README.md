# OctoAcme Project Management Documentation

Welcome to the OctoAcme project management framework. This documentation provides comprehensive guidance for running projects that deliver product features, services, and integrations with clarity, consistency, and customer focus.

## Quick Start

- **[Project Management Overview](./octoacme-project-management-overview.md)** — Start here for the big picture, core principles, and how all the pieces fit together
- **[Roles and Personas](./octoacme-roles-and-personas.md)** — Understand key team roles and responsibilities

## Phase-Based Navigation

OctoAcme projects follow a five-phase lifecycle. Navigate to the phase you're currently working on:

1. **[Initiation](./octoacme-project-initiation.md)** — Validate business need, identify stakeholders, and decide go/no-go for planning
2. **[Planning](./octoacme-project-planning.md)** — Break work into shippable increments, identify dependencies, and align timelines
3. **[Execution & Tracking](./octoacme-execution-and-tracking.md)** — Manage day-to-day delivery, quality assurance, and progress tracking
4. **[Release & Deployment](./octoacme-release-and-deployment.md)** — Standardize how we release to production and minimize risk
5. **[Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)** — Capture learnings and convert them into actionable improvements

## Cross-Cutting Concerns

- **[Risk Management & Communication](./octoacme-risks-and-communication.md)** — Applies across all phases; covers risk registers, escalation paths, and stakeholder communication

## OctoAcme Project Management Process Overview

### Principles & Approach

OctoAcme runs projects with a focus on **customer value**, **iterative delivery**, **clear ownership**, **data-informed decisions**, and **psychological safety**. Every project has a named Project Manager coordinating schedules and risks, and a Product Manager defining outcomes and measuring success. This clear role separation ensures technical execution, product strategy, and delivery coordination remain aligned.

### Lifecycle at a Glance

Projects move through five distinct phases:
- **Initiation** validates the business need and stakeholders, creating a lightweight Project One-pager with problem statement, goals, success metrics, and initial risks
- **Planning** turns the approved initiative into an actionable backlog with acceptance criteria, estimates, dependencies, and a release plan
- **Execution** focuses on day-to-day delivery using GitHub Projects, small pull requests (≤400 lines), automated CI testing, and regular standups and demos
- **Release** controls deployment to production with pre-release checklists, smoke tests, rollback plans, and post-deployment verification
- **Close & Retrospective** captures learnings through a structured review, identifies 2–3 prioritized action items, and feeds improvements back into the process

### Key Workflows & Quality Practices

During execution, teams work on a GitHub Projects board with columns: Backlog, Ready, In Progress, In Review, QA, Done. Quality is enforced through **unit tests**, **integration tests**, **end-to-end smoke tests** for critical flows, and **security scanning in CI pipelines**. Pull requests must be small, include issue links and acceptance criteria, pass automated checks, and receive at least one approval before merging. Daily standups focus on progress and blockers, while weekly delivery syncs review flagged risks.

### Risk Management & Communication

The project maintains a **Risk Register** capturing ID, description, impact, likelihood, owner, and mitigation plan. Risks are identified during planning and ongoing execution, assessed for severity, actively mitigated, and monitored at weekly syncs. Blockers escalate in levels: team triage in standup, PM escalation to Product Lead and dependent teams, and sponsor-level escalation for business-impacting issues. Stakeholder communication centers on a single source of truth (the project README or release doc) with regular status updates and clear escalation paths.

### Continuous Improvement Culture

After each sprint, release, or milestone, the team runs a retrospective to capture learnings and assign action items with clear owners and due dates. This ensures that each cycle feeds improvements back into the process, reducing single-person dependency and accelerating onboarding by making processes, decisions, and rationale searchable and versioned artifacts.

## Role-Specific Quick Links

Depending on your role, here's where to focus:

### Developers
1. Start with **[Execution & Tracking](./octoacme-execution-and-tracking.md)** to understand the daily workflow, PR conventions, and quality practices
2. Review **[Release & Deployment](./octoacme-release-and-deployment.md)** to understand how code moves to production
3. Reference **[Risk Management & Communication](./octoacme-risks-and-communication.md)** for escalation paths and incident communication

### Product Managers
1. Start with **[Project Initiation](./octoacme-project-initiation.md)** to learn how to validate and author a Project One-pager
2. Move to **[Project Planning](./octoacme-project-planning.md)** to create backlog, estimate scope, and define acceptance criteria
3. Reference **[Execution & Tracking](./octoacme-execution-and-tracking.md)** to understand how product metrics and success criteria are monitored

### Project Managers
1. Review the **[Project Management Overview](./octoacme-project-management-overview.md)** to understand the full framework
2. Follow the lifecycle sequentially: Initiation → Planning → Execution → Release → Retrospective
3. Keep **[Risk Management & Communication](./octoacme-risks-and-communication.md)** open at all times for escalation and status reporting guidance

## Key Artifacts & Templates

Across the lifecycle, OctoAcme uses these key artifacts:
- **Project Charter / One-pager** — Problem, goal, success metrics, stakeholders, timeline, risks
- **Roadmap and Release Plan** — Prioritized milestones and delivery windows
- **Sprint / Iteration Backlog** — Prioritized work with acceptance criteria and estimates
- **Risk Register** — ID, description, impact, likelihood, owner, mitigation, status
- **Release Notes** — Name, date, summary, changes, migration steps, known issues
- **Retrospective Notes** — What went well, improvements, action items with owners

## Communication Cadence

- **Daily**: Team standups (15 min) — progress, blockers, dependencies
- **Weekly**: PM + PdM sync — alignment and cross-project updates
- **Twice-weekly** (or agreed): Delivery team standups
- **End of sprint/milestone**: Demo and review with stakeholders
- **Monthly**: Stakeholder updates and roadmap briefings
- **Ad-hoc**: Escalations and incident communication

## How to Use These Docs

- **New to OctoAcme?** Start with the [Project Management Overview](./octoacme-project-management-overview.md) and [Roles and Personas](./octoacme-roles-and-personas.md)
- **Starting a new project?** Follow the Initiation and Planning guides sequentially
- **In active delivery?** Refer to Execution & Tracking and Risk Management docs
- **Preparing a release?** Use the Release & Deployment checklist and playbooks
- **After a milestone?** Run a retrospective and track action items back into your backlog

All process documents live in this folder and are maintained as living artifacts. For updates or clarifications, please refer to the [Process Doc Update issue template](../.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml).
