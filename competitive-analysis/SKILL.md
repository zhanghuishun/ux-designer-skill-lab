---
name: competitive-analysis
description: Help UX designers run competitive analysis—from clarifying goals to delivering a valuable analysis report
intent: Provide a systematic UX competitive-analysis method and workflow to guide high-quality competitive experience reviews
type: Workflow
---

# UX Competitive Analysis

## Purpose
Help UX designers run competitive analysis systematically—from clarifying objectives to producing a useful report. This skill focuses on **competitive product experience analysis** so designers understand rivals’ experience strengths and gaps, informing product decisions and directions to learn from.

**When to use:**
- Early product decisions: understand the competitive landscape
- Design iterations: find directions for experience improvements
- After a competitor ships: assess experience pros and cons
- Ongoing monitoring: stay aware of market movement

---

## Key Concepts

### Four quadrants of competitor types

| Type | Definition | When to select |
|------|------------|----------------|
| **Direct competitor** | Closest rival; same market | Primary analysis target |
| **Indirect competitor** | Same category; partial audience overlap | Broaden perspective |
| **Substitute** | Different form; same user need | Surface latent threats |
| **Cross-industry reference** | Not competing; worth learning from | Spark innovation |

### Typical analysis goals

1. **Decision support** — whether to build, positioning, selling points, competitive strategy  
2. **Learning & reference** — user needs and design rationale (not copy-paste “answers”)  
3. **Gap analysis** — compare to a benchmark; close the gap  
4. **Market warning** — track competitors; macro / industry signals  

### Three-layer experience framework

Based on Jesse James Garrett’s *The Elements of User Experience*:

- **Strategic / useful layer** — what capabilities exist  
- **Behavioral / usable layer** — flow efficiency; clarity of information  
- **Reflective / desirable layer** — visual quality, appeal, delight  

---

## Application

### Six-step competitive analysis

```
Step 1: Clarify goals     → Why now? What help do we need?
Step 2: Pick competitors  → Who? What scope?
Step 3: Multi-lens view   → From which angles?
Step 4: Gather evidence   → From which sources?
Step 5: Analyze & compare → How to contrast and synthesize?
Step 6: Report & actions  → Conclusions and recommendations?
```

---

### Step 1: Clarify goals

**Core questions:**
- Why run this analysis now?
- What decision or action should it enable?
- What stage is the product in?
- What are the biggest problems and constraints?

**Output template:**

```
[Analysis goals]
- Product stage:
- Main problems & challenges:
- Goal type: □ Decision support □ Learning □ Gap / benchmark □ Market warning
```

---

### Step 2: Select competitors

**Selection principles:**

| Goal | Suggested competitor mix |
|------|----------------------------|
| Decision support / risk | Direct, category, substitutes |
| Learning | Direct, category, cross-industry references |

**Selection signals:**
- Market share; store / chart rankings  
- Company scale (flagship products)  
- User feedback (top issues in reviews / social)  
- Category pioneers  
- Relevant cross-industry references  

**Example selection (generic):**
> When designing note-taking for a phone maker’s system “Notes,” you might include:  
> - System notes: built-in notes from at least two major mobile/desktop ecosystems  
> - Third-party notes: two high-MAU cloud-sync note products  
> - Cross-industry: physical paper notebook  

---

### Step 3: Multi-lens analysis

**Recommended UX dimensions:**

| Layer | Lens | What to cover |
|-------|------|---------------|
| Capabilities | Feature comparison | What exists? Completeness? |
| Behavior | Interaction & flow | Path efficiency? Learning cost? |
| Reflective | Visual design | Beauty, brand feel, emotion |
| Foundation | Performance | Stability, smoothness, responsiveness |

**Feature comparison matrix example:**

| Feature | Our product | Competitor A | Competitor B |
|---------|-------------|--------------|--------------|
| Do-not-disturb for messaging | ✓ | ✓ | ✗ |
| Game boosting | ✓ | ✓ | ✓ |
| Screenshots | ✓ | ✓ | ✓ |
| Screen recording | ✓ | ✓ | ✗ |

---

### Step 4: Gather information

**Main channels:**

| Channel | Examples | Signal quality |
|---------|----------|----------------|
| **Hands-on** | Try the product; user research | ★★★★★ Primary |
| **Official / public** | Sites, press, interviews, docs | ★★★★☆ Official |
| **Third-party** | Analyst reports, conferences | ★★★☆☆ Industry |
| **Sentiment** | Store reviews, forums, social | ★★★★☆ User voice |

**Timing:**
- Too early: thin evidence, shaky conclusions  
- Too late: missed window  
- Often best: planning phase when rivals are live but feature set is stable  

---

### Step 5: Analyze and synthesize

**Common methods:**

1. **Comparative** — side-by-side differences  
2. **Positioning matrix** — two axes for positioning and differentiation  
3. **Version tracking** — history to see evolution  
4. **Feature breakdown** — L1 / L2 / L3 capability trees  
5. **Needs under features** — deeper jobs-to-be-done  
6. **SWOT** — strengths, weaknesses, opportunities, threats  
7. **PEST** — political, economic, social, technological context  

**Thinking pattern: facts → insight → action (e.g. “sky–rain–umbrella”)**

```
Fact     →  Dark clouds appear
Insight  →  It will rain
Action   →  Take an umbrella
```

---

### Step 6: Report

**Competitive canvas template (recommended):**

```
[1. Analysis goals]
- Product stage:
- Analysis goal:

[2. Competitors selected]
- Names & versions:
- Why chosen:
- Type: □ Direct □ Indirect □ Substitute □ Cross-industry reference

[3. Analysis dimensions]
- Angles: □ Features □ Visual □ Interaction □ Performance □ Other

[4. Evidence]
- Main sources:

[5. Strengths]
- Our advantages vs competitors:

[6. Weaknesses]
- Our gaps vs competitors:
- Competitor advantages:

[7. Opportunities]
- External upside:

[8. Threats]
- External risk:

[9. Recommendations & summary]
- Product recommendations:
- Competitive strategy:
- Core conclusions:
```

---

## Examples

### Example: Picture-in-picture / small-window gaming (System A vs System B)

**Context:** System A keeps evolving split-screen, sidebar, and floating-window links. Compare System B’s “global small window” on entry paths and window modes. Both are first-party game / multitasking enhancements on mass-market handhelds.

**Findings:**

| Dimension | System A strength | System A gap / System B strength |
|-----------|-------------------|--------------------------------|
| Trigger | Side quick panel can be opened proactively; often no need to interrupt foreground | - |
| Switching | Multitasking and window-mode entry relatively unified; clearer learning path | - |
| Small window | - | Shorter path between full screen and mini window; more flexible floating entry |
| Details | - | Finer window resize; clearer parallel state in recents |

**Opportunities:**
1. System B’s entry is deep; “favorite apps” row at top of recents is costly to use  
2. Mini-window scenarios still feel narrow  

**Recommendations:**
1. Improve visual hierarchy and immersion for windows  
2. Align notification / banner → floating window behavior  
3. Support usable floating-window layouts in landscape  

---

### Example: Photo community (two leading products + our official community)

**Goal:** Compare our official photo community with two mainstream photo-community products on IA and key journeys (“Competitor A” and “Competitor B” are anonymized).

**Findings:**

| Experience | Competitor A (general UGC) | Competitor B (photo vertical) | Our official community |
|------------|----------------------------|---------------------------------|------------------------|
| Feed | Two-column cards | Single-column immersive + two-column mix | Single-column, low immersion |
| Posting | Stepwise assist | Quick memo-style | Fragmented; high drop-off |
| Interaction motion | Double-tap heart, etc. | Badge / reward feedback | Weak motion |
| Sharing | Many formats | Poster / link / long image | Few ways to share |

**Opportunities:**
1. Stronger immersive home reading  
2. Smoother posting; lower friction  
3. More deliberate motion for interactions  
4. Unify feed card patterns  

---

## Common Pitfalls

### 1. Describing competitors ≠ analyzing them

❌ **Avoid:** Listing what features exist  
```
Competitor A has DND, game boost…
```

✅ **Do:** Matrices + what the diff means for us  
```
Compared to Us, Competitor A’s in-game small-window reply is more flexible,
with multiple ways to trigger a global small window. We can borrow floating
entry patterns while keeping our proactive sidebar trigger.
```

### 2. Features divorced from scenarios

Don’t analyze a control in isolation.**Do** place it in end-to-end flows and real contexts for target users.

### 3. Siloed roles

Typical issues: PM, ops, IXD, visual each ship a separate doc; no shared framework; misaligned conclusions.  
**Fix:** One owner coordinates; one shared structure.

### 4. Reports that die in design-only channels

**Fix:** Name the audience; turn insights into actionable design moves; refresh on a cadence.

### 5. Treating competitors as a checklist

❌ **Wrong:** “They have it, so we must.”  
✅ **Right:** Start from positioning—what we should do, can do, and how.

---

## References

### Related skills
- `ux-research-basics` — UX research basics  
- `design-evaluation` — Design evaluation methods  

### External frameworks
- Jesse James Garrett — *The Elements of User Experience*  
- IDEO method cards — Competitive product survey  
- Anthropological comparative approaches  
- Fact–insight–action structured thinking  
- Lean Canvas  
- SWOT / PEST  
- Porter’s Five Forces  
