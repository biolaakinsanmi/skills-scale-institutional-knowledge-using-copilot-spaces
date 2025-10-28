# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans (verified by DevOps Engineer)
- Release notes drafted (collaborated by PM, PdM, and Customer Success Manager)
- Rollback / mitigation plan documented (prepared by DevOps Engineer)
- Smoke tests prepared and validated (coordinated by QA and DevOps Engineer)
- UX validation completed for customer-facing changes (signed off by UX Designer)
- Customer communication plan ready (prepared by Customer Success Manager)
- Monitoring and alerting configured (set up by DevOps Engineer)
- Success metrics and dashboards ready (configured by Data Analyst)

## Deployment Checklist
- [ ] Deployment window scheduled (if needed) — coordinated by PM and DevOps Engineer
- [ ] Backup or snapshot (if applicable) — performed by DevOps Engineer
- [ ] Deploy to staging and run smoke tests — executed by DevOps Engineer with QA validation
- [ ] Deploy to production (automated pipeline preferred) — managed by DevOps Engineer
- [ ] Run post-deploy verifications — validated by DevOps Engineer and QA
- [ ] Monitor initial metrics and user behavior — tracked by Data Analyst and DevOps Engineer
- [ ] Announce release to stakeholders and support — led by PM with input from Customer Success Manager
- [ ] Update documentation and help resources — coordinated by Customer Success Manager

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call (led by DevOps Engineer)
  - Rollback to last known-good release if necessary (executed by DevOps Engineer)
  - Triage root cause and capture action items (facilitated by Scrum Master/Agile Coach if applicable)
  - Communicate status to customers if customer-facing (coordinated by Customer Success Manager)
  - Document incident and lessons learned in blameless post-mortem

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
