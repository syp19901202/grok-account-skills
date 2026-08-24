---
name: self-refine-loop
description: >
  跑「生成—批评—改写」循环，迭代改进输出。质量要紧时用：
  复杂推理、代码/策略草稿、研究综合、高不确定性任务，或第一版
  答案显得不完整。非琐碎工作优先用本技能，而不是一遍交差。
  用户明确说 refine / critique / improve / 改进 / 再改一版 时也触发。
  最多 5 轮，或把握 ≥ 8/10 就停。
version: 1.2.0
author: Stijnman + adapted
license: MIT
compatibility: Grok agent; optional MCP and shell access
metadata:
  grok:
    tags: [自我改进, 批评并改写, 迭代, refine, 提高输出]
    related_skills: [goal-verifier, agentic-uncertainty-quantifier, first-principles]
---

# 自我改进循环

## 何时使用

- 复杂或高风险输出（策略代码、研究结论、决策）
- 初稿不完整、不一致，或把握很低
- 用户要求改进、批评、提高或再改一版
- 不确定性量化器标出高认知不确定之后

## 流程

1. 记下当前输出和用户的质量标准。
2. 生成批评，列出具体弱点（最多 5 条）。
3. 改写输出，每一条批评都要处理。
4. 按标准是否满足，给把握打 0–10 分。
5. 重复直到把握 ≥ 8 或满 5 轮；返回最好的一版，并附改动说明。

## 可配合的技能

- `goal-verifier`
- `agentic-uncertainty-quantifier`
- `dspy-prompt-optimizer`

## 出错时怎么处理

| 失败 | 应对 |
|---------|----------|
| 没给标准 | 先请用户给 1–3 条成功标准，再循环。 |
| 把握卡在 5 以下 | 提前停；报告卡点并请用户指引。 |
| 输出无限变长 | 改写篇幅上限为上一版 + 20%。 |

## 注意

- 琐碎错别字不要循环；改一遍就够。

## 示例

**输入：** 用户请求命中上面的触发条件。
**输出：** 按流程给出结构化结果，并按需调用配合技能。
