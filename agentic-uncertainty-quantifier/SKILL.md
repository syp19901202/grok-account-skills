---
name: agentic-uncertainty-quantifier
description: >
  给任务的不确定性打分（认知不确定 + 步骤不确定），用来校准想多深、
  要补多少上下文、要不要迭代。高风险决策、事实稀疏、目标含糊、交易或
  财务选择、不可逆动作，或自信显得过头时，务必考虑本技能。
  即使用户没说 uncertainty、不确定、有多大把握，也要用。
  只有琐碎或纯事实查询可以跳过。
version: 1.2.0
author: Stijnman + adapted
license: MIT
metadata:
  grok:
    tags: [量化不确定性, quantify uncertainty, 有多大把握, 决策, 风险]
    related_skills: [self-refine-loop, first-principles, research-assistant]
compatibility: Grok agent; optional MCP and shell access
---

# 智能体不确定性量化器

## 何时使用

- 高风险或不可逆决策（交易、资金、健康相关、上线）
- 事实稀疏、互相打架，或变化很快
- 目标含糊，或验收标准不清楚
- 用户问把握 / 风险 / 「有多确定」
- 第一性原理重建出了不显而易见的计划

## 流程

1. 给认知不确定性打 0–10 分（不知道的有多少）。
2. 给步骤不确定性打 0–10 分（步骤有多清楚）。
3. 认知不确定 > 6：再补上下文，跑 self-refine-loop。
4. 步骤不确定 < 4：先问清再动手。
5. 把分数和建议深度告诉用户。

## 可配合的技能

- `self-refine-loop`
- `semantic-memory-manager`
- `deep-search-enabler`

## 出错时怎么处理

| 失败 | 应对 |
|---------|----------|
| 虚假自信 | 破坏性任务上偏向谨慎。 |

## 注意

- 财务/上线动作的不确定性 > 7 时，触发人工确认（hitl-approver）。

## 示例

**输入：** 用户请求命中上面的触发条件。
**输出：** 按流程给出结构化结果，并按需调用配合技能。
