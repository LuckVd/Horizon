---
layout: default
title: "Horizon Summary: 2026-07-21 (ZH)"
date: 2026-07-21
lang: zh
---

> 从 41 条内容中筛选出 9 条重要资讯。

---

1. [Incremental：用于增量计算的 OCaml 库](#item-1) ⭐️ 8.0/10
2. [AI 在生成反例方面超越人类数学家](#item-2) ⭐️ 8.0/10
3. [代理群实现每秒千次提交，催生定制版本控制系统](#item-3) ⭐️ 8.0/10
4. [Claude Code 团队炉边谈话揭晓内部指标](#item-4) ⭐️ 8.0/10
5. [本·汤普森提议美国立法促进开放模型对抗中国 AI](#item-5) ⭐️ 8.0/10
6. [智谱建成全国产芯片大型数据中心](#item-6) ⭐️ 8.0/10
7. [谷歌被曝开发&\#x27;Frozen v2&\#x27;芯片，将 Gemini 写入硬件](#item-7) ⭐️ 8.0/10
8. [阿里将推千问办公，整合三款智能体](#item-8) ⭐️ 8.0/10
9. [谷歌发布 Gemini 3.6 Flash 并透露 Gemini 4 预训练](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Incremental：用于增量计算的 OCaml 库](https://github.com/janestreet/incremental) ⭐️ 8.0/10

Jane Street 发布了 Incremental，这是一个 OCaml 库，能够在输入数据变化时高效地部分重新评估计算图。 该库将增量计算引入 OCaml，可提升电子表格重新计算、UI 更新和派生数据同步等应用的性能，并与响应式编程和构建系统等更广泛的趋势相联系。 Incremental 基于自调整计算研究构建，支持电子表格式计算和 GUI 视图更新等用例，并被 Jane Street 的 Bonsai UI 库所使用。

hackernews · handfuloflight · 7月21日 03:50 · [社区讨论](https://news.ycombinator.com/item?id=48987822)

**背景**: 增量计算是一种通过仅重新计算依赖于变化数据的输出来节省时间的技术，常用于电子表格和构建系统。Incremental 库在 OCaml 中实现了这一技术，灵感来源于自调整计算研究。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Incremental_computation">Incremental computation</a></li>
<li><a href="https://github.com/janestreet/incremental">GitHub - janestreet/incremental: A library for incremental ...</a></li>

</ul>
</details>

**社区讨论**: 评论者指出 Incremental 与 JavaScript 框架中的响应式编程信号类似，并将其与构建系统和差分数据流系统（如 Materialize）进行比较。有评论提到高盛曾采用类似方法进行工具定价。讨论积极且富有洞察力，展示了各种应用和联系。

**标签**: `#incremental computation`, `#reactive programming`, `#OCaml`, `#janestreet`, `#signals`

---

<a id="item-2"></a>
## [AI 在生成反例方面超越人类数学家](https://xenaproject.wordpress.com/2026/07/20/human-mathematicians-are-being-outcounterexampled/) ⭐️ 8.0/10

AI 系统如今生成数学中 97%的反例，超越人类数学家，正在改变研究实践。 这一转变使数学家能够快速证伪错误猜想，节省时间并专注于证明真实命题，同时也重新定义了人类直觉在数学发现中的作用。 相关技术包括将猜想重构为优化或搜索任务，利用机器学习和计算搜索来探索巨大的可能性空间。

hackernews · artninja1988 · 7月20日 19:03 · [社区讨论](https://news.ycombinator.com/item?id=48983382)

**背景**: 反例是证伪猜想的特定实例，在完善定义和精确证明中起关键作用。自动定理证明一直是计算机科学的长期目标，但近年来 AI 和机器学习的进展显著加速了反例的发现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://math.duke.edu/mathplus/2025/ai-powered-discovery-counterexamples-combinatorics">AI powered discovery of counterexamples in combinatorics</a></li>
<li><a href="https://www.youtube.com/watch?v=vxeSjfwJQRE">97% of Counterexamples Are Now AI-Generated! - YouTube Images</a></li>
<li><a href="https://en.wikipedia.org/wiki/Automated_theorem_proving">Automated theorem proving</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍对此持积极态度，认为这节省了在错误猜想上浪费的时间，让数学家专注于富有成效的研究。有人将其与国际象棋计算机类比，起初擅长计算，后来激发创意走法。关于雅可比猜想的引用说明了未察觉错误可能带来的人性代价。

**标签**: `#mathematics`, `#AI`, `#theorem proving`, `#counterexamples`, `#research methodology`

---

<a id="item-3"></a>
## [代理群实现每秒千次提交，催生定制版本控制系统](https://cursor.com/blog/agent-swarm-model-economics) ⭐️ 8.0/10

Cursor 的博客报告了代理群实验，实现了高达每秒 1000 次的提交率，这需要专门构建的版本控制系统（VCS）来管理吞吐量和协调。 这展示了 AI 代理的极端扩展潜力，同时揭示了必须在实际应用中克服的基础设施瓶颈（如 VCS），引发了社区关于此类基准测试有效性的辩论。 新系统峰值可达每秒 1000 次提交，相较之前浏览器群每小时 1000 次提交有千倍提升。自定义 VCS 从头构建，用于高速处理冲突检测和协调。

hackernews · jlaneve · 7月20日 18:06 · [社区讨论](https://news.ycombinator.com/item?id=48982535)

**背景**: 代理群协调多个 AI 代理并行处理复杂任务。传统的版本控制系统（如 Git）并非为这种高提交率和自主协调需求而设计。Cursor 的实验挑战了代理群的能力极限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.swarms.ai/">Swarms AI — Multi- Agent Framework &amp; Agent Marketplace</a></li>
<li><a href="https://www.freestyle.sh/blog/engineering/version-control-for-ai-agents">Version Control for AI Agents - Freestyle Blog</a></li>

</ul>
</details>

**社区讨论**: 像 anthonypasq 这样的评论者赞赏其前瞻性，而 notahan 则将这些结果斥为“刷榜”并质疑其实际适用性。handfuloflight 指出 SQLite 源代码可能已在训练数据中，这使测试的有效性受到质疑。

**标签**: `#agent swarms`, `#AI`, `#version control`, `#software engineering`, `#benchmarking`

---

<a id="item-4"></a>
## [Claude Code 团队炉边谈话揭晓内部指标](https://simonwillison.net/2026/Jul/21/cat-and-thariq/#atom-everything) ⭐️ 8.0/10

在 AI 工程师世界博览会的炉边谈话中，Anthropic Claude Code 团队的 Cat Wu 和 Thariq Shihipar 透露，Claude Tag 目前处理了他们 65%的产品工程拉取请求，并且由于 Fable 5 等新模型，Claude Code 的系统提示词大小减少了 80%。 这表明 Anthropic 自身对 AI 编码代理的高度信任和采用，并反映了模型成熟后最佳实践的转变（减少提示词示例和禁止性指令），对使用 Claude Code 及其他 AI 编码工具的开发者具有重要影响。 Claude Tag 是一种依赖自动模式的 Slack 协作集成；Anthropic 内部将“吃狗粮”称为“吃蚂蚁”；Fable 被用于编辑其自己的发布视频；Thariq 建议开发者更雄心勃勃以抵消编码代理带来的效率提升。

rss · Simon Willison · 7月21日 12:54

**背景**: Claude Code 是 Anthropic 推出的 AI 编码代理，帮助开发者编写代码。Claude Tag 是一种协作集成，允许团队在 Slack 频道中与 Claude 协作。Fable 5 是 Anthropic 于 2026 年 6 月发布的最强大模型，适用于复杂编码任务。这次炉边谈话提供了 Claude Code 团队自身使用产品的内部视角。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_%28AI%29">Claude (AI)</a></li>
<li><a href="https://www.anthropic.com/news/introducing-claude-tag">Introducing Claude Tag \ Anthropic</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>

</ul>
</details>

**标签**: `#Claude Code`, `#AI coding agents`, `#Anthropic`, `#developer tools`, `#productivity`

---

<a id="item-5"></a>
## [本·汤普森提议美国立法促进开放模型对抗中国 AI](https://simonwillison.net/2026/Jul/20/afraid-of-chinese-models/#atom-everything) ⭐️ 8.0/10

本·汤普森提议美国通过法律，将训练数据收集视为合理使用，并禁止服务条款中禁止蒸馏，以帮助美国开放模型与 Qwen 3.8 Max 等中国模型竞争。 该提议直接针对 AI 实验室在未授权数据上训练却禁止蒸馏的矛盾行为，可能改变美国版权政策以支持开放性，加速 AI 创新。 该提议包含两大支柱：训练数据的明确合理使用和禁止反蒸馏服务条款。本·汤普森还指出，阿里巴巴以开放权重发布 Qwen 3.8 Max 可能受到习近平呼吁开源协作的讲话影响。

rss · Simon Willison · 7月20日 17:09

**背景**: AI 蒸馏是一种通过 API 查询让小型模型从大型模型输出中学习的技术。使用受版权保护数据训练模型的法律地位尚不明确，部分法院认定其为合理使用。开放权重模型允许用户运行模型，但不一定允许修改或重新分发，不同于真正的开源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://intellibytes.substack.com/p/ai-distillation-explained-what-it">AI Distillation Explained: What It Is, How It Works, Legality Concerns</a></li>
<li><a href="https://neysa.ai/blog/open-weights-open-source/">Open Weights vs Open Source: What’s the Real Difference?</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#distillation`, `#copyright`, `#Chinese AI models`, `#open models`

---

<a id="item-6"></a>
## [智谱建成全国产芯片大型数据中心](https://www.bloomberg.com/news/articles/2026-07-20/z-ai-completes-giant-data-center-with-chinese-chips-to-train-ai) ⭐️ 8.0/10

中国 AI 实验室智谱完成了全部采用国产芯片的 1 吉瓦数据中心建设，并已开始部分运营，用于支持其 GLM 平台开发。 这一里程碑展示了国产芯片在大型 AI 训练中的规模化应用能力，减少对外国硬件的依赖，推动了中国 AI 自主可控的目标。 该设施是中国 AI 实验室建造的最大规模设施之一，其功率足以为约 75 万户家庭供电，且已建成多个各拥有超万枚芯片的计算集群。

telegram · zaihuapd · 7月20日 15:43

**背景**: 智谱是中国领先的人工智能企业，以其 GLM 系列大语言模型闻名。该数据中心完全采用国产芯片，反映了中国在先进外国芯片（如英伟达）出口限制下，推动半导体生态系统自主可控的努力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://open.bigmodel.cn/">bigmodel - 智谱AI开放平台</a></li>

</ul>
</details>

**标签**: `#国产芯片`, `#数据中心`, `#AI`, `#智谱`, `#中国科技`

---

<a id="item-7"></a>
## [谷歌被曝开发&\#x27;Frozen v2&\#x27;芯片，将 Gemini 写入硬件](https://www.quiverquant.com/news/Google+Reportedly+Developing+%E2%80%98Frozen+v2%E2%80%99+AI+Chip+to+Boost+Gemini+Efficiency) ⭐️ 8.0/10

据报道，谷歌正在开发一款代号为&\#x27;Frozen v2&\#x27;的服务器芯片，将 Gemini AI 模型的部分能力直接融入硬件，推理效率可达最新 TPU 的 6 到 10 倍，计划于 2028 年部署。 这种方法显著降低了计算开销和功耗，可能缓解谷歌内部的算力短缺，并实现更高效的 AI 服务。它代表了向模型特定硬件的转变，可能影响整个 AI 芯片行业。 该芯片旨在补充而非取代谷歌的 TPU 产品线，专注于 Gemini 模型的推理。它通过将神经网络架构直接嵌入电路来减少数据移动，这种技术被称为&\#x27;冻结&\#x27;。

telegram · zaihuapd · 7月21日 01:01

**背景**: 当前的 AI 芯片如 GPU 和 TPU 是通用加速器，将模型存储在内存中并来回传输数据，消耗电力和时间。谷歌的 TPU 是其自研的机器学习专用 ASIC。Frozen v2 概念进一步专业化，将特定模型架构锁定在硅片中，虽然限制了灵活性，但针对该模型实现了效率最大化。这类似于比特币挖矿 ASIC 在特定任务上优于通用硬件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://qz.com/google-gemini-chip-frozen-tpu-efficiency-072026">Google developing Gemini-specific chip called Frozen v 2</a></li>
<li><a href="https://techcrunch.com/2026/07/20/google-is-working-on-a-new-ai-chip-designed-to-make-gemini-more-efficient/">Google is working on a new AI chip designed to make Gemini ...</a></li>
<li><a href="https://thenextweb.com/news/google-frozen-chip-gemini-silicon">Google Frozen chip : Gemini baked into the silicon</a></li>

</ul>
</details>

**标签**: `#AI芯片`, `#Google`, `#Gemini`, `#硬件优化`, `#推理效率`

---

<a id="item-8"></a>
## [阿里将推千问办公，整合三款智能体](https://finance.sina.com.cn/roll/2026-07-21/doc-iniiqefa9222987.shtml) ⭐️ 8.0/10

阿里巴巴即将推出“千问办公”，该产品整合了 QoderWork、悟空和 MuleRun 三款智能体，形成统一的办公平台。该项目由钉钉新任 CEO 陈宇森负责，定位为阿里在智能体办公市场的旗舰产品。 此次整合表明阿里巴巴在智能体办公市场的战略性布局，将竞争从传统协作工具转向 AI 驱动生态。随着腾讯、字节跳动等对手也在整合智能体产品，此举可能重塑企业生产力领域的竞争格局。 千问办公将以 QoderWork 为基础，QoderWork 是一款能够自主规划和执行任务的桌面 AI 智能体。该产品瞄准“Agent 办公”市场，旨在为企业工作流程提供全面的 AI 助手。

telegram · zaihuapd · 7月21日 10:11

**背景**: AI 智能体是一种自主软件程序，能够理解目标并执行多步任务，无需人工持续干预。阿里巴巴、腾讯、字节跳动等公司正竞相将此类智能体整合到办公套件中，从钉钉、飞书等传统协作工具转向 AI 生态。“Agent 办公”趋势代表了从人工驱动工作流到 AI 编排生产力的转变。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://qoder.com/qoderwork">QoderWork - AI Desktop Assistant | Intelligent Task Automation Tool | Qoder</a></li>
<li><a href="https://blog.csdn.net/2301_76268839/article/details/146032147">智能办公文具：AI Agent的工作效率追踪_ai agent办公-CSDN博客</a></li>

</ul>
</details>

**标签**: `#阿里`, `#千问办公`, `#智能体`, `#钉钉`, `#Agent办公`

---

<a id="item-9"></a>
## [谷歌发布 Gemini 3.6 Flash 并透露 Gemini 4 预训练](https://9to5google.com/2026/07/21/gemini-3-6-flash-launch/) ⭐️ 8.0/10

谷歌发布了 Gemini 3.6 Flash，该模型减少了 17%的输出 Token，并改进了推理步骤和工具调用。谷歌还透露了 Gemini 4 的预训练，并推出了包括 Gemini 3.5 Flash-Lite 和 3.5 Flash Cyber 在内的新模型。 此次发布展示了谷歌在 AI 领域的持续投入，提供了更高效、更专业化的模型。Gemini 4 的预训练标志着其旗舰模型的下一代发展，可能进一步提升 AI 助手和企业工具的能力。 Gemini 3.6 Flash 的知识截止日期为 2026 年 3 月，API 定价为每百万输入 Token 1.5 美元、输出 Token 7.5 美元。此外，Gemini 3.5 Pro 正在与合作伙伴测试，DeepMind 已开始对 Gemini 4 进行大规模预训练。

telegram · zaihuapd · 7月21日 15:23

**背景**: Token 是 AI 模型处理的文本单元，通常是单词的一部分或标点符号。推理步骤指模型将复杂问题分解为中间步骤的过程，通常使用思维链提示来提高准确性和透明度。知识截止日期表示模型训练数据最后一次更新的时间，影响其对近期事件的了解。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blogs.nvidia.com/blog/ai-tokens-explained/">What Are AI Tokens ? The Language and Currency... | NVIDIA Blog</a></li>
<li><a href="https://www.ibm.com/think/topics/chain-of-thoughts">What is chain of thought (CoT) prompting? | IBM</a></li>
<li><a href="https://www.linkedin.com/posts/arista-witty_knowledge-cut-off-in-ai-what-it-means-activity-7439630888201687040-3fkf">AI Knowledge Cutoff Dates and RAG Technology | Arista... | LinkedIn</a></li>

</ul>
</details>

**标签**: `#AI`, `#Google`, `#Gemini`, `#model release`, `#DeepMind`

---