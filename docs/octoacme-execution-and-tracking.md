# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies; facilitated by Scrum Master/Agile Coach when applicable
- Weekly delivery sync — show progress, updates, and flagged risks (include UX Designer for design reviews, DevOps Engineer for deployment updates)
- Demo/Review at the end of each sprint or milestone (include Customer Success Manager for customer impact feedback)
- Design critiques and user testing sessions (led by UX Designer, attended by PM, PdM, and key Developers)
- Metrics review (Data Analyst presents insights on success metrics and usage patterns)

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- Unit tests for new logic (written by Developers)
- Integration tests where applicable (coordinated with DevOps Engineer)
- End-to-end smoke tests for critical flows before release (automated in CI/CD pipeline)
- Security scanning in CI (managed by DevOps Engineer)
- Usability testing for new user-facing features (conducted by UX Designer)
- Manual QA for feature acceptance when needed (performed by QA team)
- Performance and reliability monitoring (tracked by DevOps Engineer)

## Reporting & Metrics
- Track velocity and burndown (monitored by Scrum Master/Agile Coach and PM)
- Monitor success metrics identified in the Project One-pager (reported by Data Analyst)
- Use dashboards for key signals (errors, latency, usage) — maintained by DevOps Engineer and Data Analyst
- Track customer satisfaction and adoption metrics (provided by Customer Success Manager)
- Monitor UX metrics like task completion rates and usability scores (tracked by UX Designer)

## Blocker Escalation
- Level 1: Team-level triage in daily standup (facilitated by Scrum Master/Agile Coach)
- Level 2: PM escalates to Product Lead and dependent teams (may involve DevOps Engineer for infrastructure issues, UX Designer for design blockers)
- Level 3: Sponsor-level escalation for business-impacting issues (include Customer Success Manager if customer-facing)
- For security incidents, follow the security incident runbook and notify Security on-call

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
