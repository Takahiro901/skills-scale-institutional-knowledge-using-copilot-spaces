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

## Support / Customer Support Representative

### Role Summary
Customer Support Representatives are the frontline connection between users and the product team. They surface real-world user pain points, triage incoming issues, and ensure user-impacting bugs are escalated appropriately.

### Responsibilities
- Handle incoming user inquiries, bug reports, and feedback
- Triage and escalate production issues to the PM and engineering leads
- Maintain and update user-facing FAQs and known-issue documentation
- Participate in release readiness reviews to prepare support materials
- Contribute post-release feedback to retrospectives

### Goals
- Minimize user friction and time-to-resolution for reported issues
- Keep internal teams informed of emerging user trends and complaints
- Ensure support documentation is accurate and current after each release

### Typical Communication
- Escalation tickets and incident summaries to PM and engineering
- Weekly digest of top reported issues shared with PdM
- Release notes review and FAQ updates before each release

### Interactions with Existing Roles
- **Project Manager (PM):** Escalates production incidents; receives timeline updates for fix delivery.
- **Product Manager (PdM):** Shares user feedback and pain points that inform backlog prioritization.
- **Developers:** Provides reproduction steps and contextual details for bug fixes.
- **Shows up in:** [Release & Deployment](octoacme-release-and-deployment.md) (post-release verification), [Retrospective](octoacme-retrospective-and-continuous-improvement.md) (user-impact feedback).

---

## UX Designer

### Role Summary
UX Designers advocate for the end user throughout the product lifecycle. They translate requirements into usable, accessible experiences and validate designs through research and feedback loops.

### Responsibilities
- Conduct user research, usability tests, and competitive analysis
- Create wireframes, prototypes, and interaction specifications
- Collaborate with Developers and PdM to ensure designs are feasible and well-scoped
- Review acceptance criteria to confirm user experience requirements are captured
- Participate in sprint reviews and provide design feedback on implemented features

### Goals
- Deliver intuitive, accessible, and consistent user experiences
- Reduce rework caused by late-stage design changes
- Bridge the gap between business requirements and user needs

### Typical Communication
- Design reviews with PdM and Developers at planning and mid-sprint
- Prototypes and annotated wireframes shared in the project repo or design tool
- Usability test summaries shared with the full team after research sessions

### Interactions with Existing Roles
- **Product Manager (PdM):** Collaborates on problem framing, acceptance criteria, and user stories.
- **Developers:** Provides detailed specs and is available for design Q&A during development.
- **Project Manager (PM):** Flags design dependencies or research timelines that affect the project schedule.
- **Shows up in:** [Project Planning](octoacme-project-planning.md) (design estimation), [Execution & Tracking](octoacme-execution-and-tracking.md) (sprint review feedback).

---

## Business Analyst

### Role Summary
Business Analysts bridge business needs and technical delivery by clarifying requirements, modeling processes, and ensuring solutions address the root problem. They reduce ambiguity before work begins.

### Responsibilities
- Elicit, document, and validate business and functional requirements
- Analyze current-state processes and identify improvement opportunities
- Support the PdM in writing clear, testable acceptance criteria
- Facilitate requirement workshops with stakeholders and engineering
- Track requirement coverage and flag scope gaps during execution

### Goals
- Ensure delivered solutions solve the stated business problem
- Reduce mid-sprint scope changes caused by unclear requirements
- Create a shared understanding of "done" across all roles

### Typical Communication
- Requirements documents and process diagrams shared before sprint planning
- Clarification questions and decisions logged in the project tracker
- Acceptance criteria reviews with PdM and QA before sprint start

### Interactions with Existing Roles
- **Product Manager (PdM):** Works together on backlog refinement, acceptance criteria, and prioritization.
- **Project Manager (PM):** Surfaces scope risks and dependency gaps that affect the project plan.
- **Developers:** Provides clear requirements and is available during sprint to answer questions.
- **Shows up in:** [Project Initiation](octoacme-project-initiation.md) (one-pager refinement), [Project Planning](octoacme-project-planning.md) (backlog refinement and acceptance criteria).

---

## Security Champion

### Role Summary
Security Champions promote a security-first mindset within the delivery team. They are embedded practitioners who identify risks early, guide secure design decisions, and ensure compliance requirements are met before release.

### Responsibilities
- Review architecture and design decisions for security implications
- Identify and document security risks in the risk register
- Ensure security scanning and testing are part of the CI/CD pipeline
- Coordinate with external security teams when required (e.g., pen testing, audits)
- Review release readiness from a security perspective before each deployment
- Run or facilitate brief security awareness check-ins for the team

### Goals
- Shift security left — catch vulnerabilities in design, not in production
- Maintain a current and actionable security risk register
- Ensure releases pass security acceptance criteria

### Typical Communication
- Security risk items added to the shared risk register
- Pre-release sign-off communicated to PM and engineering leads
- Ad-hoc security advisories shared with the team as needed

### Interactions with Existing Roles
- **Project Manager (PM):** Contributes security risks to the risk register; flags release blockers.
- **Product Manager (PdM):** Advises on security implications of prioritization and feature design.
- **Developers:** Reviews PRs for security concerns; provides guidance on secure coding practices.
- **Shows up in:** [Risk Management & Communication](octoacme-risks-and-communication.md) (risk register), [Release & Deployment](octoacme-release-and-deployment.md) (pre-release security sign-off).

---

## RACI Quick Reference

The table below maps common project activities to each role using RACI notation:
**R** = Responsible (does the work), **A** = Accountable (final decision/sign-off), **C** = Consulted (provides input), **I** = Informed (kept in the loop).

| Activity | PM | PdM | Developer | Support | UX Designer | Business Analyst | Security Champion |
|---|---|---|---|---|---|---|---|
| Project initiation one-pager | R/A | C | I | I | C | C | I |
| Backlog refinement & prioritization | C | R/A | C | C | C | C | I |
| Acceptance criteria definition | C | A | C | I | C | R | C |
| Risk register management | R/A | I | C | I | I | C | R |
| Release readiness review | A | C | R | C | C | I | C |
| Post-release verification | R | I | R | C | I | I | C |
| Retrospective facilitation | R/A | C | C | C | C | C | C |

> **Note:** R and A may be shared where a role both performs and owns the activity. Adjust ownership to match your team's structure.
>
> For a per-phase checklist of who to consult and key handoffs, see [Role Interaction Checklist](octoacme-role-interaction-checklist.md).

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See [Role Interaction Checklist](octoacme-role-interaction-checklist.md) for per-phase handoff details.

