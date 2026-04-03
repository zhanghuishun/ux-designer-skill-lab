# UX Designer Skill Lab

面向 **体验设计师** 的 Agent **Skill Kit**：把可重复的设计与研究流程写成结构化技能，方便在 Cursor、Claude Code 等环境里由 AI 按同一套方法执行与交付。

## 这套 Kit 解决什么

与 AI 协作时常见的三件事：**回答缺少关键步骤**、**结论飘在对话里**、**各环节方法接不上**。每个 Skill = **固定流程 + 可改模板**，目录按需选用。

- **漏步骤** → Skill流程里钉住该问什么、该产出什么（如竞品维度、测试类型）。
- **对不齐** → 简报、旅程等有纸面载体，方便评审与交接。
- **按需用** → 一个目录一个 Skill，不必一次装全库。

## 当前技能一览

### 1. 需求分析

澄清业务目标、问题边界与可检验假设，为设计与研发对齐提供输入。

| 技能 | 来源 | 说明 |
|------|------|------|
| [`design-brief/`](design-brief/) | 原创 | 非结构化 PM 输入 → 结构化设计简报 |
| [`jobs-to-be-done/`](jobs-to-be-done/) | [PM-Skills] | JTBD：功能 / 社交 / 情感「工作」、痛点与收益，结构化澄清动机 |
| [`lean-ux-canvas/`](lean-ux-canvas/) | [PM-Skills] | Lean UX Canvas（v2）：业务问题、关键假设与下一跳学习 |

### 2. 设计调研

竞品与市场、假设性用户轮廓、用户旅程与故事地图等，支撑方案方向与优先级。

| 技能 | 来源 | 说明 |
|------|------|------|
| [`competitive-analysis/`](competitive-analysis/) | 原创 | UX 向竞品体验分析流程与报告骨架 |
| [`proto-persona/`](proto-persona/) | [PM-Skills] | 验证前的「原型画像」：综合现有线索与假设的可操作用户轮廓 |
| [`customer-journey-map/`](customer-journey-map/) | [PM-Skills] | 按阶段 / 触点 / 行为 / 情绪 / 指标等输出完整客户旅程图 |
| [`customer-journey-mapping-workshop/`](customer-journey-mapping-workshop/) | [PM-Skills] | 递进问题引导旅程图工作坊（人物、场景、阶段、痛点与机会） |
| [`user-story-mapping/`](user-story-mapping/) | [PM-Skills] | 用户故事地图：活动 → 步骤 → 任务与发布切片，串联旅程与 backlog |

### 3. 设计执行

信息架构与对象建模、低保真表达、叙事与交付物，支撑从概念到可开发描述。

| 技能 | 来源 | 说明 |
|------|------|------|
| [`OOUX/`](OOUX/) | 原创 | OOUX / ORCA：对象、关系、操作、属性 |
| [`ascii-prototype/`](ascii-prototype/) | 原创 | ASCII 线框快速表达版式与结构 |
| [`storyboard/`](storyboard/) | [PM-Skills] | 六格故事板：从问题到方案的叙事弧线，便于评审与共识 |
| [`user-story/`](user-story/) | [PM-Skills] | 用户故事 + Gherkin 验收标准，便于与研发对齐 |

### 4. 设计检查

对已有方案或版本做可用性层面的验证与问题归纳，支撑迭代决策。

| 技能 | 来源 | 说明 |
|------|------|------|
| [`usability-test/`](usability-test/) | 原创 | 可用性测试类型判断、执行与结果分析 |

**来源**列：`原创` 为本仓库编写；`[PM-Skills]` 表示自 [deanpeters/Product-Manager-Skills](https://github.com/deanpeters/Product-Manager-Skills) 同步拷贝（类型见各技能 frontmatter 的 `type`）。
> 自 [Product-Manager-Skills](https://github.com/deanpeters/Product-Manager-Skills) 拷贝的技能，著作权以原仓库 [LICENSE](https://github.com/deanpeters/Product-Manager-Skills/blob/main/LICENSE) 为准；本 README 仅作索引与使用场景说明。

## 未来可能扩展的技能

以下方向可按优先级逐步补齐：

- 启发式评估 / UX 走查（Heuristic evaluation）
- 设计评审 facilitation 与纪要结构
- 无障碍（WCAG）自查清单与缺陷分级
- 设计系统：token 与组件提取（contribution 流程）
- 利益相关方访谈 / 设计工作坊议程模板

## 新增技能时：如何生成与校验

本仓库 **不自带** skill 脚手架；**建议直接采用** [deanpeters/Product-Manager-Skills](https://github.com/deanpeters/Product-Manager-Skills) 仓库中的技能工程化工具与约定，与本 Kit 的技能形态保持一致，便于后续打包与索引。
