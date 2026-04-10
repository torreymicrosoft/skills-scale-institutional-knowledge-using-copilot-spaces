# OctoAcme — Role Assignment & RACI

## Purpose
Provide a lightweight template for assigning ownership and clarifying accountability across a project using a RACI matrix.

---

## What is a RACI?

| Letter | Meaning | Who |
|--------|---------|-----|
| **R** | Responsible | Does the work |
| **A** | Accountable | Owns the outcome; approves the result |
| **C** | Consulted | Provides input before decisions/actions |
| **I** | Informed | Kept updated on progress and outcomes |

> Each activity should have exactly **one Accountable (A)** and at least one **Responsible (R)**. Multiple people can be Consulted or Informed.

---

## RACI Template

Copy the table below and fill in the cells for your project. Use the role abbreviations in the header row, or add/remove columns for roles not applicable to your project.

**Role abbreviations:**
- **PM** — Project Manager
- **PdM** — Product Manager
- **Dev** — Developer(s)
- **QA** — QA Lead / Test Engineer
- **UX** — UX Designer
- **BA** — Business Analyst
- **TW** — Technical Writer
- **Sponsor** — Executive Sponsor / Stakeholder
- **Support** — Support Lead / Customer Success

| Activity | PM | PdM | Dev | QA | UX | BA | TW | Sponsor | Support |
|---|---|---|---|---|---|---|---|---|---|
| Project charter approval | C | C | I | I | I | I | I | **A** | I |
| Backlog prioritization | C | **A** | C | C | C | R | I | I | C |
| Requirements documentation | I | A | C | C | C | **R** | C | I | C |
| Sprint / iteration planning | **R** | C | R | R | C | C | I | I | I |
| Feature development | I | I | **R** | C | C | C | I | I | I |
| UX design & prototyping | I | C | C | I | **R** | C | I | I | I |
| Test plan & QA execution | I | C | C | **R** | I | C | I | I | I |
| Documentation updates | I | C | C | I | I | I | **R** | I | C |
| Release go/no-go decision | **A** | C | C | C | I | I | C | C | C |
| Sponsor status update | **R** | C | I | I | I | I | I | **A** | I |
| Post-release support readiness | I | I | C | C | I | I | C | I | **R** |
| Risk register maintenance | **R** | C | C | C | I | C | I | I | I |
| Retrospective facilitation | **R** | C | C | C | C | C | C | I | I |

---

## How to fill out and use this template

1. **Start at kickoff.** Draft the RACI during or immediately after the project kickoff meeting while roles are fresh.
2. **Confirm accountable owners.** For every row, confirm that exactly one person (by name, not just role) is accountable.
3. **Share and review.** Share the completed RACI with all team members. Walk through it briefly to resolve disagreements.
4. **Revisit at major milestones.** Re-examine the RACI when project scope changes significantly or team members rotate off the project.
5. **Store with project artifacts.** Keep the RACI in the project repository alongside the Project Charter and Risk Register.

### Tips
- If a role is not applicable to your project, remove that column.
- If two people share the "Accountable" role for an activity, split the activity into two rows.
- Use names in parentheses next to abbreviations (e.g., `R (Alex)`) in your project-specific version for clarity.

---

## Example: Filled-in row

The row below illustrates how a cross-functional team handles a typical "Engineering -> QA Handoff":

| Activity | PM | PdM | Dev | QA | UX | BA | TW | Sponsor | Support |
|---|---|---|---|---|---|---|---|---|---|
| Engineering → QA handoff | **A** | I | R | R | I | I | I | I | I |

- The **PM** is accountable for ensuring the handoff happens on schedule.
- **Developers** are responsible for preparing the build, writing test notes, and notifying QA.
- The **QA Lead** is responsible for reviewing handoff artifacts and accepting or returning the build.

---

## Related docs
- [Roles and Personas](octoacme-roles-and-personas.md)
- [Handoff Checklists](octoacme-handoff-checklists.md)
- [Project Planning](octoacme-project-planning.md)
