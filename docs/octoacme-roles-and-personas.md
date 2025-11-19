# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## QA (Quality Assurance)

### Role Summary
QA Engineers ensure that features meet acceptance criteria and quality standards before release. They design test plans, execute testing, and provide feedback on quality and usability.

### Responsibilities
- Create test plans and test cases from acceptance criteria
- Execute manual and automated tests
- Report bugs and verify fixes
- Participate in acceptance reviews and sprint planning
- Provide quality feedback during development

### Goals
- Prevent defects from reaching production
- Improve testability and automation coverage
- Reduce time to find and fix bugs

### Typical Communication
- Sprint planning and backlog refinement
- Bug reports and test results
- Acceptance sign-off for features

---

## Scrum Master

### Role Summary
Scrum Masters facilitate agile ceremonies, remove impediments, and coach the team on agile practices. They ensure the team can work effectively and continuously improve their processes.

### Responsibilities
- Facilitate sprint planning, daily standups, retrospectives, and reviews
- Remove blockers and impediments for the team
- Coach team members on agile principles and practices
- Shield the team from external distractions
- Track and communicate team velocity and capacity

### Goals
- Maximize team productivity and focus
- Foster continuous improvement and self-organization
- Ensure ceremonies are effective and time-boxed

### Typical Communication / Interaction
- **With PM:** Collaborate on sprint planning and risk escalation; PM owns project timeline while Scrum Master owns team process
- **With PdM:** Ensure backlog items are ready and acceptance criteria are clear
- **With Developers:** Facilitate daily standups, remove blockers, coach on estimation and collaboration
- **With QA:** Coordinate testing activities within sprint cadence

### Escalation Path
- Team-level blockers → Scrum Master facilitates resolution
- Cross-team dependencies → Escalate to PM for coordination
- Process or organizational impediments → Escalate to leadership

---

## UX Designer

### Role Summary
UX Designers research user needs, create wireframes and prototypes, and validate designs through usability testing. They ensure products are intuitive, accessible, and aligned with user expectations.

### Responsibilities
- Conduct user research and synthesize insights
- Create wireframes, mockups, and interactive prototypes
- Define and validate design patterns and UI components
- Perform usability testing with users or stakeholders
- Collaborate on acceptance criteria to ensure design intent is captured

### Goals
- Deliver intuitive, user-centered interfaces
- Reduce usability issues and support costs
- Ensure design consistency across the product

### Typical Communication / Interaction
- **With PdM:** Partner on user research, validate problem statements, and prioritize design work based on roadmap
- **With Developers:** Hand off designs with specifications, collaborate on feasibility and technical constraints, review implementation
- **With QA:** Define expected user flows for testing, participate in acceptance reviews
- **With PM:** Align on timeline for design deliverables and dependencies

### Common Handoffs
- Design → Development: Provide annotated mockups, design specs, and component guidelines; attend sprint planning to clarify intent
- Usability Testing → Iteration: Share findings with PdM and Developers to inform backlog prioritization and refinements

---

## Technical Lead

### Role Summary
Technical Leads provide architecture guidance, set code quality standards, and mentor developers. They ensure technical decisions align with long-term maintainability and scalability goals.

### Responsibilities
- Define architecture patterns and technical standards
- Lead design reviews and provide code review feedback
- Mentor developers on best practices and technology choices
- Collaborate with PM and PdM on technical feasibility and effort estimates
- Identify technical debt and advocate for refactoring work

### Goals
- Maintain code quality and system reliability
- Enable developers to work efficiently and independently
- Reduce technical risk and long-term maintenance costs

### Typical Communication / Interaction
- **With Developers:** Conduct code reviews, pair programming, provide architecture guidance and mentorship
- **With PM:** Provide effort estimates, flag technical risks, communicate capacity constraints
- **With PdM:** Consult on technical feasibility, advise on trade-offs between features and technical debt
- **With QA:** Collaborate on test strategy and automation approach

### Common Handoffs
- Design Review → Implementation: Approve architecture approach, provide implementation guidance
- Code Review → Merge: Ensure quality standards are met before code is deployed

---

## Support Engineer (SRE/Support)

### Role Summary
Support Engineers (or Site Reliability Engineers in SRE-focused teams) monitor production systems, triage incidents, and handle post-release issues. They provide a feedback loop from production back to the product and engineering teams.

### Responsibilities
- Monitor production systems for errors, performance issues, and anomalies
- Triage and respond to incidents and customer-reported issues
- Document known issues and workarounds
- Coordinate incident response and post-mortems
- Provide feedback to PdM and Developers on recurring issues and improvement opportunities

### Goals
- Minimize downtime and customer impact
- Improve system reliability and observability
- Reduce mean time to detect and resolve (MTTD/MTTR)

### Typical Communication / Interaction
- **With PM:** Coordinate release communications, escalate high-severity incidents
- **With PdM:** Provide feedback on user-reported issues, help prioritize fixes and improvements
- **With Developers:** Collaborate on debugging production issues, share logs and metrics, participate in post-mortems
- **With QA:** Share production issues to improve test coverage

### Role in Releases
- Pre-release: Review release notes, ensure monitoring and rollback plans are in place
- Post-release: Monitor for issues, triage new bugs, coordinate hotfixes if needed

### Common Handoffs
- Incident → Post-mortem: Document timeline, root cause, and action items; share with PM, PdM, and Developers
- Production Issue → Backlog: Log bugs or feature requests based on customer feedback and triage with PdM

---

## Common Handoffs and Collaboration Points

### Design → Development
- **Trigger:** Feature prioritized for development
- **Handoff:** UX Designer provides mockups, specs, and design guidelines to Developers
- **Collaboration:** Joint review during sprint planning; Developers flag technical constraints; iterative feedback during implementation

### Incident → Post-mortem
- **Trigger:** Production incident resolved
- **Handoff:** Support Engineer documents incident timeline, impact, and initial findings; shares with PM and Technical Lead
- **Collaboration:** Team conducts post-mortem meeting to identify root cause and action items; PM tracks follow-up work

### Code Review → Deployment
- **Trigger:** Developer completes feature implementation
- **Handoff:** Developer submits PR; Technical Lead and peers review; QA validates acceptance criteria
- **Collaboration:** Iterative feedback and approval process; merge when quality standards are met

### Release → Monitoring
- **Trigger:** New release deployed to production
- **Handoff:** PM communicates release to stakeholders; Support Engineer monitors for issues
- **Collaboration:** Support Engineer reports anomalies; PM coordinates with PdM and Developers for triage and hotfix decisions

---

## Responsibilities Matrix (RACI-lite)

This table shows how personas typically engage with key project artifacts. **R** = Responsible (does the work), **A** = Accountable (final approver), **C** = Consulted (provides input), **I** = Informed (kept in the loop).

| Artifact / Activity | PM | PdM | Developer | QA | Scrum Master | UX Designer | Technical Lead | Support Engineer |
|---------------------|----|----|-----------|----|--------------|--------------|--------------------|------------------|
| **Backlog Prioritization** | C | A | C | C | C | C | C | I |
| **Sprint Planning** | C | C | R | C | A | C | C | I |
| **Feature Implementation** | I | C | R | C | I | C | A | I |
| **Code Review** | I | I | R | I | I | I | A | I |
| **Release Planning** | A | C | C | C | C | I | C | C |
| **Release Deployment** | A | I | R | C | I | I | C | R |
| **Incident Response** | C | I | C | I | I | I | C | A |
| **Post-mortem** | C | C | C | C | A | I | C | R |
| **Retrospective** | C | C | R | R | A | C | C | C |
| **Risk Register** | A | C | C | C | C | I | C | I |

**Notes:**
- Roles may vary by team size and structure. Smaller teams may combine roles.
- For key decisions, ensure the Accountable person is clearly identified.
- Use this matrix as a starting point and adapt to your team's needs.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

