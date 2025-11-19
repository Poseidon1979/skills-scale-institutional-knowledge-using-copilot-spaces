# OctoAcme — Checklists & Templates

## Purpose
Provide actionable checklists to ensure quality, consistency, and clear ownership across key delivery activities. These checklists address common gaps in planning, execution, and release processes.

---

## PR (Pull Request) Checklist

Use this checklist before submitting a pull request to ensure quality and reviewability.

### Before Opening PR
- [ ] **Small PR size**: Keep changes under 400 lines when possible; split large changes into smaller, logical PRs
- [ ] **Tests included**: Add or update unit tests, integration tests, or e2e tests as appropriate for the change
- [ ] **Tests pass locally**: Run full test suite locally before pushing
- [ ] **Linting passes**: Ensure code passes all linting and formatting checks
- [ ] **Self-review**: Review your own diff for debug code, console logs, commented code, or unintended changes

### PR Description Requirements
- [ ] **Title**: Clear, concise summary of the change
- [ ] **Link to issue**: Include "Closes #[issue_number]" or "Relates to #[issue_number]"
- [ ] **Description**: Explain what changed and why; include context for reviewers
- [ ] **Acceptance criteria**: Reference or paste relevant acceptance criteria from the issue
- [ ] **Testing notes**: Describe how to test the change (manual steps, automated test coverage)
- [ ] **Screenshots/videos**: Include for any UI or visual changes

### Review Process
- [ ] **Assign reviewers**: Request review from at least one peer (or as per team policy)
- [ ] **Technical Lead review**: For architecture or significant changes, request Technical Lead review
- [ ] **Address feedback**: Respond to all review comments; push updates as needed
- [ ] **CI checks pass**: Ensure all automated tests and checks are green before merging

**Typically responsible:** Developer (author), with Technical Lead for architecture reviews

---

## Release Checklist

Use this checklist to coordinate smooth, low-risk releases.

### Pre-Release
- [ ] **Release notes drafted**: Summarize features, bug fixes, breaking changes, and known issues
- [ ] **Acceptance criteria verified**: Confirm all features meet acceptance criteria (QA sign-off)
- [ ] **Smoke tests pass**: Run end-to-end smoke tests on staging or pre-prod environment
- [ ] **Rollback plan ready**: Document rollback steps and ensure team knows how to execute
- [ ] **Monitoring configured**: Verify alerts, dashboards, and logs are in place for new features
- [ ] **Stakeholder communication**: Notify stakeholders of release timing and expected impact
- [ ] **Database migrations tested**: If applicable, test migrations in staging and have rollback scripts ready

### During Release
- [ ] **Deploy to production**: Execute deployment according to release plan
- [ ] **Monitor initial metrics**: Watch error rates, latency, and key business metrics
- [ ] **Verify critical flows**: Manually test critical user journeys immediately after deploy
- [ ] **Team on call**: Ensure Support Engineer or on-call engineer is available for issues

### Post-Release
- [ ] **Validate metrics**: Confirm success metrics from Project One-pager are trending as expected
- [ ] **Verify no regressions**: Check for unexpected errors or user-reported issues
- [ ] **Announce release**: Share release notes with stakeholders and users (email, Slack, changelog)
- [ ] **Update documentation**: Reflect changes in user guides, API docs, or internal wikis
- [ ] **Triage any issues**: Support Engineer logs and triages post-release bugs with PM/PdM
- [ ] **Retrospective scheduled**: Ensure team retrospective is scheduled to capture learnings

**Typically responsible:** PM (coordination), Developer (deployment), QA (validation), Support Engineer (monitoring), PdM (stakeholder communication)

---

## Planning Checklist

Use this checklist during project planning to ensure alignment and readiness for execution.

### Kickoff Items
- [ ] **Kickoff meeting held**: Include PM, PdM, Technical Lead, UX Designer (if applicable), Developers, QA, Scrum Master
- [ ] **Project One-pager reviewed**: Confirm problem statement, goals, success metrics, and timeline
- [ ] **Team composition confirmed**: Identify all roles (see [octoacme-roles-and-personas.md](octoacme-roles-and-personas.md))
- [ ] **Technical Lead assigned**: Ensure Technical Lead is identified and engaged for architecture guidance
- [ ] **UX touchpoints identified**: If applicable, confirm UX Designer involvement and design milestones
- [ ] **Stakeholders aligned**: Confirm stakeholders understand scope, timeline, and expectations

### Backlog & Scope
- [ ] **Backlog created**: Break work into prioritized, shippable increments with acceptance criteria
- [ ] **Estimates provided**: Use story points, t-shirt sizing, or time estimates (as per team practice)
- [ ] **Dependencies identified**: Document cross-team or external dependencies in project board or risk register
- [ ] **Risk register populated**: Capture risks with impact, probability, and mitigation plans; assign owner to risk register
- [ ] **Definition of Done agreed**: Document DoD for user stories and features

### QA & Testing
- [ ] **QA plan drafted**: Outline testing strategy (unit, integration, e2e, manual QA)
- [ ] **Test environments ready**: Ensure staging, pre-prod, or test environments are available
- [ ] **QA involved in planning**: QA reviews acceptance criteria and test scenarios during planning

### Communication & Cadence
- [ ] **Sprint/iteration length agreed**: Confirm sprint length and planning cadence (e.g., 2-week sprints)
- [ ] **Daily standup scheduled**: Agree on time and format; assign facilitator (Scrum Master or PM)
- [ ] **Demo schedule set**: Schedule regular demos or sprint reviews with stakeholders
- [ ] **Retrospective schedule set**: Plan retrospective at the end of each sprint or milestone

**Typically responsible:** PM (coordination), PdM (backlog prioritization), Technical Lead (architecture), Scrum Master (ceremonies), QA (test planning)

---

## Execution Checklist

Use this checklist to maintain momentum and quality during active development.

### Daily Standup Etiquette
- [ ] **Time-boxed to 15 minutes**: Keep standup focused and brief
- [ ] **Three questions format**: What did you do? What will you do? Any blockers?
- [ ] **Blocker tagging**: Clearly flag blockers and identify who can help unblock
- [ ] **Parking lot for details**: Move detailed discussions offline to respect everyone's time
- [ ] **Facilitator role**: Scrum Master or PM facilitates, keeps team on track

### Blocker Escalation & Triage
- [ ] **Level 1 (Team)**: Team discusses and resolves blockers in daily standup or ad-hoc
- [ ] **Level 2 (PM/Technical Lead)**: PM escalates to dependent teams or leadership; Technical Lead provides technical guidance
- [ ] **Level 3 (Sponsor)**: PM escalates business-impacting issues to project sponsor or leadership
- [ ] **Production issues**: Support Engineer owns triage and coordinates with PM and Technical Lead for prioritization

### Ownership & Accountability
- [ ] **Daily standups facilitated by**: Scrum Master (or PM if no Scrum Master)
- [ ] **Blockers escalated by**: Developer (identifies) → Scrum Master/PM (escalates)
- [ ] **Production triage owned by**: Support Engineer (initial triage) → PM (prioritization) → Technical Lead (technical decision)
- [ ] **PR reviews**: Peers and Technical Lead (for architecture or complex changes)
- [ ] **Sprint demos**: PM coordinates; PdM and stakeholders attend

### PR & Code Quality
- [ ] **PR checklist followed**: See [PR Checklist](#pr-pull-request-checklist) above
- [ ] **Small PRs encouraged**: Keep PRs under 400 lines when possible for faster review cycles
- [ ] **CI/CD pipeline healthy**: Monitor and fix any CI failures promptly
- [ ] **Code review SLA**: Team agrees on review turnaround time (e.g., 24 hours)

### Progress Tracking
- [ ] **Project board updated**: Move cards through workflow states (Backlog, In Progress, In Review, QA, Done)
- [ ] **Risk register reviewed weekly**: PM reviews and updates risks; escalates new risks to stakeholders
- [ ] **Velocity tracked**: Scrum Master or PM tracks team velocity for sprint planning
- [ ] **Success metrics monitored**: PdM monitors metrics from Project One-pager; reports trends

**Typically responsible:** Scrum Master (facilitation), PM (coordination & escalation), Developers (execution), QA (validation), Support Engineer (production triage), Technical Lead (technical guidance)

---

## How to Use These Checklists

- **Customize to your team**: Adapt checklists based on team size, maturity, and project complexity
- **Reference in planning**: Include checklist links in sprint planning and kickoff materials
- **Automate where possible**: Use PR templates, CI checks, and automation to enforce checklist items
- **Review in retrospectives**: Discuss which checklist items are helping and which need adjustment
- **Link to other docs**: See [octoacme-roles-and-personas.md](octoacme-roles-and-personas.md) for role definitions and [octoacme-execution-and-tracking.md](octoacme-execution-and-tracking.md) for execution workflows

