# grok-account-skills

个人 Grok 账号技能合集：自动用第一性原理思考，并覆盖研究、代码、决策和**自主技能进化**。

## 包含的技能（本仓库本地副本）

- **first-principles** — 思考层（非琐碎工作默认先加载）
- **deep-reasoning** — 增强版第一性原理（第一性原理 + 逆向 + 系统 + 二阶 + 约束 + 事前验尸 + 机会成本/费米估算）
- **research-assistant** — 深度研究与综合
- **code-architect** — 代码 / 策略架构
- **agentic-uncertainty-quantifier** — 给决策打不确定性分数
- **goal-verifier** — 核对任务是否真的做完
- **self-refine-loop** — 反复批评并改进
- **skill-evolver**（精简版）— 基础技能改写
- **skill-creator**（精简版）— 创建与评测技能

## 完整自主进化（推荐）

若要真正的自我进化能力，请从上游安装完整版（含脚本和评测引擎）：

```bash
# FishSerrie skill-evolver（8 阶段循环 + 5 门禁 + GT）
bash /root/.grok/skills/skill-installer/scripts/install-skill.sh --repo FishSerrie/skill-evolver --path plugin/skills/skill-evolver --dest ~/.grok/skills --name skill-evolver

# Anthropic skill-creator（评测的硬依赖）
bash /root/.grok/skills/skill-installer/scripts/install-skill.sh --repo anthropics/skills --path skills/skill-creator --dest ~/.grok/skills --name skill-creator
```

也可以直接对 Grok Bot 说：

> 把 https://github.com/FishSerrie/skill-evolver 的 plugin/skills/skill-evolver 和 https://github.com/anthropics/skills 的 skills/skill-creator 装到我的账号技能

## 新 Bot 怎么一次装齐

对 Bot 说下面任一句话：

1. **推荐一句话**：
   > 把 https://github.com/syp19901202/grok-account-skills 里的技能全部装上，另外再从 FishSerrie/skill-evolver 和 anthropics/skills 安装完整的 skill-evolver 和 skill-creator

2. 或者分步：
   > 先安装 https://github.com/syp19901202/grok-account-skills 的所有技能
   > 再安装 FishSerrie 的 skill-evolver 和 Anthropic 的 skill-creator

## 目录结构

每个技能是一个文件夹，至少有 `SKILL.md`（可选再带 `references/` 和 `scripts/`）。
