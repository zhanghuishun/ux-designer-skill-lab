---
name: design-brief
description: Turn unstructured PM inputs (meeting notes, chat logs, scattered docs) into a structured design brief. Use for PRDs, review notes, or fragmented requirements to give enterprise UX designers clear design guidance.
intent: >-
  Convert unstructured product input (meetings, docs, chat) into a structured design brief. When PM information is scattered, organize it into clear guidance covering business context, product scope, constraints, users, and data characteristics.
type: component
theme: pm-artifacts
best_for:
  - "Turn meeting notes into a design brief"
  - "Organize scattered PM requirements"
  - "Prepare design guidance for B2B / enterprise UX designers"
scenarios:
  - "Generate a design brief from PM meeting notes"
  - "Turn a team chat thread about a new feature into a design brief"
  - "Create a design brief from PRD excerpts"
estimated_time: "5–15 minutes"
---

## Purpose
Produce a structured design brief from unstructured PM input (meetings, docs, chat). Use when information arrives in fragments and must become clear guidance for UX designers—especially in B2B/enterprise contexts. A brief sets the **boundary and context** for design work: not *how* to design, but *what* to design and *why*.

## Key Concepts

### The Golden Circle applied to design briefs
- **Why (business context):** Why build this? What business goal? What problem?
- **What (product scope):** What exactly do we build? In / out of scope?
- **How (constraints & users):** How is it used? What constraints? Who are the users?

### 5W1H for pulling requirements from messy sources
- **What:** Which capability or feature?
- **Why:** Why now? (business goal)
- **Who:** Who uses it? (roles)
- **When / Where:** Scenes and contexts?
- **How:** How it works? (data, interactions)

### Input source types
| Source | Typical content |
|--------|-----------------|
| Meeting notes | Clarifications, business context, PM expectations |
| Requirements docs | Feature lists, flows, user stories |
| Chat logs | Ad-hoc updates, priority shifts, detail confirmations |
| Email | Stakeholder asks, change descriptions |
| Product screenshots | Current state, improvement hooks |

### Why this works
- **Alignment:** PM and design share the same “what” and “why”
- **Boundaries:** Explicit in/out of scope limits creep
- **Verifiability:** Success metrics define when design is “right enough”
- **Decisions:** Constraints and user context steer design choices

---

## Application

### Step 1: Extract and bucket information

**A. Business context**
- **Business goal:** What should the business achieve? (e.g. lower ops cost, faster audits, compliance migration)
- **Core tension:** Current state? Where are users stuck? Why now?
- **Success metrics:** Which metrics prove success? (e.g. −30% task time, fewer form errors)

**B. Product scope**
- **Scope level:** □ Whole system / new product □ Sub-domain □ Single module □ Targeted improvement
- **This release (in scope):** Must design and ship
- **Future (on roadmap):** Not this release but planned
- **Explicitly out:** Not this release and no near-term plan
- **Dependencies:** Upstream, downstream, adjacent systems/products

**C. Constraints**
- **Surfaces:** □ Desktop □ Mobile □ Tablet
- **Technical:** Compatibility, performance, tech debt
- **Resources:** Design bandwidth, delivery timeline
- **Privacy / security:** Masking, permissions, compliance

**D. Users**
- **Roles:** How many? Who?
- **Frequency:** High / medium / low
- **Complexity:** Simple actions vs complex decisions

**E. Data**
- **Entities:** What data objects? (e.g. orders, approval tasks, customer records)
- **Volume:** □ Very large (pagination / virtualize) □ Tiny (strong empty states)
- **Refresh:** Real-time / near-real-time / batch
- **Provenance:** Internal / external / user-entered
- **Other:** Export, sensitive fields, etc.

---

### Step 2: Validate and complete

After bucketing:

1. **Coverage:** Are A–E all addressed?
2. **Consistency:** Do sources contradict? (e.g. scope in meeting vs doc)
3. **Open items:** Mark uncertain items `[TBD]`
4. **Assumptions:** Label inferences explicitly: `Assumption: …`

---

### Step 3: Generate the design brief

Write a Markdown file in the working directory using the structure below.

---

## Design Brief

### 1. Business context

**Business goal**

[What the business hopes to achieve with this initiative]

**Core conflict**

- **Current state:** [Situation today]
- **Pain point:** [Where users are stuck]
- **Trigger:** [Why this must happen now]

**Success metrics**

[Measurable signals after launch]

---

### 2. Product scope

**Scope level**
- [ ] Entire system / new product
- [ ] Sub-domain
- [ ] Single module
- [ ] Targeted improvement

**In scope (this release)**

[ ]

[ ]

**Future (roadmap)**

[ ]

[ ]

**Out of scope**

[ ]

[ ]

**Dependencies**
- Upstream:
- Downstream:
- Related systems:

---

### 3. Constraints

| Constraint type | Requirement |
|-----------------|-------------|
| Platform / surface |  |
| Technical |  |
| Resource |  |
| Security & compliance |  |

---

### 4. User information

| Role | Responsibility | Frequency | Complexity |
|------|----------------|-----------|------------|
|  |  |  |  |
|  |  |  |  |

---

### 5. Data information

**Data entity:**

1. [What data: e.g. orders / approvals / customers]

| Dimension | Analysis | Notes |
|-----------|----------|-------|
| **Volume** | □ Very large □ Medium □ Minimal | Large → paging/virtual scroll; minimal → empty states |
| **Update frequency** | □ Real-time □ Near-real-time □ Scheduled | Drives sync & caching |
| **Source** | □ Internal □ External □ User input | Drives fetch & error handling |
| **Other** |  | e.g. export, sensitive fields |

2. [Second entity if needed — same table pattern]

---

### 6. Open questions

| # | Question | Confirm with | Status |
|---|----------|--------------|--------|
| 1 |  |  | ⬜ |
| 2 |  |  | ⬜ |

---

### 7. Deliverables & timeline

**Milestones**

| Phase | Deliverable | Review gate | Due |
|-------|-------------|-------------|-----|
| Requirements clarified | Complete design brief | Align context with PM | YYYY-MM-DD |
| Concept / solution | First design pass | Internal design review | YYYY-MM-DD |
| Final solution | Final design | PM / business sign-off | YYYY-MM-DD |
| Handoff | Final UI + annotations | Dev can start build | YYYY-MM-DD |

**Deliverable notes**

1. **Complete design brief** — Sections 1–6 filled; PM-aligned context, scope, constraints  
   - [Full brief template — Appendix A](#appendix-a-full-design-brief-template)

2. **First design pass** — Key screens/modules: wireframes or low-fi prototype; core flows  
   - [Design proposal template](#appendix-b-design-proposal-template)

3. **Final design** — High-fidelity UI; prototype if needed; design notes  
   - [Final design checklist](#appendix-c-final-design-checklist)

4. **Handoff package** — Source files in the team’s UI tool; redlines; component notes if needed  
   - [Handoff checklist](#appendix-d-handoff-checklist)

**Timeline snippet**

```markdown
## Project timeline

| Task | Owner | Start | Due | Status |
|------|-------|-------|-----|--------|
| Clarify requirements & brief | PM + Designer | YYYY-MM-DD | YYYY-MM-DD | ⬜ In progress |
| Competitive / design research | Designer | YYYY-MM-DD | YYYY-MM-DD | ⬜ Not started |
| Solution design & review | Designer | YYYY-MM-DD | YYYY-MM-DD | ⬜ Not started |
| Finalize & hand off | Designer | YYYY-MM-DD | YYYY-MM-DD | ⬜ Not started |
```

---

### Appendix A: Full design brief template

```markdown
# Design Brief

## 1. Business context

**Business goal**
> [What the business hopes to achieve]

**Core conflict**
> - **Current state:** […]
> - **Pain point:** […]
> - **Trigger:** […]

**Success metrics**
> [Metrics after launch]

---

## 2. Product scope

**Scope level**
- [ ] Entire system / new product
- [ ] Sub-domain
- [ ] Single module
- [ ] Targeted improvement

**In scope**
- [ ]

**Future**
- [ ]

**Out of scope**
- [ ]

**Dependencies**
- Upstream:
- Downstream:
- Related systems:

---

## 3. Constraints

| Type | Requirement |
|------|-------------|
| Platform |  |
| Technical |  |
| Resource |  |
| Security & compliance |  |

---

## 4. Users

| Role | Responsibility | Frequency | Complexity |
|------|----------------|-----------|------------|
|  |  |  |  |

---

## 5. Data

**Entity:** [Describe the data]

| Dimension | Analysis | Notes |
|-----------|----------|-------|
| **Volume** | □ Very large □ Medium □ Minimal |  |
| **Update frequency** | □ Real-time □ Near-real-time □ Scheduled |  |
| **Source** | □ Internal □ External □ User input |  |
| **Other** |  |  |

---

## 6. Open questions

| # | Question | Confirm with | Status |
|---|----------|--------------|--------|
| 1 |  |  | ⬜ |

---

## 7. Deliverables & timeline

**Milestones**

| Phase | Deliverable | Review | Due |
|-------|-------------|--------|-----|
| … | … | … | YYYY-MM-DD |

**Timeline**

| Task | Owner | Start | Due | Status |
|------|-------|-------|-----|--------|
|  |  |  |  |  |
```

---

### Appendix B: Design proposal template

```markdown
# Design proposal

## 1. Design objectives
> Core problems and goals this solution addresses

## 2. Design solution

### 2.1 Overall approach
> Concept and principles

### 2.2 Information architecture
> Structure and hierarchy

### 2.3 Core flows
> User flows (diagram or narrative)

### 2.4 Screens
> Notes per screen / module

## 3. Key design decisions

| Decision | Solution | Rationale |
|----------|----------|-----------|
|  |  |  |

## 4. Open questions
> Items for PM / business

## 5. Next steps
> Follow-up work
```

---

### Appendix C: Final design checklist

- [ ] Solution passed internal design review  
- [ ] Solution confirmed with PM / business  
- [ ] All screens annotated (default, error, empty, loading, etc.)  
- [ ] Flows cover all scenarios  
- [ ] Edge cases considered  
- [ ] Meets constraints (platform, tech, resources)  
- [ ] Meets security & compliance  

---

### Appendix D: Handoff checklist

- [ ] Files named and organized per team convention  
- [ ] Redlines / specs complete and accurate  
- [ ] Component / token notes shared if required  
- [ ] Developers have access to deliverables  
- [ ] Written design notes published  
- [ ] Handoff review done  

---

## Examples

### Example 1: Meeting notes → brief

**Input (meeting notes):**
```
We reviewed the next approval flow. Approvers must use desktop today, but many are
often in the field—they need mobile. Flow: submitter creates → approver acts → done.

This release: mobile approval only. Desktop improvements later.

Business goal: let approvers work on mobile and speed up approvals.
Target: cut approval handling time by 50%.

Constraint: mobile must use WebView, not native.

Roles: approver, submitter, admin.
Data: mostly approval tasks; ~100k records in the system.
```

**Output (generated brief):**
```markdown
## Design Brief

### 1. Business context

**Business goal**
> Let approvers handle work on mobile and improve approval efficiency

**Core conflict**
> **Current:** Approvals are desktop-only  
> **Pain:** Approvers are often away from desk  
> **Trigger:** Request for mobile workflows; efficiency impact  

**Success metrics**
> Approval handling time −50%

---

### 2. Product scope

**Scope level**
- [ ] Entire system
- [ ] Sub-domain
- [x] Single module
- [ ] Targeted improvement

**In scope**
- Mobile approval handling

**Future**
- Desktop approval improvements

**Out of scope**
- Desktop changes not in this release

**Dependencies**
- Upstream: approval creation
- Downstream: approval storage
- Related systems: none

---

### 3. Constraints

| Type | Requirement |
|------|-------------|
| Platform | Mobile WebView |
| Technical |  |
| Resource |  |
| Security & compliance |  |

---

### 4. Users

| Role | Responsibility | Frequency | Complexity |
|------|----------------|-----------|------------|
| Approver | Process | High | Medium |
| Submitter | Create | Medium | Low |
| Admin | Configure | Low | High |

---

### 5. Data

**Entity:** Approval tasks

| Dimension | Analysis | Notes |
|-----------|----------|-------|
| **Volume** | □ Very large □ Medium □ Minimal | ~100k — medium |
| **Update frequency** |  |  |
| **Source** |  |  |
| **Other** |  |  |

---

### 6. Open questions

| # | Question | Confirm with | Status |
|---|----------|--------------|--------|
```

---

## Common pitfalls

### Pitfall 1: Writing a PRD, not a brief
**Symptom:** Detailed flows, interaction specs, or wireframe-level detail in the brief  
**Impact:** Creativity drops; the doc becomes a task list  
**Fix:** Brief = *what* and *why*. *How* belongs in later design work  

### Pitfall 2: Designing before buckets are filled
**Symptom:** No structured pass over A–E  
**Impact:** Gaps surface mid-design; rework  
**Fix:** Check A–E; mark unknowns `TBD`  

### Pitfall 3: Unlabeled assumptions
**Symptom:** Guesses presented as facts  
**Impact:** Wrong foundations; large rework  
**Fix:** Prefix with `Assumption:`; validate with PM early  

### Pitfall 4: Fuzzy in/out of scope
**Symptom:** “Not now” vs “never” unclear  
**Impact:** Scope creep or missed must-haves  
**Fix:** For “out,” say “not this release and no near-term plan”  

### Pitfall 5: No success metrics
**Symptom:** Know the feature, not what “good” means  
**Impact:** No way to validate or iterate  
**Fix:** At least one measurable success metric  

---

## References

### Mental models
- Golden Circle — Simon Sinek  
- 5W1H analysis  

### Related skills
- `skills/user-story/SKILL.md` — User stories (often after the brief)  
- `skills/problem-statement/SKILL.md` — Problem framing  

### Further reading
- Nielsen Norman Group — enterprise / B2B product UX  
- *The Design of Everyday Things* — Don Norman  

---

**Skill type:** Component  
**Suggested artifact filename:** `design-brief.md`  
**Dependencies:** None (standalone)  
