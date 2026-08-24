# 马斯克 / 物理学第一性原理方法

任务新颖、昂贵，或类比答案黏住不放时再读这篇。日常工作用 `SKILL.md` 里的循环就够。

## 什么是第一性原理

亚里士多德：「认识一件事的最初依据」——在**这个问题里**，没法再有用地从更底层推出来的前提。

你不是在做粒子物理。你是在拒绝把*继承来的形式*当成*必然真理*。

马斯克（TED / 访谈）：

> I tend to approach things from a physics framework. Physics teaches
> you to reason from first principles rather than by analogy. … boil
> things down to the most fundamental truths and say, "What are we
> sure is true?" … and then reason up from there.

> 我倾向用物理学框架看问题。物理教你从第一性原理推理，而不是靠类比。
> ……把事情拆到最基本的事实，问「我们确定什么是真的？」……再从那里往上推。

> The normal way we conduct our lives is we reason by analogy. We are
> doing this because it is like something else that was done, or it is
> like what other people are doing.

> 日常生活里我们通常靠类比推理：因为以前有人这么做过，或别人都在这么做。

> Though most of our life we get through it by reasoning through
> analogy … otherwise mentally you wouldn't be able to get through the
> day. But when you want to do something new you have to apply the
> physics approach. Physics has really figured out how to discover new
> things that are counter-intuitive, like quantum mechanics.

> 大部分日子靠类比就能过完，否则脑子撑不住。但要做新东西，就必须用物理方法。
> 物理真正会发现反直觉的新事物，比如量子力学。

> The only rules are the ones dictated by the laws of physics.
> Everything else is a recommendation.

> 硬规则只有物理定律。其余都是建议。

他还配了两个习惯：

- **主动要负面反馈**，尤其是真会告诉你「你错了」的人。屋里没别人，就自己写反方。
- **日常用类比。** 第一性原理留给必须新、更便宜、更简单、或必须为真的那一段。

## 出处里的例子（数字要保留）

### 火箭 — SpaceX

类比框架：「轨道火箭要 5000–6500 万美元；火箭就是这个价。」

第一性原理问题：

1. 火箭*是什么做的*？航空铝合金、钛、铜、碳纤维。
2. 这些材料在大宗商品市场卖多少钱？
3. 马斯克引用的答案：材料大约只占典型火箭售价的 **2%**。

所以公理不是「火箭很贵」。公理是「这些材料按物理排好之后，现在扛着巨大的制造和不复用溢价」。重建后的动作：自己造、删零件、把贵的那些拿回来复用。

类比行业优化的是*形式*（一次性政府火箭）。第一性原理优化的是*功能*（把质量送上轨道）。

### 电池

类比框架：「电池每度电要 X，因为行业价就是 X。」

第一性原理：什么材料、什么比例、大宗商品价是多少？然后：哪些工序把剩下的成本加上去了？把贵的步骤删掉，或自己做。

## 算法（执行顺序 — 不许颠倒）

1. **先让需求不那么蠢** — 谁提的，为什么？质疑每一条需求，尤其是聪明人提的（包括你自己）。
2. **删除**部件或流程。如果后来加不回大约 10%，说明删得不够。
3. **简化**剩下的。最常见的错，是把本不该存在的东西打磨得很亮。
4. **加快**循环时间。
5. **最后才自动化**。把没用的步骤自动化，只是把坑挖得更快。

硬规则只有物理规律和用户的真实约束。
其余都是建议。

## 什么时候类比才是对的工具

类比不是罪。它是压缩。

可以类比的时候：

- 问题常规，继承来的形式又便宜又已知能用
- 你是故意对齐现有系统（这个应用的 token、这个引擎的惯例、用户已经说的品味）
- 你需要五秒答案，浪费 10% 也无所谓

该拒绝类比的时候：

- 形式很贵、很难看，或只是「大家都这么做」
- 你准备加一层 / 一个实体 / 一个设置页 / 一个引擎，「因为真应用都有」
- 用户要克隆，但功能其实比克隆小
- 某个数字（成本、延迟、步骤、字段）感觉是继承来的，不是量出来的

实用拆分：**用类比先动起来，对你准备留下的东西再用第一性原理。**

## 挖多深

James Clear 的操作规则：不必挖到原子。比常见描述再低一两层即可。

| 常见描述 | 低一层 | 低两层 |
| --- | --- | --- |
| 「我们需要仪表盘」 | 「得有人看到这 4 个数并行动」 | 「行动是：催那张逾期发票」 |
| 「克隆 Twitter」 | 「人发短公开笔记，并关注别人」 | 「这个用户想随手记想法，并看朋友的想法」 |
| 「加上登录」 | 「这些数据必须属于一个人」 | 「只有主人能读或写这些行」 |
| 「游戏需要教程」 | 「玩家第一次撞车前必须学会 A = 向左」 | 「前 10 秒就是教程」 |

再拆下去也不改变下一步时，就停。

## 把负面反馈当成一步

锁定非琐碎计划之前，花一轮填这些空：

- 「这个计划是错的，因为 ___。」
- 「我最没把握的公理是 ___。」
- 「如果我只是在抄熟悉的应用，破绽是 ___。」

填不出，就是还没看。填得出，就去核那条弱公理，或睁着眼往下做。
