# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared

## Release Readiness Checklist

Run this checklist before triggering any release:

- [ ] All acceptance criteria met and verified by QA
- [ ] All PRs merged and feature branch deleted
- [ ] CI pipeline fully green (tests, lint, security scan)
- [ ] Release notes drafted and reviewed
- [ ] Risk review completed — see [Risk Review Checklist](octoacme-risk-review-checklist.md)
- [ ] Rollback plan documented and communicated to on-call
- [ ] Staging deployment verified with smoke tests
- [ ] Stakeholders and support team notified of release window
- [ ] On-call schedule confirmed for post-release window

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:

## Related Documents
- [Risk Review Checklist](octoacme-risk-review-checklist.md)
- [Execution & Tracking](octoacme-execution-and-tracking.md)
- [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)
- [Risk Management & Communication](octoacme-risks-and-communication.md)
