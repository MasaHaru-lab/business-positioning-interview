# 商业定位深度访谈

**Business Positioning Interview — A Claude Skill for Finding Your Real Position**

> 一个**和 AI 一起做的、60-150 分钟的深度自我盘点**——
> 帮你找到那个**别人替代不了你**的商业位置。

> 不是问卷，不是 checklist，不是"3 个步骤找到你的 niche"。
> 是一次有温度、有挑战、有"被看见"瞬间的真实对话。

---

[English summary →](#english)

---

## 这是什么

一份**给 AI 的剧本**。

把它喂给 Claude / ChatGPT / Gemini / 任何能读 markdown 的大模型，它就会扮演一个**有 10 年经验的商业教练**，用 60-150 分钟跟你走完：

```
   热爱（你愿意持续投入）
 × 擅长（你天然比别人做得好）
 × 资源（你已积累的杠杆）
 × 市场（有人愿意为之付费）
 ─────────────────────────
 = 你的定位
```

但**真正的价值不在于走完四个圈**——四个圈你自己写问卷也能填。**价值在维度之间的连接、矛盾、和盲区**。这是 skill 真正在做的事。

访谈结束后，你会得到：

- 一句**用你自己的原话**搭起来的核心定位句
- 一个画得出来的**目标客户画像**（一个具体的人，不是一类人）
- **5 个差异化标签**（5 秒内能记住）
- **产品体系初版**（引流品 / 利润品 / 后端品，含定价区间）
- **5 个关键洞察**——访谈中浮现的、你自己看不见的发现
- **盲区与风险清单**——坦白告知你还没想透的事
- **30 天 / 90 天行动计划**，包括"**不做什么**"
- 一份**你自己原话的素材库**——以后写文案、做内容直接引用

[**看一份样本输出 →**](./examples/sample-output-skeleton.md)

---

## 为什么我做了这个

市面上的"找定位"内容多数是**营销课**——告诉你怎么"包装"自己。

这个 skill 反过来——**它假设你身上已经有那个位置，只是你自己看不清**。

它的任务是：**用提问把它问出来，再用你自己的原话搭成定位句**。

> **定位的核心从来不是"找到一个赛道"，是"被一双足够认真的眼睛看见你已经是的样子"。**

设计哲学：

- **温暖但不讨好**——不会有"哇好棒"。会反映、会指出矛盾、会温和地挑战
- **提问 > 给答案**——90% 是问，10% 是反映和综合
- **用你的原话**——不替你"翻译"成商业书面语。原话才有体温
- **看到矛盾就指出**——不让你的诠释偷偷取代你的真实
- **不灌输理论**——IKIGAI、定位理论、黄金圈是 skill 的内功，不是台词

---

## Quick Start — 三种启动方式

### A. 用 Claude Code（最完整）

```bash
# 把整个文件夹放到你的 Claude Code skills 目录
git clone https://github.com/MasaHaru-lab/business-positioning-interview.git ~/.claude/skills/business-positioning-interview
```

然后在 Claude Code 里说：

> 帮我做商业定位访谈

或：

> Run the business-positioning-interview skill

skill 会自动加载，开始访谈。

### B. 用 ChatGPT / Claude.ai / Gemini / DeepSeek / 其他大模型

任何能读长文本的 AI 都行。**5 步**：

1. 复制 [`SKILL.md`](./SKILL.md) 全文
2. 打开 ChatGPT / Claude.ai / Gemini 网页版
3. 把 SKILL.md 整段粘贴到对话开头
4. 加一句："请按照上面的方法论给我做商业定位访谈，从开场词开始"
5. 跟着 AI 走 60-150 分钟

访谈结束时，AI 会按 [`references/output-template.md`](./references/output-template.md) 的结构生成你的定位文档。把那个模板也喂给 AI 就好。

> 💡 **小贴士**：选最聪明的模型（Claude Sonnet 4.5+ / GPT-5+ / Gemini 2.5 Pro+）效果最好。便宜的模型会跳过特殊时刻处理。

### C. 不用 AI（两人配对版）

两个朋友坐下来——

- 一个当**提问者**（拿着 SKILL.md，按流程问）
- 一个当**受访者**（答）
- 90-150 分钟后，**一起**整理输出文档

效果可达 AI 版的 70-85%。优势是真实的情绪共振，劣势是没法实时维护"信号笔记"和反模式识别。

**适合**：朋友间互助、读书会、工作坊、coaching pair-up。

---

## 这个 skill 适合谁

✅ **适合**：

- 自由职业者 / 独立创业者
- 知识博主 / 自媒体作者
- 咨询师 / 教练 / 培训师
- 副业探索者 / 想从打工转向自雇的人
- 中年身份转型者
- 任何**有内容、想被看见、但没找到那个具体位置**的人

❌ **不适合**：

- 已经有清晰定位、只是想要执行建议的人（去找营销课）
- 完全没有任何积累、想"无中生有"找定位的人（先做事，再找定位）
- 不愿意花 60+ 分钟认真自我盘点的人（这个 skill 不替你想）

---

## 仓库结构

```
business-positioning-interview/
├── SKILL.md                          ← 主访谈剧本（核心）
├── README.md                         ← 你正在读的这个
├── CHANGELOG.md                      ← 版本演变记录
├── LICENSE                           ← MIT
├── examples/
│   └── sample-output-skeleton.md    ← 一份虚构样本输出
└── references/
    └── output-template.md            ← 最终定位文档的模板
```

---

## 这个 skill 是怎么演变的

v1 是按"自我梳理表"的四维度框架写的——4 个维度 × 6 个启发式问题 + 6 个交叉问题 + 综合定位。

**v2 是迭代之后的版本**，把 v1 在实操中暴露出的几类"骨架之外的隐藏知识"显性化了——

> v1 的"问题列表"是骨架，但**真正决定访谈成败的，是骨架之外的"特殊时刻处理"**：
>
> - 当受访者情绪化（泪目 / 上头）那一刻，怎么接住？
> - 当受访者画出 boundary（不想展开的过去 / 经历），怎么尊重又仍提取价值？
> - 当受访者用 AI 转引代替回答（"chat 说我是 X"），怎么不羞辱地穿透？
> - 当受访者外部认证证据浮现（行业内人误判他为同行），怎么立刻锁定？

v2 把这些显性化了。详细演变见 [CHANGELOG.md](./CHANGELOG.md)。

---

## 设计原则

1. **用对方的原话做脚手架**——不替用户"翻译"成商业书面语
2. **看见连接、矛盾、盲区**——单独的问题用户自己也能写问卷，价值在维度之间
3. **温暖但不讨好**——不要"哇好棒"
4. **不灌输理论**——IKIGAI / 定位理论 / 黄金圈是访谈者的内功，不是台词
5. **响应长度有节制**——中段反映 1-3 句 + 1 个问题；长综合只在阶段过渡时出现
6. **画一个人，不画一类人**——目标客户必须能"画出一个具体人"，群体描述不接受
7. **承认不确定**——v1 文档是初稿，鼓励 7 天后回看 / 3 个月后修订 v2

---

## 关于作者

我是 **FelicityFish**——

重度 AI 学习和使用者，古典音乐爱好者。这次参考**诗奥老师**的课程，做了这个 skill，可以通过 1-2 小时的访谈，找到自己的真实定位。

欢迎大家使用，有反馈也可以发给我。

---

## 跟我连接

- 公众号：**鱼头烤玉米**
- Email: [ambrosiaz@gmail.com](mailto:ambrosiaz@gmail.com)
- GitHub: [@MasaHaru-lab](https://github.com/MasaHaru-lab)

> **想给反馈、想分享你的访谈体验、想跟我聊聊你跑出来的定位——都欢迎来邮件。**
> 我读每一封，但不一定回每一封。同步信件式陪伴是这个 skill 设计的产品形态之一——
> 我自己也用同样的节奏。

---

## License

MIT — 详见 [LICENSE](./LICENSE)

简单说：

- ✅ 自由使用、修改、再分发、商业化
- ✅ 改了之后开源 OR 闭源都可以
- ⚠️ 必须保留版权声明（基于 MasaHaru-lab's work）
- ❌ 我不为任何后果负责

---

## 致谢

- **第一次跑这个 skill 的真实用户**——你的"看见"那一刻让我重写了整个 v2
- **Anthropic Claude 团队**——把访谈型 AI 协作变成可能
- **所有相信"定位不是被设计出来的，是被看见出来的"的人**
- **诗奥老师的深度分享**

---

<a name="english"></a>

## English Summary

This is a **Claude / ChatGPT / Gemini-compatible skill** for **deep business positioning interviews**.

Feed `SKILL.md` to any capable LLM and it will conduct a 60-150 minute structured interview that walks you through four dimensions:
- What you love
- What you're good at
- What resources you have
- What the market needs

But the real value isn't covering each dimension — it's surfacing the **connections, contradictions, and blind spots between them**.

You'll end up with:
- A core positioning sentence built from your own words
- A specific customer avatar (one person, not a category)
- 5 differentiation tags
- A product system v1 (lead magnet / core product / high-end backend with pricing)
- 5 key insights surfaced during the interview
- A blind spot & risk inventory
- 30/90-day action plan including "what NOT to do"
- A library of your own quotable phrases

**Designed in Chinese** but the methodology is universal — translation to English is straightforward.

License: MIT.

Author: **FelicityFish** · GitHub: [@MasaHaru-lab](https://github.com/MasaHaru-lab)

---

> **"定位不是你给他的，是从他嘴里掏出来的。**
> **你只是那个负责掏的人。"**
>
> *— from SKILL.md*
