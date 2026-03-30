---
name: ASCII-wireframe
description: Create ASCII wireframes to communicate UI layout, structure, and component placement. Use when quickly sketching ideas, documenting screen designs, or communicating layout intent to designers and engineers.
intent: >-
  Generate low-fidelity wireframes using ASCII art to visualize page layouts, component hierarchies, and interaction patterns. Use this to rapidly ideate on layouts, document existing screen structures, communicate design intent without needing design tools, or create text-based design specifications that can be easily shared and version-controlled.
type: component
theme: design-critique
best_for:
  - "Rapidly sketching page layouts during ideation sessions"
  - "Documenting screen structures in design specifications"
  - "Communicating layout intent to engineers before visual design"
  - "Creating text-based wireframes for version control"
  - "Reviewing and commenting on layout structure"
scenarios:
  - "Sketch the layout of a new dashboard screen"
  - "Document the component structure of a form page"
  - "Communicate the difference between mobile and desktop layouts"
  - "Create a series of wireframes for a user flow"
  - "Review a screen's layout structure"
estimated_time: "5-15 min per wireframe"
---

## Purpose

Wireframes are low-fidelity visual representations of UI layout that communicate structure without the distraction of visual design. ASCII wireframes use text characters to represent UI elements, making them:
- **Fast to create** — no design tools required
- **Easy to share** — plain text, works anywhere
- **Version-controllable** — diff-friendly, works with git
- **Discussion-focused** — encourages feedback on structure, not aesthetics

This skill helps UX Designers and Product Managers:
- **Communicate layout intent** clearly without design tools
- **Document existing structures** for reference
- **Enable rapid iteration** through text-based sketching
- **Support design discussions** with concrete visual references

---

## Key Concepts

### ASCII Wireframe Elements

| Element | ASCII Symbol | Usage |
|---------|--------------|-------|
| Container/Border | `┌─┐│└┘├┤┬┴┼` | Layout regions, cards, sections |
| Horizontal Line | `─` or `-` | Separators, section dividers |
| Vertical Line | `│` | Column divisions, list items |
| Menu Icon | `≡` or `☰` | Hamburger menu, navigation |
| User Avatar | `◉` or `○` | User profile, avatar placeholder |
| Button | `[ Button ]` or `< Button >` | Action buttons |
| Input Field | `[____________]` | Text input, search |
| Dropdown | `[▼ Select ]` | Selection controls |
| Checkbox | `[ ]` / `[x]` | Boolean options |
| Radio | `( )` / `(*)` | Single selection |
| Image Placeholder | `[  IMG  ]` | Image/media areas |
| Loading | `...` or `///` | Loading states |
| Arrow | `→` or `->` | Navigation, relationships |
| Link | `~link~` or `_link_` | Clickable text |
| Ellipsis | `...` | Truncation, overflow |
| Star/Favorite | `★` or `☆` | Rating, favorites |
| Notification | `●` | Badge, notification indicator |

### Layout Conventions

```
┌─────────────────────────────────────────────────────┐
│                    HEADER                           │
│  [Logo]        [Navigation Tabs]        [User ▼]   │
├──────────────┬──────────────────────────────────────┤
│              │                                      │
│   SIDEBAR    │              MAIN CONTENT            │
│              │                                      │
│  • Item 1    │  ┌─────────────┐  ┌─────────────┐   │
│  • Item 2    │  │   Card 1    │  │   Card 2    │   │
│  • Item 3    │  │   [IMG]    │  │   [IMG]    │   │
│              │  │   Title    │  │   Title    │   │
│  ──────────  │  │   Desc     │  │   Desc     │   │
│              │  └─────────────┘  └─────────────┘   │
│  • Section   │                                      │
│              │  ┌─────────────────────────────┐    │
│              │  │        Full Width           │    │
│              │  │        Section              │    │
│              │  └─────────────────────────────┘    │
│              │                                      │
└──────────────┴──────────────────────────────────────┘
```

---

## Workflow

### Step 1: Clarify Platform (MUST ASK FIRST)

Before creating any wireframe, ALWAYS confirm the platform with the user. Do NOT assume.

Ask the user:
- **"Is this for web, mobile (iOS/Android), or desktop?"**
- **"Is this for frontend (user-facing) or backend (admin/management)?"**

If unclear, request clarification before proceeding.

### Step 2: Choose Appropriate Layout

Based on the platform:
- **Web (Desktop)**: Full sidebar + header layout, multi-column
- **Web (Tablet)**: Collapsible sidebar, 2-column max
- **Mobile**: Single column, hamburger menu, bottom navigation
- **Desktop App**: May include native window chrome

### Step 3: Build Wireframe

Follow the conventions in the rest of this skill.

---

## Application

<!--ts-->
### Table of Contents

1. [Part 1: ASCII Conventions Reference](#part-1-ascii-conventions-reference)
   - [Border Drawing Guide](#border-drawing-guide)
   - [Spacing and Alignment](#spacing-and-alignment)
   - [Complex Layout Patterns](#complex-layout-patterns)
2. [Part 2: Common Component Wireframes](#part-2-common-component-wireframes)
   - [Navigation Components](#navigation-components)
   - [Form Components](#form-components)
   - [Data Display Components](#data-display-components)
   - [Feedback Components](#feedback-components)
   - [Modal/Drawer Separation](#modaldrawer-separation)
3. [Part 3: Page-Level Wireframes](#part-3-page-level-wireframes)
   - [Dashboard Page](#dashboard-page)
   - [Form Page](#form-page)
   - [List/Grid Page](#listgrid-page)
4. [Part 4: Multi-Container Wireframes](#part-4-multi-container-wireframes)
   - [Page + Modal Pattern](#page--modal-pattern)
   - [Page + Drawer Pattern](#page--drawer-pattern)
   - [Page + Modal + Drawer Pattern](#page--modal--drawer-pattern)
5. [Part 5: Responsive Wireframe Comparison](#part-5-responsive-wireframe-comparison)
<!--te-->

### Part 1: ASCII Conventions Reference

#### Border Drawing Guide

```text
Single Box:
┌─────────────┐
│   Content   │
└─────────────┘

Rounded Corners (optional):
╭─────────────╮
│   Content   │
╰─────────────╯

Double Box (emphasized):
┌─────────────┐
│             │
│  ┌────────┐ │
│  │ Content│ │
│  └────────┘ │
│             │
└─────────────┘

Header + Body:
┌────────────────────┐
│     Header         │
├────────────────────┤
│     Content        │
│     Content        │
└────────────────────┘
```

#### Spacing and Alignment

```text
Standard Padding (2 spaces):
┌─────────────────┐
│  Content here   │
└─────────────────┘

Compact (1 space):
┌───────────────┐
│ Content here  │
└───────────────┘

Loose (4 spaces):
┌───────────────────┐
│     Content       │
│     here          │
└───────────────────┘
```

#### Complex Layout Patterns

```text
Two-Column Layout:
┌─────────┬─────────┐
│  Col 1  │  Col 2  │
│         │         │
├─────────┼─────────┤
│  Col 1  │  Col 2  │
│         │         │
└─────────┴─────────┘

Sidebar Layout:
┌──────┬──────────────┐
│ Side │    Main      │
│ bar  │   Content    │
│      │              │
│      ├──────────────┤
│      │   Another    │
│      │    Section   │
└──────┴──────────────┘

Card Grid (2x2):
┌───────────┐┌───────────┐
│   Card 1  ││   Card 2  │
│  [Image]  ││  [Image]  │
│   Title   ││   Title   │
└───────────┘┌───────────┘
│   Card 3  ││   Card 4  │
│  [Image]  ││  [Image]  │
│   Title   ││   Title   │
└───────────┘┌───────────┘
```

---

### Part 2: Common Component Wireframes

#### Navigation Components

```text
Top Navigation Bar:
┌─────────────────────────────────────────────────────┐
│ [Logo]     [Dashboard] [Reports] [Settings]  [👤] │
└─────────────────────────────────────────────────────┘

Sidebar Navigation:
┌──────────────┐
│  [Logo]      │
├──────────────┤
│  ▶ Dashboard │
│    Reports   │
│    Settings  │
│              │
│  ──────────  │
│    About     │
│    Help      │
└──────────────┘

Breadcrumb:
Dashboard / Orders / Order #1234

Tabs (● means selected):
[ ● Details ] [ History ] [ Files ]
[ Details ] [ ● History ] [ Files ]
```

#### Form Components

```text
Input Fields:
Label
[____________________]

Required Field:
Label *
[____________________]

Textarea:
Label
[____________________]
[____________________]
[____________________]

Select/Dropdown:
Role
[Admin           ▼]

Checkbox Group:
☑ Read
☑ Write
☑ Delete

Radio Group:
(○) Option A
(●) Option B
(○) Option C

Form with Labels:
┌────────────────────────┐
│ Username               │
│ [___________________]  │
│                        │
│ Email                  │
│ [___________________]  │
│                        │
│ Role                   │
│ [Admin            ▼]   │
│                        │
│        [ Submit ]      │
└────────────────────────┘
```

#### Data Display Components

```text
Data Table:
┌────┬───────────┬──────────┬────────┐
│ ID │   Name    │  Status  │ Action │
├────┼───────────┼──────────┼────────┤
│ 01 │  Item A   │  Active  │[Edit]  │
│ 02 │  Item B   │  Pending │[Edit]  │
│ 03 │  Item C   │  Active  │[Edit]  │
└────┴───────────┴──────────┴────────┘

List Item:
┌─────────────────────────────────────────────┐
│ [◉]  Title of the item            [Button] │
│      Subtitle or description...             │
│      Date or metadata            ★★★★☆     │
└─────────────────────────────────────────────┘

Card Component:
┌─────────────────────────┐
│     [     IMG     ]     │
│                         │
│    Card Title Here      │
│    Brief description    │
│    of the content...    │
│                         │
│  [Primary]  [Secondary] │
└─────────────────────────┘
```

#### Feedback Components

```text
Alert/Message:
┌─────────────────────────────────────────────┐
│ ⚠ Warning: This action cannot be undone.   │
└─────────────────────────────────────────────┘

Success Message:
✓ Operation completed successfully.

Error State:
┌─────────────────────────────────────────────┐
│ ✗ Error: Unable to save changes.            │
│   Please check your connection and try      │
│   again.                        [Try Again] │
└─────────────────────────────────────────────┘

Loading State:
[ █████████████░░░░░░░ ] 75% Loading...

Empty State:
┌─────────────────────────────────────────────┐
│                                             │
│              [ Icon/Illustration ]          │
│                                             │
│            No items found                   │
│        Create your first item to get        │
│              started.                       │
│                                             │
│            [ Create New ]                   │
│                                             │
└─────────────────────────────────────────────┘
```

#### Tab Components

```text
Tabs (● means selected):
[ ● Details ] [ History ] [ Files ]
[ Details ] [ ● History ] [ Files ]

Tab Badges:
[ Details ] [ History (3) ] [ Files ]

Tab with Dropdown:
[ All Items ▼ ] ───────────────────────────
```

#### Modal/Dialog Components

> NOTE: When showing a modal/dialog, display it as a SEPARATE container from the main page. See Part 4 for best practices.

```text
Modal Dialog (centered overlay):
┌─────────────────────────────────────────────┐
│                                             │
│  ┌─────────────────────────────────────┐   │
│  │  Confirm Action              [X]    │   │
│  ├─────────────────────────────────────┤   │
│  │                                     │   │
│  │  Are you sure you want to delete   │   │
│  │  this item? This action cannot be  │   │
│  │  undone.                            │   │
│  │                                     │   │
│  │  Affected: Order #12345            │   │
│  │                                     │   │
│  ├─────────────────────────────────────┤   │
│  │               [Cancel]  [Delete]   │   │
│  └─────────────────────────────────────┘   │
│                                             │
└─────────────────────────────────────────────┘

Modal Header Style Variants:
[ Header Title          ]  (without X - use only if no close action)
┌─ Confirmation ─────────────────────────────┐  (with title bar)
```

#### Drawer/Side Panel

```text
Drawer (Right side, overlays page):
┌────────────────────┐ ┌───────────────────────────────┐
│ Main Content       │ │ Drawer Header         [X]    ││
│                    │ ├───────────────────────────────┤│
│                    │ │                               ││
│                    │ │ Drawer Content                ││
│                    │ │                               ││
│                    │ │                               ││
│                    │ │                               ││
│                    │ ├───────────────────────────────┤│
│                    │ │       [Cancel]  [Save]        ││
└────────────────────┘ └───────────────────────────────┘
```

---

### Part 3: Page-Level Wireframes

#### Dashboard Page

```text
┌────────────────────────────────────────────────────────┐
│ Dashboard                           [Search] [🔔] [👤]│
├─────────┬──────────────────────────────────────────────┤
│         │  ┌─────────┐ ┌─────────┐ ┌─────────┐        │
│ Dashboard│  │  Total  │ │  Active │ │  Revenue│        │
│ Reports  │  │  Users  │ │  Orders │ │ $12,450 │        │
│ Settings │  │  1,234  │ │   567   │ │  +12%   │        │
│         │  └─────────┘ └─────────┘ └─────────┘        │
│ ─────── │                                              │
│ Profile │  Recent Activity                    [View]  │
│         │  ┌────────────────────────────────────┐     │
│         │  │ ◉ New user registered             │     │
│         │  │   John Doe - 2 minutes ago        │     │
│         │  ├────────────────────────────────────┤     │
│         │  │ ◉ Order completed                 │     │
│         │  │   Order #1234 - $450 - 5m ago     │     │
│         │  ├────────────────────────────────────┤     │
│         │  │ ◉ Payment received                │     │
│         │  │   $1,200 from Acme Inc - 1h ago   │     │
│         │  └────────────────────────────────────┘     │
└─────────┴──────────────────────────────────────────────┘
```

#### Form Page

```text
┌────────────────────────────────────────────────────────┐
│ New Order                                  [Cancel]    │
├────────────────────────────────────────────────────────┤
│                                                        │
│  Customer Information                                  │
│  ─────────────────────────────────────────             │
│                                                        │
│  Customer *                                            │
│  [Search customers...                            ▼]   │
│                                                        │
│  ┌──────────────────┐ ┌──────────────────┐            │
│  │ First Name       │ │ Last Name        │            │
│  │ [________________]│ │[________________]│            │
│  └──────────────────┘ └──────────────────┘            │
│                                                        │
│  Order Details                                         │
│  ─────────────────────────────────────────             │
│                                                        │
│  Product *                                             │
│  [Select product...                              ▼]   │
│                                                        │
│  Quantity *                                            │
│  [1   ]                                                │
│                                                        │
│  ┌─────────────────────────────┐                       │
│  │ Notes                       │                       │
│  │ [_________________________]│                       │
│  │ [_________________________]│                       │
│  └─────────────────────────────┘                       │
│                                                        │
│                          [ Cancel ]    [ Submit Order ]│
└────────────────────────────────────────────────────────┘
```

#### List/Grid Page

```text
┌────────────────────────────────────────────────────────┐
│ Orders                              [+ New]  [Search] │
├─────────┬──────────────────────────────────────────────┤
│ All     │  Filter: [Status ▼] [Date ▼]        [Export]│
│ Pending │ ───────────────────────────────────────────  │
│ In      │                                                │
│ Shipped │  ┌───────────┐ ┌───────────┐ ┌───────────┐   │
│ Deliv.  │  │ #ORD-001  │ │ #ORD-002  │ │ #ORD-003  │   │
│ Returns │  │ Acme Corp │ │ Beta Inc  │ │ Gamma Co  │   │
│         │  │ $1,200    │ │ $850      │ │ $2,400    │   │
│ ─────── │  │ Pending   │ │ Shipped   │ │ Delivered │   │
│ Date    │  │ Jan 15    │ │ Jan 14    │ │ Jan 13    │   │
│         │  │ [View]    │ │ [View]    │ │ [View]    │   │
│         │  └───────────┘ └───────────┘ └───────────┘   │
│         │                                                │
│         │  ┌───────────┐ ┌───────────┐ ┌───────────┐   │
│         │  │ #ORD-004  │ │ #ORD-005  │ │ #ORD-006  │   │
│         │  │ Delta Org │ │ Epsilon   │ │ Zeta Ltd  │   │
│         │  │ $960      │ │ $1,100    │ │ $780      │   │
│         │  │ Cancelled │ │ Pending   │ │ Shipped   │   │
│         │  │ Jan 12    │ │ Jan 11    │ │ Jan 10    │   │
│         │  │ [View]    │ │ [View]    │ │ [View]    │   │
│         │  └───────────┘ └───────────┘ └───────────┘   │
│         │                                              │
├────────────────────────────────────────────────────────┤
│Showing 1-6 of 234             [< Prev] [1] [2] [Next >]|
└────────────────────────────────────────────────────────┘
```

---

### Part 4: Multi-Container Wireframes

A critical skill in wireframing is correctly separating:
1. **Page/View** - The main container the user is on
2. **Modal** - A dialog that overlays the page (centered)
3. **Drawer** - A side panel that slides in from the right (or left)

#### Page + Modal Pattern

Show page and modal as SEPARATE containers. The [X] in modal header indicates it's an overlay:

```
┌──────────────────────────────────────────────────────────┐
│ PAGE: Skill Detail                          [User] [🔔] │
├──────────────────────────────────────────────────────────┤
│ ┌────────────────┐  ┌─────────────────────────────────┐  │
│ │ Skill: Claude  │  │ Author: John Doe               │  │
│ │ Category: AI   │  │ Version: 2.1                   │  │
│ │                │  │ Status: Published              │  │
│ │ [Edit Button]  │  └─────────────────────────────────┘  │
│ └────────────────┘                                        │
│ [ ● Details ] [ Reviews ]                                │
└──────────────────────────────────────────────────────────┘


┌──────────────────────────────────────────────────────────┐
│ MODAL: Edit Skill                               [X]      │
├──────────────────────────────────────────────────────────┤
│                                                          │
│  Skill Name                                              │
│  [______________________________]                        │
│                                                          │
│  Description                                             │
│  [______________________________]                        │
│  [______________________________]                        │
│                                                          │
│                 [Cancel]  [Save]                         │
└──────────────────────────────────────────────────────────┘
```

#### Page + Drawer Pattern

Drawer slides in from the right, shown alongside the page:

```
┌─────────────────────────────────────────────────┐
│ PAGE: Dashboard                     [User] [🔔]│
├────────────┬────────────────────────────────────┤
│  Dashboard │                                     │
│  Reports   │   [Filter] button here             │
│  Settings  │                                     │
└────────────┴────────────────────────────────────┘
┌─────────────────────────────────────────────────┐─────────────────────────┐
│                                                │ DRAWER: Filter  [X]     │
│                                                ├─────────────────────────┤
│                                                │ Category                │
│                                                │ [ ] All                 │
│                                                │ [ ] AI                  │
│                                                │ [ ] Design              │
│                                                │                         │
│                                                │ Status                  │
│                                                │ ( ) Any                 │
│                                                │ (•) Active              │
│                                                │ ( ) Inactive            │
│                                                ├─────────────────────────┤
│                                                │           [Clear] [Apply]
└─────────────────────────────────────────────────┴─────────────────────────┘
```

#### Page + Modal + Drawer Pattern

Complex interactions showing all three container types in sequence:

```
┌───────────────────────────────────────────────────────┐
│ PAGE: Skill List                          [+ Add New]│
├────────────┬──────────────────────────────────────────┤
│  All       │  ┌──────────┐ ┌──────────┐ ┌──────────┐  │
│  Active    │  │ Skill A  │ │ Skill B  │ │ Skill C  │  │
│  Pending   │  │ [Edit]   │ │ [Edit]   │ │ [Edit]   │  │
│  Archived  │  └──────────┘ └──────────┘ └──────────┘  │
└────────────┴──────────────────────────────────────────┘


┌───────────────────────────────────────────────────────┐
│ MODAL: Confirm Publish                       [X]      │
├───────────────────────────────────────────────────────┤
│                                                       │
│  This skill will be published to the marketplace.   │
│                                                       │
│                  [Cancel]  [Publish]                  │
└───────────────────────────────────────────────────────┘


┌───────────────────────────────────────────────────────┐
│ PAGE: Skill List                          [+ Add New]│
├────────────┬──────────────────────────────────────────┤
│  All       │  ┌──────────┐ ┌──────────┐ ┌──────────┐  │
│  Active    │  │ Skill A  │ │ Skill B  │ │ Skill C  │  │
│  Pending   │  │ [Edit]   │ │ ● Edit   │ │ [Edit]   │  │
│  Archived  │  └──────────┘ └──────────┘ └──────────┘  │
└────────────┴──────────────────────────────────────────┘
┌───────────────────────────────────────┬───────────────┐
│                                       │ DRAWER: Edit  │
│                                       │         [X]   │
│                                       ├───────────────┤
│                                       │ Name          │
│                                       │ [_________]   │
│                                       │               │
│                                       │ Description   │
│                                       │ [_________]   │
│                                       │ [_________]   │
│                                       ├───────────────┤
│                                       │ [Cancel][Save]│
└───────────────────────────────────────┴───────────────┘
```

---

### Part 5: Responsive Wireframe Comparison

```text
Desktop Layout (≥1024px)          Mobile Layout (<768px)
┌─────────────────────────┐       ┌─────────────┐
│ Header                  │       │ [☰] [Logo] │
├────────┬────────────────┤       ├─────────────┤
│ Side   │ Content        │       │ Content     │
│ bar    │                │       │             │
│        │                │       │             │
│        │                │       │             │
│        │                │       │             │
└────────┴────────────────┘       └─────────────┘

tablet Layout (768-1024px)
┌─────────────────────────┐
│ Header                  │
├─────────────────────────┤
│ Content (full width)    │
│ with collapsible nav   │
└─────────────────────────┘
```

---

## Template Usage

For standard templates, see: **[template.md](./references/template.md)**

---

## Common Pitfalls

### Pitfall 1: Inconsistent Character Usage

**Symptom:** Mixing different border styles (`┌` mixed with `+`)

**Fix:** Pick one style and use consistently throughout

---

### Pitfall 2: Misaligned Elements

**Symptom:** Columns don't line up, spacing is irregular

**Fix:** Use monospaced font; count characters carefully

---

### Pitfall 3: Over-complicating

**Symptom:** Trying to show too much detail

**Fix:** Wireframes are low-fidelity—focus on structure, not pixels

---

### Pitfall 4: Missing Key Elements

**Symptom:** Forgetting headers, footers, or navigation

**Fix:** Always include the basic page shell first

---

### Pitfall 5: No Legend

**Symptom:** Using custom symbols without explanation

**Fix:** Include a legend or key for non-obvious symbols

---

## Quick Reference

### Essential Symbols

| Symbol | Meaning |
|--------|---------|
| `┌─┐│└┘` | Box borders |
| `──` or `==` | Horizontal lines |
| `│` | Vertical dividers |
| `[ ]` | Input fields, buttons |
| `[▼]` | Dropdowns |
| `[x]` | Checked state |
| `(x)` | Selected radio |
| `[IMG]` | Image placeholder |
| `→` | Navigation/flow |
| `///` | Loading |

### Standard Dimensions (character count)

| Container | Width | Notes |
|-----------|-------|-------|
| Full width | 60-80 chars | Standard terminal width |
| Card | 20-30 chars | Comfortable reading |
| Input field | 20-40 chars | Based on content |
| Button | 8-15 chars | Label + padding |

---

## References

### External Resources
- Wireframing.org — Industry best practices
- UX Booth, "The Art of Wireframing"
- Smashing Magazine, "Wireframe Best Practices"

### Provenance
- Adapted from UX design documentation standards
- Standardized ASCII conventions

