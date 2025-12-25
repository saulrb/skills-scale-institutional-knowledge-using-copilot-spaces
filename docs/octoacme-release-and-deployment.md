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
- QA Lead sign-off on test results and quality criteria
- UX Designer approval for user-facing changes
- Release notes drafted by Technical Writer
- Rollback / mitigation plan documented by Operations/DevOps
- Smoke tests prepared and validated
- Documentation updated and published

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] QA Lead validates staging environment
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Operations/DevOps monitors system metrics and alerts
- [ ] Announce release to stakeholders and support
- [ ] Technical Writer publishes updated documentation

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call (Operations/DevOps)
  - Rollback to last known-good release if necessary
  - QA Lead validates rollback in staging
  - Triage root cause and capture action items
  - Technical Writer updates any affected documentation

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
