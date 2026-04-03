# UX Designer Skill Lab

面向 **UX / 体验设计师** 的 Agent **Skill Kit**：把可重复的设计与研究流程写成结构化技能，方便在 Cursor、Claude Code 等环境里由 AI 按同一套方法执行与交付。

## 这套 Kit 解决什么

- **统一方法**：从需求澄清到可用性验证，用固定章节（Purpose → Concepts → Application → Pitfalls → References）降低「随口一句 prompt」带来的漂移。
- **可对齐产研**：提供产出模板（可修改），与 PM 侧文档（如设计简报、竞品结论）口径一致，便于评审与 handoff。
- **可演进**：单技能独立成目录，按需增删，不需要的可以不装。

## 当前技能一览

| 技能 | 说明 |
|------|------|
| [`design-brief/`](design-brief/) | 非结构化 PM 输入 → 结构化设计简报 |
| [`competitive-analysis/`](competitive-analysis/) | UX 向竞品体验分析流程与报告骨架 |
| [`usability-test/`](usability-test/) | 可用性测试类型判断、执行与结果分析 |
| [`OOUX/`](OOUX/) | OOUX / ORCA：对象、关系、操作、属性 |
| [`ascii-prototype/`](ascii-prototype/) | ASCII 线框快速表达版式与结构 |

在对应目录中打开 `SKILL.md` 即可查看完整说明与模板。

## 未来可能扩展的技能（示意）

以下方向可按优先级逐步补齐：

- 启发式评估 / UX 走查（Heuristic evaluation）
- 设计评审 facilitation 与纪要结构
- 无障碍（WCAG）自查清单与缺陷分级
- 用户旅程图 / 服务蓝图 workshop
- 设计系统：token 与组件提取（contribution 流程）
- 利益相关方访谈 / 设计工作坊议程模板

## 新增技能时：如何生成与校验

本仓库 **不自带** skill 脚手架；**建议直接采用** [deanpeters/Product-Manager-Skills](https://github.com/deanpeters/Product-Manager-Skills) 仓库中的技能工程化工具与约定，与本 Kit 的技能形态保持一致，便于后续打包与索引。
