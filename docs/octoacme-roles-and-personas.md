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

## Quality Assurance (QA) / Testing

### Role Summary
QA validates that work meets acceptance criteria and quality standards through test planning and execution.

### Responsibilities
- Create and run test plans and test cases
- Validate acceptance criteria and regression coverage
- Report and track defects
- Support release verification and smoke tests

### Typical Communication
- Test results in PRs and release notes
- Collaboration with Developers on testability and coverage
- Coordination with PM for release readiness

---

## Additional Personas (Proposed additions)

Below are proposed personas to add to the Roles & Personas document. Each entry lists responsibilities and how they typically interact with the existing roles.

### Technical Lead
- Responsibilities:
  - Own technical direction and architecture for the project.
  - Make or coordinate major design decisions and trade-offs.
  - Identify and mitigate technical risks and dependencies.
  - Mentor engineers and review larger technical designs and PRs.
- Interactions:
  - Works closely with Product Manager (PdM) and Project Manager (PM) on technical feasibility and trade-offs.
  - Collaborates with Developers on design, implementation approach, and code reviews.
  - Partners with QA for testability concerns and to ensure non-functional requirements are testable.
  - Engages with Security/Compliance Owner for threat modeling and secure design.

When to involve:
- At kickoff for architecture decisions, before major design choices, and during complex PR reviews.

---

### Release / Build Engineer
- Responsibilities:
  - Own release pipelines, packaging, and build stability.
  - Define and maintain deployment steps, rollback procedures, and release verification checks.
  - Coordinate release schedules and ensure releases follow the deployment checklist.
- Interactions:
  - Works with DevOps/SRE on pipeline implementation and platform constraints.
  - Coordinates with PM for release windows and communication.
  - Works with QA for pre-release smoke and verification tests.
  - Communicates with Customer Success/Support before release for support readiness.

When to involve:
- During release planning, when changing CI/CD pipelines, and during production rollouts.

---

### DevOps / Platform Engineer (SRE)
- Responsibilities:
  - Ensure production readiness, capacity planning, and runbook creation.
  - Implement and maintain observability (logs, metrics, alerts).
  - Support incident response and post-incident analysis.
  - Help design for operability and resilience.
- Interactions:
  - Collaborates with Developers to instrument code and improve observability.
  - Works with Release Engineer on deployment automation and safety.
  - Supports PM/PdM on operational constraints and SLO/SLA implications.
  - Coordinates with Security/Compliance Owner on secure operations.

When to involve:
- During architecture and design for operability, pre-release checks, and incident triage.

---

### Security / Compliance Owner
- Responsibilities:
  - Identify security requirements, run threat models, and define compliance obligations.
  - Provide gating checks for sensitive changes and review security-related PRs.
  - Maintain security runbooks and ensure appropriate approvals are obtained.
- Interactions:
  - Engages early with Technical Lead and Developers for secure design.
  - Works with PM to assess and accept security/risk trade-offs.
  - Coordinates with Legal/Contracts Liaison for regulatory or contractual compliance.
  - Partners with QA for security testing where applicable.

When to involve:
- During planning for sensitive data handling, before major releases that affect compliance boundaries, and during incident response.

---

### UX Researcher / Designer
- Responsibilities:
  - Conduct user research, prototypes, and usability testing.
  - Provide design artifacts, accessibility guidance, and UI acceptance criteria.
  - Validate UX changes with users and translate findings into product decisions.
- Interactions:
  - Partners with PdM to define user needs and acceptance criteria.
  - Works with Developers to clarify designs and feasibility.
  - Collaborates with QA on UI/UX acceptance tests and accessibility checks.
  - Informs PM of timelines for design work and handoffs.

When to involve:
- During discovery, design reviews, and before UI-focused development sprints.

---

### Data Analyst / Reporting Owner
- Responsibilities:
  - Define success metrics and event tracking; design dashboards and reports.
  - Validate data collection and ensure instrumentation meets analysis needs.
  - Analyze launch performance and provide insights for iteration.
- Interactions:
  - Works with PdM to define measurable success criteria.
  - Collaborates with Developers to implement tracking and events.
  - Shares results with Stakeholders and PM to inform decisions.

When to involve:
- During planning for metrics, before release to confirm tracking, and post-release to measure impact.

---

### Customer Success / Support Liaison
- Responsibilities:
  - Gather customer feedback and surface real-world issues and requests.
  - Prepare support documentation and runbooks for new features.
  - Coordinate customer communications and readiness with product launches.
- Interactions:
  - Informs PdM on customer pain points and feature reception.
  - Works with PM for rollout communications and escalation paths.
  - Provides QA with real-world scenarios and test cases.

When to involve:
- During planning for customer-impacting changes, pre-release communications, and post-release support.

---

### Legal / Contracts Liaison
- Responsibilities:
  - Review contractual obligations, terms of service, and data handling requirements.
  - Ensure product changes comply with regulatory and contractual constraints.
  - Provide guidance on acceptable risk and mandatory controls.
- Interactions:
  - Coordinates with PM and PdM on launch constraints and gating requirements.
  - Works with Security/Compliance Owner for data protection and regulatory controls.
  - Advises on legal language in release notes or customer communications when needed.

When to involve:
- When features touch legal or contractual terms, data privacy, or when new vendor contracts are required.

---

## How to use these persona entries
- For each new project, identify which personas are required and assign owners or points-of-contact.
- Add recommended handoff points for each persona (e.g., design review complete → UX hands off to Devs; release plan approved → Release Engineer coordinates the pipeline).
- Keep responsibilities short and actionable; include links to runbooks for operational roles (SRE, Release Engineer, Security) when available.
- Ensure the Risk Register captures any missing persona involvement that could cause delivery or compliance risk.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
