---
name: usability-test
description: Help UX designers prepare usability test plans and analyze results, first determining whether the test is exploratory or evaluative, then guiding test execution and issue analysis
intent: Provide an end-to-end usability testing workflow, from test type selection to results analysis
type: interactive
---

# Usability Test Planning and Results Analysis

## Purpose
Help UX designers systematically plan and run usability tests: first determine the test type (exploratory/evaluative), then complete test planning, test execution, and results analysis. Applicable to user experience evaluation during the product design process.

## Key Concepts

### Definition of usability
Usability is a measure of the quality of user experience when users interact with a product or system, and includes three core dimensions:
- **Effectiveness**: whether users can achieve their goals
- **Efficiency**: the resources required for users to complete tasks
- **Satisfaction**: the degree of user satisfaction with the interaction process

### Test types: Exploratory vs Evaluative
| Feature | Exploratory Test | Evaluative Test |
|--------|------------------|-----------------|
| Goal | Discover usability issues | Evaluate whether design solutions are effective |
| Timing | Early design, prototype stage | Late design, optimization stage |
| Sample size | 5–8 participants can uncover most issues | Comparable historical data or benchmarks |
| Output | Issue list, design recommendations | Quantitative metrics, solution comparison |
| Analysis method | Descriptive analysis | Summative testing (benchmark/comparative) |

> According to Nielsen’s formula, testing with 10 users can discover about 98% of usability problems.

### Core components of a usability test
1. **Goals**: test objectives
2. **Users**: target user profiles
3. **Tasks**: typical usage scenarios and tasks
4. **Evaluation metrics**: efficiency, error rate, satisfaction, etc.

## Application

### Step 1: Determine test type

**Please answer the following question:**

**Q1: What is the objective of your test?**
1. Discover existing usability problems in the product
2. Compare which of several design solutions performs better
3. Verify whether an optimized solution is effective
4. Evaluate the gap between the product and its competitors

### Step 2: Define research goals based on test type

According to your choice:

**If you chose 1 (discover problems) → Exploratory test**
- Goal: Identify current usability issues of the product
- Focus: Observe where users encounter difficulties or confusion
- Output: Issue list + priority + improvement suggestions

**If you chose 2/3/4 (evaluate/compare/verify) → Evaluative test**
- Goal: Use data to evaluate design solutions
- Focus: Compare quantitative metrics (completion rate, completion time, satisfaction)
- Output: Data report + solution recommendation

### Step 3: Define user sample

**Q2: What are the characteristics of the target users?**

Please describe:
- User profiles (job role/role type/experience level)
- Product usage experience (novice/intermediate/expert)
- Recruitment channels (internal/external)

**Sample size reference:**
- Exploratory test: 5–10 participants can uncover most problems
- Evaluative test: at least 5 participants per group for comparison

### Step 4: Design test tasks

**Q3: What tasks do users need to complete?**

Please list core tasks, for example:
- Task 1: Create a new Scrum project
- Task 2: Configure and complete host deployment
- Task 3: Create and run a new pipeline

**Task design guidelines:**
- Tasks must have a clear starting point and end point
- Tasks should include real user usage scenarios
- Define evaluation metrics (completion time, number of errors, satisfaction rating 1–10)

### Step 5: Run the test

**Observation focus:**
- Whether the user completes the task
- Whether there are invalid operations or moments of “not knowing what to do”
- Whether there are pages or moments the user is dissatisfied with

**What to record:**
- Behavior–actions
- Thoughts–steps
- Problems–what users say and do

### Step 6: Analyze results

**Data analysis dimensions:**

| Metric | Description | Calculation |
|--------|-------------|------------|
| Task completion rate | Proportion of users who successfully complete the task | Number of completers / total participants |
| Task error rate | Frequency of user operation errors | Number of errors / number of task attempts |
| Completion time | Time required for users to complete the task | Mean / median |
| Satisfaction | User satisfaction with the task | Rating from 1–10 |

**Severity rating of issues:**

- **Severe**: Occurs in critical business scenarios, directly impacts business success, prevents users from completing common tasks
- **Major**: Seriously interferes with task completion or increases user burden, significantly reduces user experience
- **Minor**: Superficial problem that does not prevent task completion but harms user experience

**Exploratory test output template:**
```
Issue ID | Issue description | Issue category | Severity | Number of users who encountered it | Improvement suggestion
---------|-------------------|----------------|----------|------------------------------------|------------------------
```

**Evaluative test comparison template:**
```
Metric | Option A | Option B | Conclusion
-------|----------|----------|----------
Task completion rate | 80% | 95% | Option B is better
Average completion time | 120s | 90s | Option B is more efficient
Satisfaction rating | 6.5 | 8.2 | Option B has higher satisfaction
```

## Examples

### Example 1: Exploratory test (discovering problems)

**Scenario:** First-party camera app usability test on widely used smartphone hardware

**Users:** 18–45 years old, balanced gender ratio, mix of typical smartphone owners (multiple device makers and OS generations represented)

**Example tasks:**
- Task 1: Switch to the front camera and take a selfie
- Task 2: Find the mirror switch and take a selfie
- Task 3: Take a photo with a filter applied

**Output:** Top issues discovered
- No swipe hint on the main camera interface
- Secondary menus collapse in a way that prevents mode switching
- Icon recognizability problems (color mode vs. “pro” color profile labeling)

### Example 2: Evaluative test (solution comparison)

**Scenario:** Usability comparison between two leading smart-home companion apps (anonymous: App A vs App B)

**Comparison dimensions:**
- Effectiveness: task completion quality
- Efficiency: completion time
- Satisfaction: users’ subjective ratings

**Result:** For the task “add a device to a specific room,” App A had higher task success; App B was slightly faster for expert users who already knew the layout.

### Example 3: Longitudinal evaluative test (version comparison)

**Scenario:** Satisfaction comparison between two consecutive major releases of the same productivity suite (v3.x → v4.x)

**Data:**
- Overall satisfaction: 7.88 → 8.25
- Experience keywords: more concise, younger, more innovative

## Common Pitfalls

### 1. Testing at the wrong time
- **Problem:** Running evaluative tests too early in design, or doing exploratory tests too late
- **Consequence:** Either you cannot get valuable findings, or you waste completed development work
- **Suggestion:** Choose test type according to the product stage

### 2. Unrepresentative sample
- **Problem:** Only testing with internal users or a narrow user group
- **Consequence:** Findings do not represent real users
- **Suggestion:** Configure the sample according to target user profiles

### 3. Tasks not reflecting real usage
- **Problem:** Tasks are not typical user scenarios
- **Consequence:** Test results cannot reflect real problems
- **Suggestion:** Use user research to identify real task scenarios

### 4. Focusing only on quantitative data
- **Problem:** Only paying attention to completion rate/time and ignoring user behavior and feedback
- **Consequence:** Missing important experience insights
- **Suggestion:** Combine quantitative (metrics) and qualitative (interviews/observation) analysis

### 5. Poor issue categorization
- **Problem:** Mixing all issues together without classifying by severity
- **Consequence:** Unable to determine improvement priority
- **Suggestion:** Classify issues into three levels: severe/major/minor

## References

### Related skills
- `discovery-interview-prep` — Interview preparation skill
- `user-story` — User story writing

### External resources
- Nielsen Norman Group: https://www.nngroup.com/
- ISO 9241-11 (Usability standard)