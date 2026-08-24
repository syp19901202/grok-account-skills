---
name: skill-evolver
description: "自动技能进化引擎：skill-creator（评测）+ AutoResearch（迭代）+ 多门禁 + 记忆。模式：evolve/eval/create/benchmark/improve。自然语言要求优化、改进、调参、评测、对比或新建技能时触发。英文：'/skill-evolver', '/evolve', 'optimize this skill', 'improve this skill'。中文：'优化这个 skill', '优化 skill', '帮我优化', '帮我调一下 skill', '用 skill-evolver 优化', '让这个 skill 变强', '改进 skill', '创建 skill', '新建 skill', '自动优化', 'skill 评测'。"
---

# 技能进化器（FishSerrie 自主版）

这是**完整的自主技能进化引擎**。

完整脚本、参考资料、代理和评测工具，请从上游安装：

```bash
bash /root/.grok/skills/skill-installer/scripts/install-skill.sh --repo FishSerrie/skill-evolver --path plugin/skills/skill-evolver --dest ~/.grok/skills --name skill-evolver
```

或者对 Bot 说：

> 从 FishSerrie/skill-evolver 安装 plugin/skills/skill-evolver 到我的技能目录

硬依赖：还要从 anthropics/skills 安装 skill-creator。

一键安装说明见仓库主 README。
