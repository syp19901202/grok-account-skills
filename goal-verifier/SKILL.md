---
name: goal-verifier
description: >
  在宣称做完之前，对照说清的或推断出的目标核对任务是否完成。
  多步任务、代码改动、研究交付、策略更新结束时，或用户要求确认 /
  核对 / 「做完了吗」时，务必做一次轻量检查。
  即使没说 verify，只要对话里有清楚的原始目标，也要用。
version: 1.2.0
author: Stijnman + adapted
license: MIT
compatibility: Grok agent; optional MCP and shell access
metadata:
  grok:
    tags: [核对目标, 确认完成, 做完了吗, verify goal, 验收]
    related_skills: [self-refine-loop, first-principles]
---

# 目标核对器

## 何时使用

- 任何有明确或隐含目标的多步任务结束时
- 改完代码/策略，或做完研究综合之后
- 用户要求确认、核对，或问「做完了吗 / 够不够」
- 把交付物标成完成之前

## 流程

1. 用一句话重述原始目标。
2. 列出验收标准（对话里说清的，或推断出来的）。
3. 逐条检查：通过 / 未过 / 部分过，并给出证据。
4. 有未过的，就调用 self-refine-loop，或把缺口报出来。
5. 只有关键标准都通过，才标成完成。

## 可配合的技能

- `self-refine-loop`
- `auto-tester`

## 出错时怎么处理

| 失败 | 应对 |
|---------|----------|
| 目标没定义 | 先请用户确认目标，再核对。 |
| 误报完成 | 必须有证据（文件路径、命令输出或测试结果）。 |

## 注意

- 核对是只读的；检查时不要改产物。

## 示例

**输入：** 用户请求命中上面的触发条件。
**输出：** 按流程给出结构化结果，并按需调用配合技能。
