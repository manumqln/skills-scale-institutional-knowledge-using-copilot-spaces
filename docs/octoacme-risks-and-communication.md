# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner
- Mitigation plan
- Status

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status

## Communication Templates
Weekly Status Template:
- Progress this week:
- Next steps:
- Risks & blockers:
- Ask / decisions needed:

Incident Communication
- Triage summary
- Actions being taken
- Expected timeline
- Post-incident blameless retrospective scheduled

## Escalation Paths

| Level | Condition | Action | Owner |
|---|---|---|---|
| L1 | Risk identified by any team member | Add to risk register; discuss in next standup | Developer / QA |
| L2 | Medium or High risk unresolved after one sprint | Escalate to PM; update mitigation plan | PM |
| L3 | High impact + High likelihood; business-critical | Escalate to Product Lead and Sponsor; document decision log | PM + Product Lead |
| L4 | Security or compliance risk | Immediately notify Security on-call; follow the security incident runbook | PM + Security |

For structured risk reviews, use the [Risk Review Checklist](octoacme-risk-review-checklist.md).

## Related Documents
- [Risk Review Checklist](octoacme-risk-review-checklist.md)
- [Project Planning](octoacme-project-planning.md)
- [Execution & Tracking](octoacme-execution-and-tracking.md)
- [Release & Deployment Guide](octoacme-release-and-deployment.md)
