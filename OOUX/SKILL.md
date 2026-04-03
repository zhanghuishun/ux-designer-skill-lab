---
name: ooux
description: Apply OOUX (Object Oriented User Experience) method to design intuitive B2B products. Use when analyzing business requirements, structuring information architecture, or designing complex enterprise systems.
intent: >-
  Design user experiences that align with users' mental models by treating business objects as first-class citizens in the UX. OOUX helps Product Managers identify core business objects, define their relationships, determine user actions on those objects, and specify their attributes—creating products that are easier to learn, use, and maintain.
type: component
theme: discovery-definition
estimated_time: "45-60 min"
---

## Purpose

OOUX (Object Oriented User Experience) applies object-oriented programming concepts to user experience design. Instead of designing screens around tasks (task-based), OOUX designs around business objects (object-based)—the nouns users work with.

**Core Value:**
- **For Users:** Products match mental models, are easier to learn/use, and require fewer clicks
- **For Business:** Reduced development/testing costs, faster onboarding, clearer IT-business communication

OOUX bridges the gap between "doing the right thing" (Design Thinking) and "doing things right" (Interaction Design)—it's the translator from user needs to interaction solutions.

## Key Concepts

### The ORCA Framework

OOUX follows a four-step methodology known as ORCA:

| Step | Full Name | What It Produces |
|------|-----------|------------------|
| **O** | Objects | Core business entities (e.g., Order, Customer, Product) |
| **R** | Relationships | How objects connect (aggregation, composition, inheritance) |
| **C** | Call to Actions | User operations on objects (add, edit, delete, view) |
| **A** | Attributes | Properties that describe each object |

### Business Object Definition

A valid business object has four characteristics (common criteria in enterprise information architecture and object modeling):

1. **Essential to business operations** — Cannot be ignored in enterprise management
2. **Has unique identifier** — Distinguishable from other instances
3. **Independent with attributes** — Can be described by properties
4. **Can be instantiated** — Has concrete real-world examples

### Object Relationship Types

| Relationship | Description | UI Implication |
|--------------|-------------|----------------|
| **Aggregation** | "Has-a" — Object contains other objects (e.g., Order has OrderItems) | Shared operations: list/table view, filters, batch actions |
| **Composition** | "Part-of" — Object is component of another (e.g., Comment is part of Product) | Usually displayed together; prevents "dead ends" |
| **Inheritance** | "Is-a" — Child shares parent properties (e.g., Electronics extends Product) | Shared operations across child types |

### Objects vs. Tasks

| Approach | Thinking | Example |
|----------|----------|---------|
| **Task-based (Traditional)** | "What does user need to do?" | Transfer Asset, Return Asset, Compensate Asset (3 pages) |
| **Object-based (OOUX)** | "What does user work with?" | Asset object with operations: Transfer, Return, Compensate (1 page) |

---

## Application

### Step 1: Identify Business Objects

**Input:** User stories, business process documentation, or existing system analysis

**Process:**
1. Extract nouns from user stories — these are potential objects
2. Apply the four-character test:
   - Is it essential to business? ✓
   - Does it have a unique ID? ✓
   - Does it have describable properties? ✓
   - Can it be instantiated? ✓
3. For complex products, conduct a workshop with BA, UX, Dev, and Business reps

**Output:** List of business objects with brief descriptions

```
Example: E-commerce System
- Product (offering with SKU, name, price)
- Customer (buyer with contact, address)
- Order (transaction with items, status, total)
- Cart (aggregation of products for purchase)
- Review (customer feedback on product)
```

---

### Step 2: Describe Object Relationships

**Process:**
1. For each object, identify its connection to other objects
2. Classify relationships:
   - **Aggregation:** "X has many Y" (Order → OrderItems)
   - **Composition:** "Y is part of X" (Comment → Product)
   - **Inheritance:** "Y is a type of X" (Laptop → Product)
3. Express in plain language: "[Object] [verb] [Object]"

**Output:** Relationship diagram or list

```
Example E-commerce Relationships:
- Product ←aggregation→ Cart (products can be added to cart)
- Order ←composition→ OrderItem (order contains line items)
- Product ←inheritance→ Clothing, Electronics (product categories)
- Customer ←association→ Order (customer has orders)
```

**Quality Check:** Relationships should be explainable in one sentence without jargon.

---

### Step 3: Define Object Operations (CTAs)

**Process:**
1. For each object, ask: "What can users DO with this?"
2. Standard operations: Create, Read, Update, Delete (CRUD)
3. Add domain-specific operations based on user stories
4. Note: Operations change object STATE; these are NOT operations:
   - Page-level micro-interactions (expand/collapse, sort)
   - Attribute changes (selecting product color)

**State-Based Operations:**
Objects have lifecycles—their available operations change based on state:

| Object | State | Available Operations |
|--------|-------|----------------------|
| Expense Claim | Draft | Save, Submit |
| Expense Claim | Pending Approval | Withdraw |
| Expense Claim | Approved | View, Print |
| Expense Claim | Rejected | Edit, Resubmit |

**Output:** Object-Operation matrix

---

### Step 4: Define Object Attributes

**Process:**
1. List all properties that describe each object
2. Classify attributes:
   - **Content:** Descriptive info (text, images)
   - **Status:** Filterable/sortable values (state, type)
   - **Association:** Links to related objects

3. Prioritize using:
   - Identity first (what instance is this?)
   - Importance: high-value → low-value
   - Usage frequency: high-frequency → low-frequency
   - Data type and space constraints

**Output:** Attribute lists per object

---

### Step 5: Validate and Apply

**Validation Checklist:**
- [ ] Can users find any object in ≤3 clicks?
- [ ] Are related objects connected in UI?
- [ ] Do operation names match user vocabulary?
- [ ] Are attribute priorities aligned with user needs?
- [ ] Does the object model enable future scaling?

**Application to Design:**
- Object model → Page structure
- Relationships → Navigation links
- Operations → Action buttons
- Attributes → Form fields and list columns

---

## Examples

### Example: Asset Management System (Before vs. After)

**Before (Task-based):**
```
├── Asset Transfer Page
├── Asset to Personal Page
├── Asset Compensation Page
└── Asset Return Page
```

Problems:
- 4 pages for related operations
- Doesn't match user mental model (find asset first, then act)
- High development cost

**After (OOUX-based):**
```
├── Asset Object
│   ├── Operations: Transfer, To Personal, Compensate, Return
│   ├── Attributes: Asset ID, Description, Status, Owner
│   └── Related: Asset Transfer Request (electronic flow)
```

Result: Single page for core operations; clear mental model

---

### Example: Car Dealership CRM

**Objects Identified:**
- Consumer (potential buyer)
- Opportunity (sales opportunity)
- Test Drive (appointment)
- Order (purchase)
- Follow-up (communication log)

**Relationships:**
- Consumer ←has many→ Opportunity
- Consumer ←has many→ Test Drive
- Consumer ←has many→ Order
- Consumer ←has many→ Follow-up

**Key Operations by Object:**
| Object | Operations |
|--------|------------|
| Consumer | Add, Edit, View, Delete, Top/Pin |
| Opportunity | Create, Stage Update, Win/Lose, Add Follow-up |
| Test Drive | Schedule, Complete, No-show |
| Order | Create, Modify, Cancel, Fulfill |

**Attributes Priority:**
| Object | Priority Attributes |
|--------|---------------------|
| Consumer | Name, Phone, Interest Level, Last Contact |
| Opportunity | Customer, Vehicle, Stage, Estimated Close |
| Test Drive | Date, Time, Vehicle, Location, Status |

---

## Common Pitfalls

### Pitfall 1: Confusing Tasks with Objects
**Symptom:** Creating separate pages for each user task

**Example:** "Transfer Asset" as a top-level menu item instead of "Asset" with "Transfer" operation

**Fix:** Ask "What object does the user work with?" not "What task do they perform?"

---

### Pitfall 2: Ignoring Object Lifecycle
**Symptom:** Showing all operations regardless of object state

**Example:** Allowing "Edit" on an already-approved expense claim

**Fix:** Map operations to states; show only valid operations per state

---

### Pitfall 3: Mixing Aggregation with Composition
**Symptom:** Related objects shown in different places, breaking context

**Example:** Product details on Page A, reviews on Page B with no visible connection

**Fix:** Composition relationships (part-of) should appear together; use links for aggregation

---

### Pitfall 4: No Unique Answer
**Symptom:** Team argues about "correct" object model

**Fact:** Object modeling has no single correct answer—models reflect the modeler's interpretation

**Fix:** Focus on models that solve user problems; validate with user research

---

### Pitfall 5: Skipping Relationship Mapping
**Symptom:** Objects exist but navigation between them is unclear

**Example:** "Customer" page has no link to their "Orders"

**Fix:** Map all relationships to navigation paths; test with user journeys

---

### Pitfall 6: Over-Designing Attributes
**Symptom:** Listing every possible attribute, overwhelming users

**Fix:** Show only key attributes in list views; reveal details on demand

---

### Pitfall 7: Ignoring System Vocabulary
**Symptom:** Same object called different names across pages ("Customer" vs "Client" vs "Account")

**Consequence:** User confusion; perception of unprofessionalism

**Fix:** Create enterprise-wide terminology standard; enforce in design system

---

## References

### Related Skills
- `skills/information-architecture/SKILL.md` — Complements OOUX with navigation structure
- `skills/user-story-mapping/SKILL.md` — Source material for object identification
- `skills/proto-persona/SKILL.md` — Defines user roles that interact with objects
- `skills/ux-design-principles/SKILL.md` — Foundational UX principles

### External Resources
- Alan Cooper, *About Face: The Essentials of Interaction Design* — Introduces mental model concepts
- UML Class Diagrams — For formal relationship modeling
- User Story format: "As a [role], I want [feature], so that [value]"

### Provenance
- Based on OOUX White Paper
- Combines Design Thinking, UML, and User Story methods

---

**Skill type:** Component
**Suggested filename:** `ooux.md`
**Dependencies:** Works well with `skills/information-architecture`, `skills/user-story-mapping`