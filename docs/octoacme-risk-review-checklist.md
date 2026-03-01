# OctoAcme — Risk Review Checklist

Use this checklist during weekly syncs, planning sessions, and pre-release reviews to ensure risks are identified, assessed, and actively managed. See [Risk Management & Communication](octoacme-risks-and-communication.md) for the full risk process.

---

## Weekly Risk Review

**Date:** _______ | **Project:** _______ | **Reviewed by:** _______

### Risk Register Review

- [ ] Risk register is up to date (all items reviewed this week)
- [ ] Each open risk has a named owner
- [ ] All High-impact risks have a documented mitigation plan
- [ ] Risks that have materialized are updated to "Issue" status and tracked
- [ ] Any new risks identified this week are added with ID, description, impact, likelihood, owner, and mitigation

### Escalation Check

- [ ] Any risk rated High impact + High likelihood has been escalated to PM/Product Lead
- [ ] Sponsor-level risks (business-impacting) have been communicated to sponsors
- [ ] Security or compliance risks have been flagged to the Security team and tracked separately

### Dependency Check

- [ ] Cross-team dependencies are visible on the project board
- [ ] Blocked dependencies have been escalated and have an owner
- [ ] Upcoming dependencies are flagged at least one sprint in advance

---

## Pre-Release Risk Review

Run this checklist before every release. Also see the [Release & Deployment Guide](octoacme-release-and-deployment.md).

- [ ] All High/Medium risks reviewed and mitigated or accepted with documented rationale
- [ ] Rollback plan is documented and reviewed
- [ ] On-call / incident response rotation confirmed
- [ ] Security scan results reviewed; no unresolved critical findings
- [ ] Customer-impacting risks communicated to support and success teams

---

## Risk Escalation Path

| Level | Condition | Action | Owner |
|---|---|---|---|
| L1 | Risk identified by team member | Add to risk register; discuss in standup | Developer / QA |
| L2 | Medium or High risk unresolved > 1 sprint | Escalate to PM; update mitigation plan | PM |
| L3 | High impact + High likelihood; business-impacting | Escalate to Product Lead / Sponsor | PM + Product Lead |
| L4 | Security or compliance risk | Notify Security on-call; follow security incident runbook | PM + Security |

---

## Risk Register Template

| ID | Description | Impact | Likelihood | Owner | Mitigation | Status |
|---|---|---|---|---|---|---|
| R-001 | | High / Med / Low | High / Med / Low | | | Open / Mitigated / Closed |

---

**Related docs:**
- [Risk Management & Communication](octoacme-risks-and-communication.md)
- [Execution & Tracking](octoacme-execution-and-tracking.md)
- [Release & Deployment Guide](octoacme-release-and-deployment.md)
- [Project Planning](octoacme-project-planning.md)
