# Wireframe Template

---

## Pre-Creation Checklist (MUST ASK FIRST)

Before generating any wireframe, ALWAYS confirm with the user:

```
Platform:
□ Web (Desktop) - Full sidebar + header
□ Web (Tablet) - Collapsible sidebar, 2-col max
□ Mobile (iOS/Android) - Single column, hamburger/bottom nav
□ Desktop App - Native window chrome possible

Scope:
□ Single page only
□ Page + Modal
□ Page + Drawer
□ Page + Modal + Drawer (multi-step flow)

User Goal:
□ View / Browse
□ Edit / Modify
□ Create / Add
□ Search / Filter
```

> **IMPORTANT:** If the user hasn't specified platform, ASK before proceeding. Do NOT assume.

---

## Standard Templates

### 1. Single Page

```
═══════════════════════════════════════════════════
SCREEN: [Screen Name]
PLATFORM: [Web/Mobile/Desktop]
PURPOSE: [What user accomplishes here]
═══════════════════════════════════════════════════

┌─────────────────────────────────────────────────┐
│ [Header: Logo] [Nav Links]     [Search] [User] │
├──────────┬──────────────────────────────────────┤
│ Sidebar  │  Main Content                        │
│          │                                      │
│ • Item 1 │  ┌────────────────────────────┐      │
│ • Item 2 │  │ Section Title              │      │
│ • Item 3 │  ├────────────────────────────┤      │
│          │  │ Content here               │      │
│          │  │                            │      │
│          │  └────────────────────────────┘      │
│          │                                      │
│          │  [ ● Details ] [ History ] [ Files ]│
│          │  ─────────────────────────────────── │
│          │  Tab content...                     │
│          │                                      │
├──────────┴──────────────────────────────────────┤
│ [Footer: Pagination]                            │
└─────────────────────────────────────────────────┘
```

### 2. Page + Modal

```
═══════════════════════════════════════════════════
SCREEN: [Page Name] + [Modal Name]
PLATFORM: [Web/Mobile/Desktop]
═══════════════════════════════════════════════════

┌─────────────────────────────────────────────────┐
│ PAGE: [Page Name]                               │
│ [Header]                        [Search] [User] │
├──────────┴──────────────────────────────────────┤
│                                                  │
│  Content with trigger:                          │
│  [Button that opens modal]                      │
│                                                  │
│  ...more content...                             │
│                                                  │
└─────────────────────────────────────────────────┘


┌─────────────────────────────────────────────────┐
│ MODAL: [Modal Name]                     [X]     │
├─────────────────────────────────────────────────┤
│                                                 │
│  Modal content here...                          │
│                                                 │
│  ┌─────────────────────────────────────────┐   │
│  │ [Form fields / Info / Actions]          │   │
│  └─────────────────────────────────────────┘   │
│                                                 │
│              [Cancel]  [Confirm]                │
└─────────────────────────────────────────────────┘
```

### 3. Page + Drawer

```
═══════════════════════════════════════════════════
SCREEN: [Page Name] + [Drawer Name]
PLATFORM: [Web]
═══════════════════════════════════════════════════

┌─────────────────────────────────────────────────┐
│ PAGE: [Page Name]                    [User] [🔔]│
├────────────────────┬────────────────────────────┤
│ Sidebar            │  Main Content              │
│                    │                            │
│                    │  [Filter] triggers drawer  │
│                    │                            │
└────────────────────┴────────────────────────────┘

┌─────────────────────────────────────────────────┐─────────────────────────┐
│                                                 │ DRAWER: Filter   [X]    │
│                                                 ├─────────────────────────┤
│                                                 │ Category                │
│                                                 │ [ ] All                 │
│                                                 │ [ ] AI                  │
│                                                 │                         │
│                                                 │ Status                  │
│                                                 │ ( ) Any                 │
│                                                 │ (•) Active              │
│                                                 ├─────────────────────────┤
│                                                 │      [Clear]  [Apply]   │
└─────────────────────────────────────────────────┴─────────────────────────┘
```

### 4. Page + Modal + Drawer (Multi-Step Flow)

Show containers sequentially - no arrows needed, names indicate entry points:

```
═══════════════════════════════════════════════════
SCREEN: [Flow Name]
PLATFORM: [Web]
═══════════════════════════════════════════════════

┌─────────────────────────────────────────────────┐
│ PAGE: [Page Name]                               │
├──────────┴──────────────────────────────────────┤
│                                                  │
│  [List of items]                                │
│  ┌────────┐ ┌────────┐ ┌────────┐              │
│  │ Item A │ │ Item B │ │ Item C │              │
│  │ [Edit] │ │ [Edit] │ │ [Edit] │              │
│  └────────┘ └────────┘ └────────┘              │
│                                                  │
└─────────────────────────────────────────────────┘


┌─────────────────────────────────────────────────┐
│ MODAL: Confirm Action                   [X]    │
├─────────────────────────────────────────────────┤
│                                                 │
│  "Are you sure you want to...?"                │
│                                                 │
│              [Cancel]  [Confirm]                │
└─────────────────────────────────────────────────┘


┌─────────────────────────────────────────────────┐
│ PAGE: [Page Name] (Updated State)               │
├──────────┴──────────────────────────────────────┤
│                                                  │
│  [List shows updated state]                     │
│  ┌────────┐ ┌────────┐ ┌────────┐              │
│  │ Item A │ │ Item B*│ │ Item C │              │
│  │ [Edit] │ │ [Edit] │ │ [Edit] │              │
│  └────────┘ └────────┘ └────────┘              │
│                       * = updated item          │
└─────────────────────────────────────────────────┘


┌───────────────────────────────────────┬─────────┐
│                                       │ DRAWER: │
│                                       │  Edit   │
│                                       │   [X]   │
│                                       ├─────────┤
│                                       │ Name    │
│                                       │ [_____] │
│                                       │         │
│                                       │ [Cancel]│
│                                       │ [Save]  │
└───────────────────────────────────────┴─────────┘
```

---

## Template Guidelines

| Rule | Example |
|------|---------|
| **Use `●` for selected/active** | `[ ● Details ] [ History ]` |
| **Show triggered containers separately** | Modal/Drawer as separate boxes, not nested |
| **No flow arrows needed** | Container names indicate entry point |
| **Keep containers independent** | Modal doesn't need underlying page border |

---

## Notes

- Before using this template, confirm platform with user
- Template assumes Web desktop by default - adjust for mobile
- For mobile, use single column layout with hamburger menu