## 递归客（diguike）

Agent 工程师，也写技术书。全栈出身，主力是 Node.js + TypeScript。

工程上一直在琢磨几件事：怎么让 Agent 自己迭代、自己拿反馈变好；怎么让长程 Agent 跑得久又不跑偏；团队里的 skill、prompt、知识库、评测集这些 AI 资产怎么攒起来；一个团队的 AI 体系又该从哪里搭起。

另一半时间在写书。一个方向弄明白了，就写成一本工程师拿来能直接上手的书，正文和代码都开源。最近还在做自己的产品 [GoAfter6](https://goafter6.com)。

我学东西的路子比较笨：先读源码，再自己写一遍跑通，确认理解没偏，才写出来给别人看。写出来的东西都放在 [inferloop.dev](https://inferloop.dev)。

> Agent engineer. I write hands-on Chinese books on AI agents and LLM infra, with runnable code, all open source.

---

### 现在在做

- GoAfter6：帮人准点下班的产品，北京已上线，介绍在下面
- 《源码精读》还在一章章往后加，每章读透一个开源项目
- 把《Agent 知识库工程实战》搬上 inferloop.dev，现在只能在 GitHub 上看

---

### 产品

**GoAfter6 · 下班健康** — [goafter6.com](https://goafter6.com)

AI 帮人省下来的时间，转头就会被新活填满。可要是晚上真约了一场读书会、一节课或者一场夜跑，白天自然会排得紧一点，下午也不太会再开新坑，到点就走。GoAfter6 做的就是这件事：给你一个今晚值得赶的理由，再帮你把它赶上。

- 找今晚赶得上的工作日活动，或者自己发起一个。排序看从公司过去多远、几点开始、多少钱、一个人去合不合适
- 报名后，通勤和活动一起写进日历（Google / 飞书 / ICS），算出最晚几点必须走，到点提醒你出发，而不是等活动开始了才提醒
- 桌面端在后台记下每天第一次和最后一次干活的时间。攒上一段，拿有活动和没活动的工作日一比，就知道下班到底早了没有、拿回了几个晚上

用 Next.js + TypeScript + Tailwind 写，跑在 Cloudflare Workers 上，数据存 MongoDB；另外有一个 macOS 菜单栏采集器和一个 Android 的 React Native 壳。活动查询和投稿开了个人 Token API，也打包成了可以直接安装的 Agent Skill。

拿过 VibeHacks #05「Vibe Coding for 准点下班」的最具变现潜力奖。目前只做北京，代码不开源，欢迎直接上站试试。

---

### 书

17 本。除了《源码精读》还在往后加，其余都已写完，正文和配套代码都开源在这个账号下。

**Agent 工程**

- **Hermes Agent 实战** — 解剖一个会成长的个人 AI Agent · [在线](https://inferloop.dev/hermes-agent) · [源码](https://github.com/diguike/book-hermes-agent)
- **自己动手写 AI Agent** — 从 Claude Code 架构到你的第一个编程助手 · [在线](https://inferloop.dev/ling-agent) · [源码](https://github.com/diguike/book-ling-agent)
- **一切皆插件** — DeepSeek Harness 源码精读、Mini 实现与插件开发实战 · [在线](https://inferloop.dev/deepseek-harness) · [源码](https://github.com/diguike/book-deepseek-harness)
- **OpenClaw 源码解析** — 现代 Agent 系统架构 · [在线](https://inferloop.dev/openclaw) · [源码](https://github.com/diguike/book-openclaw)
- **LangChain.js Agent 开发权威指南** — TypeScript 工程师的 LangChain 1.x · [在线](https://inferloop.dev/langchain-agent) · [源码](https://github.com/diguike/book-langchain-agent)
- **Agent Memory 工程实战** — 基于 claude-mem 源码 · [在线](https://inferloop.dev/claude-mem) · [源码](https://github.com/diguike/book-claude-mem)
- **Agent 知识库工程实战** — 知识库的组织、分发、共建与度量 · [源码](https://github.com/diguike/agent-knowledge-base-engineering)
- **百万级 AI Agent 平台架构** — 智能客服 SaaS 实战 · [在线](https://inferloop.dev/enterprise-agent) · [源码](https://github.com/diguike/book-enterprise-agent)

**Agent 评测**

- **AI Agent 评测工程实战** — 从 0 用 TypeScript 构建评测平台 · [在线](https://inferloop.dev/agent-evals) · [源码](https://github.com/diguike/book-agent-evals)
- **Agent Harness 评测工程** — 给已经在跑的 harness 装上评测闭环 · [在线](https://inferloop.dev/harness-evals) · [源码](https://github.com/diguike/book-harness-evals)

**LLM Infra**

- **LLM Infra 工程实战** — 面向应用层工程师的 LLM 基础设施 · [在线](https://inferloop.dev/llm-infra) · [源码](https://github.com/diguike/book-llm-infra)
- **AI Token 中转站实战** — 从 0 搭建企业级 LLM 网关 · [在线](https://inferloop.dev/llm-gateway) · [源码](https://github.com/diguike/book-llm-gateway)
- **Transformer 工程实战** — 从向量、注意力机制到 RAG · [在线](https://inferloop.dev/transformer) · [源码](https://github.com/diguike/book-transformer)

**工具与生态**

- **Claude Code Skill 开发指南** · [在线](https://inferloop.dev/claude-skill) · [源码](https://github.com/diguike/book-claude-skill)
- **Claude 插件官方指南** · [在线](https://inferloop.dev/claude-plugins) · [源码](https://github.com/diguike/book-claude-plugins)
- **AI 时代的 CLI 工具开发实战** — 用 TypeScript 构建现代 CLI，贯穿案例是 repox · [在线](https://inferloop.dev/repox) · [源码](https://github.com/diguike/repox)
- **源码精读** — 持续追加，每章一个开源仓库 · [在线](https://inferloop.dev/source-reading) · [源码](https://github.com/diguike/book-source-reading)

哪本对你有用，去对应仓库点个 star 我就知道了。

---

### 顺手做的东西

- **AI 发音速查** — 带发音的 AI 黑话词典：CUDA、Qwen、nginx 这些看得懂却念不准的词，点击即听标准读法，配中文谐音和一句话含义，收录 290+ 术语 · [打开](https://inferloop.dev/pronounce) · [源码](https://github.com/diguike/ai-pronounce)
- **克劳德医生** — 给 Claude Code 做封禁风险体检的 CLI：检测 → 修复 → 复验，只算有因果的信号 · [打开](https://claudedoctor.pages.dev) · [源码](https://github.com/diguike/claudedoctor)
- **lark-ai-task-queue** — 把飞书任务清单当成寄给 AI 的待办队列：定时拉取、执行、产出文档再回写 · [源码](https://github.com/diguike/lark-ai-task-queue)
- **工具推荐** — 我自己天天在用的工具，一篇讲一个，像跟朋友聊工具那样写，不写成产品手册 · [源码](https://github.com/diguike/tool-picks)
- **CoffeesMap** — 找安静咖啡馆的地图，专挑能带电脑坐一下午的店 · [打开](https://coffeesmap.pages.dev/)

---

### 联系

- 站点 · [inferloop.dev](https://inferloop.dev)（书与公开产物）
- 产品 · [goafter6.com](https://goafter6.com)（GoAfter6 · 下班健康）
- 邮箱 · diguike@inferloop.dev（合作 / 约稿 / 勘误 / 课程使用）
- 公众号 · **AI Reading Hub**

<img src="https://meikan-public-images.oss-cn-beijing.aliyuncs.com/imeikan/assets/2025-06-13005433-qrcode_for_gh_27101e9a2f9d_258.jpg" alt="递归客的公众号 AI Reading Hub 二维码" width="140" />
