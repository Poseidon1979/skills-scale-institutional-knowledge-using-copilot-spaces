# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
  - **Facilitated by:** Scrum Master (or PM if no Scrum Master)
  - **Expected etiquette:** Time-boxed, three questions format, flag blockers clearly
- Weekly delivery sync — show progress, updates, and flagged risks
  - **Coordinated by:** PM, with PdM and Technical Lead participating
- Demo/Review at the end of each sprint or milestone
  - **Coordinated by:** PM; PdM and stakeholders attend

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - **PR size policy:** Keep PRs small (<= 400 lines when possible) for faster review and lower risk
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)
  - **For detailed PR guidance, see:** [PR Checklist](octoacme-checklists-and-templates.md#pr-pull-request-checklist)

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

### Ownership & Escalation Path
- **Level 1 (Team):** Team-level triage in daily standup
  - **Owner:** Scrum Master facilitates discussion; Developers propose solutions
- **Level 2 (PM/Technical Lead):** PM escalates to Product Lead and dependent teams; Technical Lead provides technical guidance
  - **Owner:** PM for cross-team coordination; Technical Lead for technical decisions
- **Level 3 (Sponsor):** Sponsor-level escalation for business-impacting issues
  - **Owner:** PM escalates to project sponsor or leadership
- **Production issues:** Support Engineer owns initial triage, coordinates with PM and Technical Lead for prioritization and resolution
  - **Owner:** Support Engineer (triage) → PM (prioritization) → Technical Lead (technical guidance)

### Blocker Tagging
- Clearly tag blockers in daily standup and project board (e.g., "🚫 Blocked" label)
- Identify expected owner for resolution and escalation path
- Track blocker age and escalate if unresolved after agreed threshold (e.g., 2 days)

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
- [ ] Daily standup facilitator assigned (Scrum Master or PM)
- [ ] Support Engineer identified for production triage
- [ ] Blocker escalation path communicated to team

**For detailed checklists, see:** [Checklists & Templates](octoacme-checklists-and-templates.md)
