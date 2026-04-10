# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## How to use these personas across lifecycle docs

Reference these persona definitions when:
- Assigning ownership in planning docs, risk registers, and RACI tables
- Writing acceptance criteria or Definition of Done entries that specify who validates
- Framing scenarios for Copilot Spaces context prompts
- Onboarding new team members to understand expectations and communication patterns

**Required vs. optional roles by project type**

| Role | Small / Internal Project | Cross-functional Product Initiative |
|------|--------------------------|--------------------------------------|
| Project Manager | Required | Required |
| Product Manager | Required | Required |
| Developer(s) | Required | Required |
| QA Lead / Test Engineer | Recommended | Required |
| UX Designer | Optional | Required |
| Business Analyst | Optional | Recommended |
| Technical Writer | Optional | Recommended |
| Executive Sponsor / Stakeholder | Recommended | Required |
| Support Lead / Customer Success | Optional | Recommended |

> **Note:** Even when a role is "Optional," someone on the team should be identified as the owner of those responsibilities to prevent gaps.

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

## QA Lead / Test Engineer

### Role Summary
QA Leads own the test strategy and quality bar for a project. They ensure that features meet acceptance criteria and that regressions are caught before release.

### Responsibilities
- Define and maintain the test plan and coverage strategy
- Write and execute manual and automated test cases
- Set and enforce entry/exit criteria for QA phases
- Coordinate regression, integration, and end-to-end testing
- Participate in go/no-go decisions and release readiness reviews
- Track and triage defects; communicate status to PM and team

### Goals
- Ensure product quality and customer confidence
- Reduce escaped defects in production
- Shift testing left to catch issues early in development

### Typical Communication
- Daily standups and sprint demos
- Defect triage and test-result summaries
- Go/no-go sign-off at release milestones

### Interactions with Existing Roles
- **Developers:** Collaborates on testability, code reviews, and defect resolution; receives builds and environment details.
- **Product Managers:** Reviews acceptance criteria and clarifies ambiguous requirements; escalates quality risks.
- **Project Managers:** Reports test status and defect metrics; flags schedule risk when quality gates are not met.

---

## UX Designer

### Role Summary
UX Designers define the user experience and interaction patterns to ensure that features are intuitive, accessible, and aligned with user needs.

### Responsibilities
- Conduct user research, usability testing, and persona development
- Produce wireframes, prototypes, and visual design assets
- Define and maintain design system usage and accessibility standards
- Review implemented features against design specifications
- Advocate for the end user in backlog refinement and planning discussions

### Goals
- Deliver interfaces that are usable, accessible, and delightful
- Reduce rework by aligning design and engineering early
- Ground product decisions in user evidence

### Typical Communication
- Design reviews and critique sessions
- Annotated design files and prototype links shared with developers
- User research readouts to Product Managers and stakeholders

### Interactions with Existing Roles
- **Developers:** Provides specifications, assets, and design tokens; collaborates during implementation to ensure fidelity.
- **Product Managers:** Partners on problem framing, user stories, and feature prioritization; validates designs against requirements.
- **Project Managers:** Flags design-dependency risks and timeline needs for research or design cycles.

---

## Business Analyst

### Role Summary
Business Analysts bridge the gap between business needs and technical solutions. They elicit, document, and validate requirements to ensure solutions deliver the intended value.

### Responsibilities
- Facilitate requirements workshops with stakeholders and subject matter experts
- Document use cases, process flows, and business rules
- Translate business needs into user stories and acceptance criteria
- Clarify ambiguities between business intent and technical implementation
- Support QA in test planning by mapping requirements to test cases

### Goals
- Ensure the solution solves the right business problem
- Reduce rework caused by misunderstood or missing requirements
- Create clear, traceable requirements artifacts

### Typical Communication
- Requirements review meetings and workshop facilitation
- Detailed user stories and process flow documentation
- Regular syncs with Product Managers and QA Leads

### Interactions with Existing Roles
- **Developers:** Provides detailed requirements and acceptance criteria; answers clarifying questions during implementation.
- **Product Managers:** Collaborates on backlog refinement and feature specifications; surfaces stakeholder feedback.
- **Project Managers:** Reports requirements risks, scope changes, and dependency blockers.

---

## Technical Writer / Documentation Specialist

### Role Summary
Technical Writers ensure that product features, processes, and APIs are clearly documented for internal teams and end users.

### Responsibilities
- Write, review, and maintain user guides, API references, and release notes
- Keep process documentation (including this doc) accurate and up to date
- Coordinate with developers and PMs to capture feature changes before release
- Incorporate learnings from retrospectives into updated documentation
- Establish and maintain documentation standards and templates

### Goals
- Make knowledge discoverable and maintainable
- Reduce support burden through clear end-user documentation
- Ensure documentation is released alongside features

### Typical Communication
- Feature review meetings and documentation planning sessions
- Draft reviews with developers and PMs
- Release-gate checklists to confirm docs are complete

### Interactions with Existing Roles
- **Developers:** Gathers technical details, reviews drafts for accuracy, and coordinates on API documentation.
- **Product Managers:** Aligns on feature scope and messaging; ensures docs reflect the intended user experience.
- **Project Managers:** Flags documentation as a release dependency; highlights risks when docs lag behind delivery.

---

## Executive Sponsor / Stakeholder

### Role Summary
Executive Sponsors provide strategic direction, organizational resources, and decision-making authority for a project. They hold ultimate accountability for project outcomes and business alignment.

### Responsibilities
- Approve project charters, scope changes, and significant trade-offs
- Provide resources and remove organizational blockers
- Receive regular project status updates and act on escalated risks
- Represent the project at leadership level and align it with business strategy
- Participate in go/no-go decisions for major milestones and releases

### Goals
- Ensure the project delivers measurable business value
- Maintain organizational alignment and executive visibility
- Enable the team by removing impediments that are beyond the PM's authority

### Typical Communication
- Monthly or milestone-based status reports from PM
- Escalation communications for high-impact risks or blockers
- Approval requests for scope or resource changes

### Interactions with Existing Roles
- **Project Managers:** Receives status updates, risk escalations, and approval requests; empowers PM to act on their behalf day-to-day.
- **Product Managers:** Aligns on strategic priorities and validates business case; approves major roadmap pivots.
- **Developers:** Minimal direct interaction; engaged for demos or escalations requiring technical context.

---

## Support Lead / Customer Success

### Role Summary
Support Leads and Customer Success managers represent the voice of the customer within the delivery team. They surface real-world usage patterns, known issues, and feedback that inform priorities and readiness decisions.

### Responsibilities
- Surface customer-reported bugs, pain points, and feature requests
- Assess and communicate support readiness before releases
- Coordinate with developers and QA to reproduce and resolve customer-impacting issues
- Contribute to support documentation and FAQ updates
- Participate in release readiness reviews and go/no-go meetings

### Goals
- Minimize customer disruption from new releases
- Ensure the support team has the knowledge and tools to handle new features
- Close the feedback loop between customers and the delivery team

### Typical Communication
- Issue triage and escalation channels (e.g., support tickets, Slack channels)
- Pre-release readiness reviews and release notes reviews
- Post-release incident updates and support-impact assessments

### Interactions with Existing Roles
- **Developers:** Reports reproducible customer issues; collaborates on root cause and resolution timelines.
- **Product Managers:** Provides customer feedback and usage data to inform prioritization; validates that planned features address real needs.
- **Project Managers:** Flags support-readiness risks before release; requests coordination on customer communication for impactful changes.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See [Role Assignment & RACI](octoacme-role-assignment-and-raci.md) for a template to assign these roles on a project.
- See [Handoff Checklists](octoacme-handoff-checklists.md) for structured handoff criteria between roles.

