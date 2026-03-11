# OctoAcme — Role Interaction Checklist

## Purpose
Provide a per-phase checklist of who must be consulted, informed, and responsible for key handoffs across the OctoAcme project lifecycle. Use this alongside the [Roles & Personas](octoacme-roles-and-personas.md) doc and the [Project Management Overview](octoacme-project-management-overview.md).

---

## Phase 1: Initiation

Reference: [Project Initiation Guide](octoacme-project-initiation.md)

### Checklist
- [ ] **PM** creates the project one-pager and shares with PdM and key stakeholders for review.
- [ ] **PdM** confirms problem statement, success metrics, and initial priority.
- [ ] **Business Analyst** (if engaged) reviews the problem statement and flags any requirement ambiguities.
- [ ] **UX Designer** (if engaged) is informed of the project scope and notes any early UX research needs.
- [ ] **Security Champion** is informed; flags any known security requirements or compliance concerns.
- [ ] **Support** is informed if the project addresses a known user-reported pain point.
- [ ] **PM** records go/no-go decision and shares outcome with all roles listed above.

### Key Handoffs
| From | To | Handoff Artifact |
|---|---|---|
| PM | PdM | Reviewed one-pager |
| PdM | Business Analyst | Problem statement and draft success metrics |
| PM | All roles | Go/no-go decision and project timeline |

---

## Phase 2: Planning

Reference: [Project Planning](octoacme-project-planning.md)

### Checklist
- [ ] **PdM** leads backlog refinement with input from Business Analyst and Developers.
- [ ] **Business Analyst** documents acceptance criteria for priority backlog items; reviewed by PdM and QA.
- [ ] **UX Designer** provides wireframes or interaction specs for user-facing features before sprint planning.
- [ ] **Security Champion** reviews architecture decisions for security implications; adds items to the risk register.
- [ ] **PM** incorporates design, security, and BA estimates into the project plan and milestone schedule.
- [ ] **PM** confirms resource availability for all involved roles.
- [ ] **Support** is informed of planned features so they can prepare user documentation and FAQs.

### Key Handoffs
| From | To | Handoff Artifact |
|---|---|---|
| Business Analyst | PdM / Developers | Acceptance criteria |
| UX Designer | Developers | Annotated wireframes / specs |
| Security Champion | PM | Security risks added to risk register |
| PM | All roles | Finalized sprint plan and milestones |

---

## Phase 3: Execution & Tracking

Reference: [Execution & Tracking](octoacme-execution-and-tracking.md)

### Checklist
- [ ] **Developers** implement features per acceptance criteria; raise blockers in daily standup.
- [ ] **UX Designer** is available for design Q&A and reviews implemented features mid-sprint.
- [ ] **Business Analyst** is available to clarify requirements; logs decisions in the project tracker.
- [ ] **Security Champion** reviews security-sensitive PRs and flags risks immediately.
- [ ] **PM** tracks progress, updates risk register, and escalates blockers.
- [ ] **PdM** reviews demos and confirms acceptance criteria are met before closing stories.
- [ ] **Support** is kept informed of any changes that affect user-facing behavior.

### Key Handoffs
| From | To | Handoff Artifact |
|---|---|---|
| Developers | PdM / QA | Feature demo / PR for acceptance review |
| UX Designer | Developers | Design feedback and updated specs |
| Security Champion | PM | Updated security risk status |

---

## Phase 4: Release & Deployment

Reference: [Release & Deployment Guide](octoacme-release-and-deployment.md)

### Checklist
- [ ] **PM** confirms all acceptance criteria are met and release is authorized.
- [ ] **Security Champion** provides pre-release security sign-off (CI scans passed, no open critical risks).
- [ ] **UX Designer** confirms that user-facing changes match approved designs.
- [ ] **Support** reviews release notes and updates FAQs and support documentation.
- [ ] **Business Analyst** confirms all stated requirements are covered in the release.
- [ ] **Developers** run post-deploy verifications and smoke tests.
- [ ] **PM** announces release to stakeholders and Support.

### Key Handoffs
| From | To | Handoff Artifact |
|---|---|---|
| Security Champion | PM | Security sign-off confirmation |
| PM | Support | Final release notes |
| Developers | PM | Post-deploy verification results |

---

## Phase 5: Close & Retrospective

Reference: [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)

### Checklist
- [ ] **PM** facilitates the retrospective and documents action items with owners.
- [ ] **Support** shares a summary of post-release user feedback and reported issues.
- [ ] **Security Champion** reports on any security incidents or near-misses during the project.
- [ ] **UX Designer** shares usability observations gathered post-release (if applicable).
- [ ] **Business Analyst** reviews whether delivered features met the original business requirements.
- [ ] **PdM** confirms outcome metrics and shares findings with stakeholders.
- [ ] **PM** ensures action items are added to the backlog with owners and due dates.

### Key Handoffs
| From | To | Handoff Artifact |
|---|---|---|
| Support | PM / PdM | Post-release user feedback summary |
| Security Champion | PM | Security retrospective notes |
| PM | All roles | Action items and retrospective summary |

---

## Quick Reference: Consultation Guide

When in doubt about who to involve, use this guide:

| Decision Type | Must Consult | Must Inform |
|---|---|---|
| New feature scope or priority change | PdM, Business Analyst | PM, Developers, Support |
| Architecture or technology choice | Developers, Security Champion | PM, PdM |
| Design or UX change | UX Designer, PdM | Developers, Support |
| Schedule or milestone change | PM, PdM | All roles |
| Security risk identified | Security Champion, PM | PdM, Developers |
| Production incident | PM, Developers | Support, PdM, Security Champion |
| Requirements ambiguity | Business Analyst, PdM | PM, Developers |
