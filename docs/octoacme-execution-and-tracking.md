# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup — developer or QA raises the issue
- Level 2: PM escalates to Product Lead and dependent teams if unresolved after one sprint
- Level 3: Sponsor-level escalation for business-impacting issues; PM documents in risk register and notifies sponsor
- Security issues: Immediately notify Security on-call and follow the security incident runbook

See [Risk Management & Communication](octoacme-risks-and-communication.md) and [Risk Review Checklist](octoacme-risk-review-checklist.md) for the full escalation matrix.

## Quality Gates

Before moving work through each stage, confirm the following gates:

| Gate | Criteria | Who Verifies |
|---|---|---|
| Ready for development | Acceptance criteria written and reviewed | PM + PdM |
| Ready for review | CI passes (tests + lint), PR description complete, issue linked | Developer |
| Ready for QA | At least one peer approval, no unresolved review comments | Developer + Reviewer |
| Ready for release | All acceptance criteria verified, QA signed off, smoke tests passing | QA + PM |
| Release complete | Post-deploy verification passed, release notes published | PM + Engineering Lead |

See [Release & Deployment Guide](octoacme-release-and-deployment.md) for the full release readiness checklist.

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
- [ ] Quality gate criteria agreed by team

## Related Documents
- [Project Planning](octoacme-project-planning.md)
- [Risk Management & Communication](octoacme-risks-and-communication.md)
- [Risk Review Checklist](octoacme-risk-review-checklist.md)
- [Release & Deployment Guide](octoacme-release-and-deployment.md)
- [Roles and Personas](octoacme-roles-and-personas.md)
