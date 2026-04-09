# Midas Skill

> **Turn Your Repeated Orders Into Gold.**
> **把你的重复指令变成黄金。**

A self-learning wealth extraction engine for OpenClaw / Claude Code.
An OpenClaw Skill by [@realteamprinz](https://github.com/realteamprinz).

---

## English

### The Core Insight

You leak wealth signals every single day without noticing.

- The small talk with coworkers ("man, shipping costs are insane right now")
- The photos you snap absent-mindedly (a construction site, a packed restaurant, an empty storefront)
- The videos you binge-watch at 2am (repair tutorials, product reviews, industry rants)
- The group chats you scroll through ("anyone know a good accountant?", "this app is broken again")
- The complaints you repeat ("why is this so expensive", "nobody does this well", "I wish someone would just...")
- The purchases you make on autopilot (the same protein powder, the same SaaS subscription, the same takeout order)

**This is raw ore. Midas turns it into gold.**

The fundamental insight: wealth is not hidden in Bloomberg terminals or VC pitch decks. Wealth is hiding in the noise of your daily life. The problem isn't access to information — it's that you've been trained to ignore the signals you encounter every single day.

**Midas doesn't just analyze billionaires. Midas analyzes YOU.**

### Nuwa vs. Midas

| | Nuwa | Midas |
|---|---|---|
| **What it distills** | How people *think* | How to turn your noise into *money* |
| **Input** | Biographies, interviews, ideas | Slack, photos, chats, complaints, receipts |
| **Output** | Mental models | Ranked opportunities + next actions |
| **Learns over time** | Yes | Yes (cross-references every input) |

Nuwa is a thinking tool. Midas is a wealth extraction tool. They compose.

### Quick Start

```bash
# 1. Clone the repo
git clone git@github.com:realteamprinz/midas-skill.git

# 2. Install as a Claude Code / OpenClaw skill
cp -r midas-skill ~/.claude/skills/

# 3. Activate in any conversation by saying one of the trigger phrases:
#    "Midas, mine this"
#    "Turn this into gold"
#    "What money signal is here"
#    "点石成金"

# 4. Feed your first input — anything goes:
#    - A week of Slack messages
#    - Screenshots of group chats
#    - A list of your last 20 purchases
#    - 30 phone photos from one week
#    - Your YouTube history
```

### The 6-Lens Extraction Engine

Every input runs through six lenses:

1. **Money Signal Detection** — Where is money moving, stuck, or leaking?
2. **Demand Gap Identification** — What do people want that nobody provides?
3. **Arbitrage Window Detection** — Where is value being mispriced?
4. **Skill-to-Revenue Bridge** — What do you already know that has market value?
5. **Network Monetization Path** — Who should be talking to whom, and what's the finder's fee?
6. **Behavioral Leverage Point** — What autopilot habit is one pivot away from revenue?

See `references/signal-extraction-framework.md` for the full methodology.

### Example Walkthroughs

| Example | What it shows |
|---|---|
| [`examples/daily-slack-mining/`](examples/daily-slack-mining/) | **Flagship** — extracting 4+ money signals from one week of mundane Slack noise |
| [`examples/photo-roll-mining/`](examples/photo-roll-mining/) | Turning 30 casual phone photos into a neighborhood arbitrage thesis |
| [`examples/complaint-mining/`](examples/complaint-mining/) | Turning 2 weeks of group chat complaints into a business concept |
| [`examples/browsing-mining/`](examples/browsing-mining/) | Using YouTube + browsing history to find your latent skill-to-revenue bridge |
| [`examples/billionaire-pattern-match/`](examples/billionaire-pattern-match/) | Matching your extracted signals against Musk / Buffett / Thiel playbooks |

### How Midas Gets Smarter Over Time

Midas is **cumulative**. Every input enriches everything else.

- **Day 1:** You feed it your Slack. It flags a potential signal at 35% confidence.
- **Day 3:** You feed it photos from the same week. A photo corroborates the Slack signal. Confidence → 58%.
- **Day 7:** You feed it your browsing history. You've been researching the exact domain for 6 months without noticing. Confidence → 82%. **GOLDEN OPPORTUNITY flag.**
- **Day 30:** Midas knows your opportunity landscape better than you do.

All confidence changes are logged to `evolution/evolution.jsonl`.

### The Pattern Matcher

Midas maintains pre-built **wealth operating systems** for famous figures (Musk, Buffett, Thiel). These are NOT for worship — they're reference frames for pattern matching.

When your signals accumulate, Midas automatically checks:

> "Your pattern looks like early-stage Thiel: monopoly in a niche nobody takes seriously. Thiel's playbook says: dominate the small market first."

This is the bridge between analyzing billionaires and analyzing yourself.

### Project Structure

```
midas-skill/
├── SKILL.md                              # Main entry — Midas core instructions
├── README.md                             # This file
├── LICENSE                               # MIT
├── references/
│   ├── signal-extraction-framework.md    # 6-lens methodology
│   ├── noise-to-gold-pipeline.md         # 7-stage extraction pipeline
│   ├── deal-template.md                  # Deal analyzer template
│   ├── sources-guide.md                  # Input source hierarchy
│   └── famous-models/
│       ├── README.md
│       ├── elon-musk.md
│       ├── warren-buffett.md
│       └── peter-thiel.md
├── examples/
│   ├── daily-slack-mining/
│   ├── photo-roll-mining/
│   ├── complaint-mining/
│   ├── browsing-mining/
│   └── billionaire-pattern-match/
└── evolution/
    └── evolution.jsonl                   # Your personal cumulative intelligence log
```

### How to Contribute

Pull requests welcome. Two kinds of contributions are especially valuable:

1. **New famous-person wealth OS files** — add profiles for figures whose playbooks illustrate a wealth pattern (Ma, Bezos, Soros, Kathryn Wood, Icahn, Arnault, etc.). Follow the first-person format in `references/famous-models/elon-musk.md`.
2. **New extraction patterns** — if you identify a wealth lens the 6-lens framework misses, open an issue before submitting a PR.

### Design Principles

1. **Your noise is your ore.** Every mundane interaction contains potential wealth signals.
2. **Repetition is the primary signal.** If something shows up twice in your life, it's a market.
3. **Cross-reference beats single-source.** One signal is a guess. Three are a conviction.
4. **Action over analysis.** Midas outputs next-steps, not essays.
5. **Compounding intelligence.** Day 1 gives guesses. Day 90 gives a playbook.
6. **No moral judgment.** Midas studies how money moves, not how it *should* move.
7. **Honest boundaries.** No predictions. No guarantees. No financial advice.
8. **Public information only.** Only what you voluntarily feed it.

### License

MIT. See `LICENSE`.

### Not Financial Advice

Midas does not provide investment, tax, legal, or accounting advice. Nothing in a Midas output is a recommendation to buy or sell any security. Before acting on any Midas-generated opportunity that involves material capital, consult a licensed professional in your jurisdiction.

---

## 中文

### 核心洞察

你每天都在泄漏财富信号,却浑然不觉。

- 你和同事的闲聊("最近运费涨疯了")
- 你无意中拍下的照片(一个工地、一家挤满客人的餐馆、一间空置的店铺)
- 你凌晨两点刷的视频(维修教程、产品评测、行业吐槽)
- 你划过的群聊("谁认识靠谱的会计师?""这个 APP 又崩了")
- 你重复的抱怨("为什么这么贵""没人做得好""真希望有人能做一下……")
- 你自动续费的订单(同一罐蛋白粉、同一个 SaaS 订阅、同一家外卖)

**这些都是原矿。Midas 把它提炼成黄金。**

根本洞察是:**财富不在 Bloomberg 终端里,也不在 VC 路演里。财富藏在你每天的日常噪音里。** 真正的问题不是信息获取权,而是你被训练得对每天遇到的信号视而不见。

**Midas 不只分析富豪,Midas 分析的是你自己。**

### Nuwa vs. Midas

| | Nuwa 女娲 | Midas 点石成金 |
|---|---|---|
| **提炼什么** | 人如何*思考* | 如何把你的噪音变成*钱* |
| **输入** | 传记、访谈、思想 | Slack、照片、聊天、抱怨、小票 |
| **输出** | 思维模型 | 排序后的机会 + 下一步行动 |
| **随时间变聪明** | 是 | 是(每次输入都会交叉引用) |

Nuwa 是思考工具,Midas 是财富提取工具。它们相互配合,不互相取代。

### 快速上手

```bash
# 1. 克隆仓库
git clone git@github.com:realteamprinz/midas-skill.git

# 2. 作为 Claude Code / OpenClaw 技能安装
cp -r midas-skill ~/.claude/skills/

# 3. 在任意对话中用以下触发词激活:
#    "Midas, mine this"
#    "Turn this into gold"
#    "点石成金"
#    "这里面有什么信号"

# 4. 喂给它第一批输入 —— 什么都可以:
#    - 一周的 Slack 消息
#    - 微信群聊截图
#    - 你最近 20 笔消费清单
#    - 手机里一周拍的 30 张照片
#    - 你的 B 站观看历史
```

### 六重提取引擎

每一次输入都会经过六重滤镜:

1. **金钱信号检测** — 钱在哪里流动、卡住、渗漏?
2. **需求缺口识别** — 人们想要什么而没人在好好提供?
3. **套利窗口检测** — 价值在哪里被错误定价?
4. **技能变现桥梁** — 你已经掌握的什么东西有市场价值?
5. **人脉货币化路径** — 谁该跟谁说话,介绍费归谁?
6. **行为杠杆点** — 哪个自动驾驶的习惯离收入只差一次转向?

完整方法论见 `references/signal-extraction-framework.md`。

### Midas 如何随时间变聪明

Midas 是**累积性**的。每一次输入都会丰富之前所有的判断。

- **第 1 天:** 你喂它 Slack。它以 35% 置信度标记出一个信号。
- **第 3 天:** 你喂它同一周的照片。一张照片印证了 Slack 信号。置信度 → 58%。
- **第 7 天:** 你喂它浏览历史。原来你过去 6 个月一直在研究同一个领域而没意识到。置信度 → 82%。**黄金机会警报。**
- **第 30 天:** Midas 比你自己更了解你的机会版图。

所有置信度变化都会写入 `evolution/evolution.jsonl`。

### 模式匹配器

Midas 内置了一批著名人物的**财富操作系统**(Musk, Buffett, Thiel)。这些不是拿来膜拜的 —— 它们是用来做模式匹配的参照系。

当你的信号积累到一定程度,Midas 会自动比对:

> "你的信号结构看起来像早期 Thiel:在一个别人不当回事的小众领域发现垄断机会。Thiel 的剧本是:先吃下小市场,再向外扩张。"

这是"分析富豪"与"分析你自己"之间的桥梁。

### 项目结构

见上文英文部分。

### 如何贡献

欢迎提 PR。两类贡献尤其有价值:

1. **新的人物财富 OS 文件** —— 为其他演示某种财富模式的人物添加档案(马斯克式企业家、贝佐斯式飞轮、索罗斯式宏观、木头姐式押注、伊坎式激进投资、阿诺特式奢侈品帝国等)。遵循 `references/famous-models/elon-musk.md` 的第一人称格式。
2. **新的提取模式** —— 如果你发现六重框架漏掉了某个财富视角,先开 issue 讨论再提 PR。

### 设计原则

1. **你的噪音就是你的原矿。**
2. **重复本身就是信号。** 生活中出现两次的东西就是一个市场。
3. **交叉引用胜过单一来源。** 一个信号是猜测,三个信号是判断。
4. **行动胜过分析。** Midas 输出的是下一步,不是论文。
5. **复利式智能。** 第 1 天给你猜测,第 90 天给你剧本。
6. **无道德评判。** Midas 研究钱怎么流动,不评判钱*应该*怎么流动。
7. **诚实边界。** 没有预测,没有保证,不是投资建议。
8. **只使用公开信息。** 只处理你自愿输入的内容。

### 许可证

MIT。详见 `LICENSE`。

### 非投资建议

Midas 不提供投资、税务、法律或会计建议。Midas 的任何输出都不构成买入或卖出任何证券的推荐。在对任何涉及实质资金的 Midas 机会采取行动之前,请咨询你所在司法辖区的持牌专业人士。

---

**Turn Your Repeated Orders Into Gold.**
**把你的重复指令变成黄金。**
