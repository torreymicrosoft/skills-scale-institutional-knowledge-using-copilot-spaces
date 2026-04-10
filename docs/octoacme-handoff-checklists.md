# OctoAcme — Handoff Checklists

## Purpose
Provide lightweight, role-specific checklists for the key handoffs in a project lifecycle. Each checklist names the owners, required artifacts, and conditions that must be met before work moves to the next stage.

---

## 1. Product → Engineering (Requirements Readiness)

**Trigger:** Engineering is about to begin implementation of a feature or initiative.

**Owner:** Product Manager (PdM) — responsible for completing; Project Manager (PM) — accountable for timing.

### Checklist

- [ ] Problem statement and business rationale documented
- [ ] User stories or feature spec written and reviewed with stakeholders
- [ ] Acceptance criteria defined for every user story
- [ ] UX designs / wireframes finalized and linked (if applicable)
- [ ] Business rules and edge cases documented (BA sign-off if BA is on the project)
- [ ] Non-functional requirements captured (performance, security, accessibility)
- [ ] Dependencies on other teams or systems identified
- [ ] Initial test plan reviewed with QA Lead
- [ ] Prioritization confirmed in backlog (item is "Ready" per Definition of Ready)

**Required artifacts:**
- User stories with acceptance criteria
- Design specifications or prototype link
- Dependency map (or note that none exist)

---

## 2. Engineering → QA (Test Readiness)

**Trigger:** Development of a feature or increment is complete and the team is requesting QA validation.

**Owner:** Developer (Responsible for preparing); QA Lead (Accountable for accepting or returning).

### Checklist

- [ ] Code merged to integration/staging branch (or agreed handoff branch)
- [ ] CI build passing (tests, lint, security scans)
- [ ] Test environment updated and accessible to QA
- [ ] Developer test notes written: what was changed, known edge cases, manual steps to exercise the feature
- [ ] All acceptance criteria from the user story reachable in the test environment
- [ ] Known bugs or deferred items documented and linked
- [ ] Feature flags or configuration changes documented
- [ ] API/schema changes communicated to QA and Technical Writer

**Required artifacts:**
- Link to passing CI build
- Test notes / handoff summary (in PR description or linked document)
- Updated test environment confirmation

**Return criteria (QA returns to Engineering):**
- Build is not deployable
- Acceptance criteria cannot be exercised (environment issue or missing feature)
- Undocumented breaking change discovered

---

## 3. Engineering / QA → Release (Go/No-Go)

**Trigger:** Release candidate is ready; team is deciding whether to proceed to production deployment.

**Owner:** Project Manager (PM) — facilitates go/no-go; QA Lead — provides quality sign-off; Product Manager (PdM) — confirms scope and business readiness.

### Checklist

**Quality gates (QA Lead confirms):**
- [ ] All planned test cases executed
- [ ] No open P0 (critical) defects
- [ ] P1 defects reviewed and accepted or deferred with PdM approval
- [ ] Regression suite passed
- [ ] Performance / load tests passed (if applicable)
- [ ] Security scan results reviewed and no new critical findings

**Product/business gates (PdM confirms):**
- [ ] All committed scope delivered or deferred with stakeholder approval
- [ ] Acceptance criteria signed off
- [ ] Release notes drafted and reviewed

**Operational gates (PM confirms):**
- [ ] Release plan and rollback plan documented
- [ ] Deployment window communicated to stakeholders and support
- [ ] Documentation updated (Technical Writer sign-off or owner confirmation)
- [ ] Support Lead briefed on new features and known issues
- [ ] Executive Sponsor / Stakeholder notified of release (if required by project)
- [ ] Monitoring and alerting confirmed ready

**Required artifacts:**
- QA test-result summary
- Release notes (draft)
- Rollback plan
- Go/no-go decision log (record who approved and any conditions)

---

## 4. Release → Support / Customer Success (Support Readiness)

**Trigger:** Release has been deployed (or is imminent); Support / Customer Success must be ready to handle customer inquiries.

**Owner:** Support Lead / Customer Success (Responsible); PM (Accountable for ensuring handoff occurs).

### Checklist

- [ ] Support team notified of release date and scope
- [ ] Release notes and user-facing documentation published or shared with support
- [ ] Known issues list shared with support (including workarounds where available)
- [ ] Internal FAQ or support runbook updated for new features
- [ ] Escalation path confirmed: who to contact in Engineering/QA for urgent post-release issues
- [ ] Customer communication drafted and reviewed (if applicable — announcements, in-app banners, emails)
- [ ] Success metrics identified so support can flag anomalies (e.g., spike in ticket volume)
- [ ] Post-release check-in scheduled (e.g., 24–48 hours after release) between PM, Support Lead, and on-call Dev

**Required artifacts:**
- Published or shared release notes
- Known issues list with workarounds
- Updated support runbook or internal FAQ
- Customer communication (if applicable)

---

## Related docs
- [Role Assignment & RACI](octoacme-role-assignment-and-raci.md)
- [Roles and Personas](octoacme-roles-and-personas.md)
- [Execution & Tracking](octoacme-execution-and-tracking.md)
- [Risks and Communication](octoacme-risks-and-communication.md)
