---
layout: default
title: "Horizon Summary: 2026-07-27 (ZH)"
date: 2026-07-27
lang: zh
---

> 从 33 条内容中筛选出 11 条重要资讯。

---

1. [vLLM v0.26.0 发布：新增 Inkling 模型系列和 DeepSeek-V4 性能提升](#item-1) ⭐️ 9.0/10
2. [美国公民在边境使用 GrapheneOS 胁迫 PIN 擦除手机后遭起诉](#item-2) ⭐️ 8.0/10
3. [Go 分析框架：Go 团队推出的模块化静态分析](#item-3) ⭐️ 8.0/10
4. [欧盟提议浏览器级隐私设置消灭 Cookie 横幅](#item-4) ⭐️ 8.0/10
5. [中继市场助长 LLM 代币转售与欺诈](#item-5) ⭐️ 8.0/10
6. [开源 4B 模型在瑞典语医学问答中接近 o3 水平](#item-6) ⭐️ 8.0/10
7. [LLM 在 IMO 2026 题目上的比较：前沿模型表现优异](#item-7) ⭐️ 8.0/10
8. [长鑫科技明日登陆上海证券交易所，有望成 A 股市值最高公司](#item-8) ⭐️ 8.0/10
9. [Claude 共享链接遭搜索引擎索引泄露数据](#item-9) ⭐️ 8.0/10
10. [SpaceX 拒收 Falcon 9 远期订单，全力押注 Starship](#item-10) ⭐️ 8.0/10
11. [谷歌 Gemini 4：迄今最雄心预训练，预计年底发布](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.26.0 发布：新增 Inkling 模型系列和 DeepSeek-V4 性能提升](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 9.0/10

vLLM v0.26.0 已发布，新增对 Inkling 模型系列的全面支持，显著优化 DeepSeek-V4 性能，引入灵活注意力后端，共有 411 次提交和 212 位贡献者。 这次发布增强了 vLLM 的通用性，支持了如 Inkling（多模态 MoE）等前沿模型，并提高了 DeepSeek-V4（一个重要的开源权重模型）的生产部署效率。灵活的注意力后端和扩展的硬件支持惠及整个 LLM 推理生态。 Inkling 支持包括基础建模、CUDA 图、Hopper FA4 相对注意力、MTP 推测解码、LoRA 和 ModelOpt NVFP4 量化。DeepSeek-V4 优化包括专用路由内核（端到端 TPOT 提升 2.94%）和 fused\_topk\_bias（内核速度提升 1.5-2 倍）。

github · khluu · 7月27日 01:06

**背景**: vLLM 是一个开源的高性能 LLM 推理库。Thinking Machines Lab 开发的 Inkling 模型系列是一个多模态混合专家模型（总计 9750 亿参数，410 亿激活），支持文本、图像和音频。DeepSeek-V4 是中国 DeepSeek 公司推出的开源权重 MoE 模型系列，参数规模可达 1.6 万亿。此次发布引入了按 KV 缓存组选择注意力后端的灵活性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.baseten.co/library/inkling/">Inkling | Model library</a></li>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling : Our Open-Weights Model - Thinking Machines Lab</a></li>
<li><a href="https://docs.vllm.ai/en/stable/api/vllm/models/inkling/nvidia/ops/fa4_rel_attention/">fa 4 _rel_ attention - vLLM</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#release notes`, `#model optimization`, `#attention mechanisms`

---

<a id="item-2"></a>
## [美国公民在边境使用 GrapheneOS 胁迫 PIN 擦除手机后遭起诉](https://www.techspot.com/news/113236-us-prosecutors-charge-atlanta-man-after-grapheneos-phone.html) ⭐️ 8.0/10

一名来自亚特兰大的美国公民在边境检查期间使用 GrapheneOS 的胁迫 PIN 功能擦除了手机，随后被起诉。 此案引发了关于边境数字隐私和安全实践的重要法律问题，政府搜查权与个人隐私权在此产生冲突。 胁迫 PIN 是 GrapheneOS 的一项功能，输入该 PIN 会有意擦除设备而非解锁。这与多次尝试失败后的自动擦除不同。

hackernews · eecc · 7月26日 22:21 · [社区讨论](https://news.ycombinator.com/item?id=49063022)

**背景**: GrapheneOS 是一个基于 Android 的注重安全的移动操作系统，旨在保护隐私和防御攻击。胁迫 PIN 是一种嵌入在身份验证中的求救信号：输入特定 PIN 可以触发擦除设备等操作，用于用户被迫解锁手机的情况。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GrapheneOS">GrapheneOS</a></li>
<li><a href="https://en.wikipedia.org/wiki/Duress_PIN">Duress PIN</a></li>

</ul>
</details>

**社区讨论**: 评论者们就法律影响和用户责任进行了辩论。有人认为在边境使用胁迫 PIN 存在风险，用户必须接受后果，而另一些人则建议采用如 VeraCrypt 的隐藏卷等替代方法。

**标签**: `#GrapheneOS`, `#duress PIN`, `#privacy`, `#border security`, `#digital rights`

---

<a id="item-3"></a>
## [Go 分析框架：Go 团队推出的模块化静态分析](https://pkg.go.dev/golang.org/x/tools/go/analysis) ⭐️ 8.0/10

Go 分析框架（具体为 golang.org/x/tools/go/analysis 包）为 Go 语言提供了模块化静态分析接口，允许开发者创建可组合和复用的自定义 linter 和分析器。 该框架标准化了 Go 语言的静态分析过程，使开发者能够轻松创建自定义 linter 并与 LLM 等 AI 工具集成，从而改进代码审查流程并减少技术债务。 该框架支持传递性分析，即一个分析器的输出可作为另一个分析器的输入。它每次只检查一个包，但允许在不同包之间共享信息。

hackernews · AbuAssar · 7月26日 12:21 · [社区讨论](https://news.ycombinator.com/item?id=49057398)

**背景**: 静态分析在不运行代码的情况下检查源代码，帮助查找错误、强制代码风格并提升质量。模块化静态分析框架允许开发者编写独立的检查（分析器），这些检查可以组合在一起运行。Go 分析框架提供了定义、运行和组合这些分析器的标准方式，便于创建 linter 和代码格式化工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pkg.go.dev/golang.org/x/tools/go/analysis">analysis package - golang.org/x/tools/go/analysis - Go Packages</a></li>
<li><a href="https://arslan.io/2020/07/07/using-go-analysis-to-fix-your-source-code/">Using go / analysis to fix your source code</a></li>
<li><a href="https://docs.google.com/document/d/1-azPLXaLgTCKeKDNg0HVMq2ovMlD-e7n1ZHzZVzOlJk/edit">Analysis API: modular static analysis for Go - Google Docs</a></li>

</ul>
</details>

**社区讨论**: 讨论中包含对 Go 设计和工具的高度赞赏，一位用户称赞了语言的可读性。一个实用评论指出，该框架结合 LLM 能简化自定义分析器的创建，用于代码审查。但也有用户指出该框架并非新事物，已被广泛使用。

**标签**: `#Go`, `#static analysis`, `#linter`, `#code quality`, `#developer tools`

---

<a id="item-4"></a>
## [欧盟提议浏览器级隐私设置消灭 Cookie 横幅](https://killthecookiebanner.eu/) ⭐️ 8.0/10

欧盟委员会提出一项新方案，允许用户在浏览器中一次性设置隐私偏好，从而消除网站上的 Cookie 横幅。 该提案可能简化同意管理并提升用户体验，但其成功取决于广泛采纳，并避免重蹈 P3P 等先前尝试的覆辙。 浏览器级别的设置功能类似于 Global Privacy Control \(GPC\)，向网站发送用户偏好信号，但技术可行性和浏览器的支持仍是未解问题。

hackernews · rapnie · 7月26日 11:53 · [社区讨论](https://news.ycombinator.com/item?id=49057175)

**背景**: Cookie 横幅在欧盟电子隐私指令要求对非必要 Cookie 获取同意后变得普遍。停滞的 ePrivacy Regulation 提案旨在取代该指令，但争论仍在继续。早期的 P3P 和 Do Not Track 等举措曾试图自动化隐私选择，但因缺乏行业采纳而失败。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://digitalcompliance.snellman.com/regulation/e-privacy-regulation-proposal/">e- Privacy Regulation ( proposal ) - EU Digital Compliance Tracker...</a></li>
<li><a href="https://medium.com/@sean.oriyano/do-not-track-vs-global-privacy-control-cc0ad5655e53">Do Not Track vs. Global Privacy Control | by Sean Oriyano | Medium</a></li>
<li><a href="https://privacybadger.org/">Privacy Badger | Electronic Frontier Foundation</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了谨慎乐观：一些人支持浏览器级别方法，但警告像 P3P 那样的过去失败；其他人认为真正的解决方案是彻底停止跟踪。还有评论者提到加州的类似举措是积极范例。

**标签**: `#privacy`, `#cookie banners`, `#EU regulation`, `#browser`, `#web standards`

---

<a id="item-5"></a>
## [中继市场助长 LLM 代币转售与欺诈](https://simonwillison.net/2026/Jul/26/relay-market/#atom-everything) ⭐️ 8.0/10

Matt Lenhard 的调查揭示了一个蓬勃发展的市场，转售商通过汇集来自欺诈来源的 API 密钥来提供折扣 LLM 代币，主要在中国活跃。 这一欺诈生态系统对 LLM 供应商和合法用户构成重大安全风险，因为它利用免费试用、窃取的凭证和拒付攻击，并可能导致模型蒸馏和滥用。 这些代理使用开源软件如 one-api 及其分支 new-api，它们是合法的 API 代理工具，可在汇集的多组 API 凭证之间进行负载均衡。

rss · Simon Willison · 7月26日 19:30

**背景**: LLM 代币是用于衡量语言模型 API 使用量的单位；供应商按代币收费。转售商利用免费试用、未受保护的支持机器人、被盗信用卡和拒付攻击来获得廉价或免费的 API 访问，然后通过代理服务以折扣价转售。这些代理的开源性质使欺诈者很容易建立此类运营。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/IllTamer/new-api-proxy">GitHub - IllTamer/ new - api - proxy : AI...</a></li>
<li><a href="https://proxyapi.ru/">ProxyAPI - OpenAI API , DeepSeek API , Gemini API , Claude API ...</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论可能表达了对安全影响的担忧，并呼吁 LLM 供应商提供更好的 API 密钥上限和监控。中文论坛帖子（v2ex）是文章的主要来源，提供了该市场的详细示例。

**标签**: `#LLM`, `#security`, `#fraud`, `#API`, `#AI`

---

<a id="item-6"></a>
## [开源 4B 模型在瑞典语医学问答中接近 o3 水平](https://www.reddit.com/r/MachineLearning/comments/1v71wds/openweight_4b_models_approach_o3level_medical/) ⭐️ 8.0/10

实验表明，像 Qwen3.5-4B 这样的开源 4B 参数模型，在启用推理后，在瑞典医学执照考试 MedQA-SWE 上达到了 87%的准确率，接近 OpenAI o3 模型的 88%。这相比之前经过监督微调仅达 60%的 MedGemma-1.5-4B 是一个重大飞跃。 这表明小型高效的开放权重模型在专业任务上能与专有顶级系统相媲美，有望在资源较少的语言中普及医疗 AI。同时也凸显了紧凑模型推理能力的快速进步。 Qwen3.5-4B 尽管输入为瑞典语，却用英语进行推理，说明语言并非推理障碍，其训练数据中瑞典语仅占 1%。作者使用了 S-GRPO 论文中的早期退出思考干预以防止无限循环，并尝试用强化学习缩短推理轨迹，但收益甚微。

reddit · r/MachineLearning · /u/AccomplishedCat4770 · 7月26日 11:58

**背景**: 开放权重模型是指其训练参数公开可用的大语言模型，允许修改和研究。S-GRPO 是一种强化学习方法，支持从思维链推理中早期退出以避免过度计算。MedQA-SWE 是一个基于瑞典执业医师考试创建的多选题数据集。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ai21.com/glossary/foundational-llm/open-weights-model/">What is an Open-Weights Model? | AI21</a></li>
<li><a href="https://arxiv.org/abs/2505.07686">S - GRPO : Early Exit via Reinforcement Learning in Reasoning Models</a></li>
<li><a href="https://aclanthology.org/2024.lrec-main.975/">MedQA-SWE - a Clinical Question &amp; Answer Dataset for Swedish - ACL Anthology</a></li>

</ul>
</details>

**标签**: `#Machine Learning`, `#LLM`, `#Medical AI`, `#Reasoning`, `#Swedish`

---

<a id="item-7"></a>
## [LLM 在 IMO 2026 题目上的比较：前沿模型表现优异](https://www.reddit.com/r/MachineLearning/comments/1v6wskz/we_compared_different_llms_on_imo_2026_r/) ⭐️ 8.0/10

这项研究系统性地比较了多个大型语言模型在国际数学奥林匹克（IMO）2026 题目上的表现，结果显示前沿模型（sol 和 fable）无论使用何种框架都能获得接近满分的成绩，而其他模型（如 sonnet、opus 和 GLM）在使用专门设计的框架（如 Claude Code 和 AutoFyn）后性能显著提升。 这一基准测试表明，艰苦的数学推理仍然是 LLM 通用智能的有力替代指标，框架工程可以部分缩小差距但无法完全弥合。同时它也突显了即使先进模型在可验证领域仍存在幻觉问题。 评分由前沿模型进行并通过前 IMO 奖牌得主人工验证。在最难的问题（P3）上，所有非前沿模型即使在 20 小时运行后也无法找到关键简化步骤，表明存在根本性的推理局限。

reddit · r/MachineLearning · /u/pequalnp92 · 7月26日 07:21

**背景**: 国际数学奥林匹克（IMO）是一场面向中学生的著名赛事，其题目新颖且考验深层数学推理能力。LLM 框架（harness）是一种协调模型调用、工具和记忆的架构，帮助模型解决复杂的多步骤任务。本研究中使用的 AutoFyn 是一个自定义多智能体框架，旨在通过检索和验证来改善推理。这类框架在 LLM 实际部署中愈发重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/agent-framework/agents/harness">Agent Harnesses | Microsoft Learn</a></li>
<li><a href="https://ryanalberts.github.io/best-of-Agent-Harnesses/">Best of Agent Harnesses — curated, ranked AI agent harnesses</a></li>

</ul>
</details>

**标签**: `#LLM`, `#Benchmark`, `#Mathematical Reasoning`, `#IMO`, `#Multi-agent Harness`

---

<a id="item-8"></a>
## [长鑫科技明日登陆上海证券交易所，有望成 A 股市值最高公司](https://www.bloomberg.com/news/articles/2026-07-26/memory-frenzy-primes-china-champion-cxmt-for-historic-debut?srnd=phx-technology) ⭐️ 8.0/10

中国 DRAM 制造商长鑫科技（CXMT）完成了自 2010 年以来 A 股最大规模 IPO，募集资金 666 亿元（约 98 亿美元），将于上海证券交易所挂牌，发行价每股 8.66 元，初始市值约 5800 亿元。散户认购超额 212 倍，940 万个订单共冻结约 7.07 万亿元资金。 这一里程碑式的 IPO 彰显了中国推动半导体自主化的努力，若长鑫科技首周股价上涨约 330%，将可能超越工商银行，成为 A 股市值最高的公司。在地缘政治紧张和全球芯片供应链重塑的背景下，该事件反映了投资者对国内 DRAM 行业的强烈信心。 长鑫科技的发行估值较全球 DRAM 同行折价约 56%，较国内芯片同行折价约 77%。分析师预计，若首周股价上涨 330%，其市值将超越工商银行；华西证券更给出 5 万亿元市值预期，认为公司到 2028 年营收有望增至 5727 亿元。

telegram · zaihuapd · 7月26日 07:31

**背景**: DRAM（动态随机存取存储器）是一种常用于计算机和服务器的半导体存储器，用于临时数据存储。IDM（设计制造一体化）模式指企业自主完成芯片设计、制造和销售，与将生产外包的无晶圆厂模式相对。长鑫科技是中国规模最大、技术最先进的 DRAM IDM 企业，在中国减少对外国内存芯片依赖的努力中扮演关键角色。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cn.linkedin.com/pulse/%E6%80%8E%E4%B9%88%E7%9C%8B%E5%BE%85groq-boyang-zhou-tpc8c">怎 么 看待Groq</a></li>
<li><a href="https://m.elecfans.com/article/2301399.html">誉鸿锦 半 导 体 媒 体 开放日，现场见证Super IDM ...</a></li>
<li><a href="http://www.bmronline.com.cn/index.php?m=content&amp;c=index&amp;a=show&amp;catid=24&amp;id=7354">“ 半 导 体 教父”张汝京的中国“芯事”</a></li>

</ul>
</details>

**标签**: `#DRAM`, `#IPO`, `#Semiconductor`, `#China`, `#Stock Market`

---

<a id="item-9"></a>
## [Claude 共享链接遭搜索引擎索引泄露数据](https://search.brave.com/search?q=site%3Aclaude.ai%2Fshare&amp;amp;source=android) ⭐️ 8.0/10

Claude 的共享对话链接因缺少 noindex 标签，被 Google 等搜索引擎索引，泄露了 API 密钥、个人信息等敏感数据。Anthropic 尚未修复此漏洞，类似问题曾发生在 ChatGPT 上。 此隐私漏洞削弱了用户对 AI 聊天服务的信任，并将个人和组织置于严重风险中。它突显了在共享内容功能中默认启用隐私保护措施的必要性。 目前 Google 已屏蔽这些被索引的页面，但 Brave Search 和 Bing 仍在索引。建议用户进入设置中的共享对话管理页面，手动删除涉及隐私的聊天记录。

telegram · zaihuapd · 7月26日 11:16

**背景**: noindex 元标签用于指示搜索引擎不将页面编入索引。Claude 的共享链接会生成公开 URL，若缺少 noindex 标签，则可被搜索引擎爬取和索引，使内容对任何人可访问。约一年前 ChatGPT 曾出现类似漏洞并迅速修复。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Noindex">noindex - Wikipedia</a></li>
<li><a href="https://www.ibtimes.co.uk/anthropic-claude-chatbot-privacy-concerns-1810644">Claude Shared Chats Surface in Search Results... | IBTimes UK</a></li>
<li><a href="https://www.linkedin.com/posts/badalxai_claude-chat-privacy-alert-if-youve-shared-activity-7357401546793410561-1i3s">Claude.ai conversations indexed by Google. How to protect your privacy.</a></li>

</ul>
</details>

**标签**: `#Privacy`, `#Claude`, `#Security`, `#Vulnerability`, `#Search Engines`

---

<a id="item-10"></a>
## [SpaceX 拒收 Falcon 9 远期订单，全力押注 Starship](https://www.bloomberg.com/news/articles/2026-07-23/spacex-is-turning-away-falcon-customers-in-major-bet-on-starship) ⭐️ 8.0/10

SpaceX 已停止接受 2028 年后使用 Falcon 9 的独家发射请求，并削减了非可重复使用部件的生产，加速向 Starship 过渡。 这一战略转变可能扰乱商业发射市场，因为 Starship 尚未投入运营；如果 Starship 在 2028 年前无法商业化，许多卫星运营商可能面临发射能力缺口。 SpaceX 仍为美国国防部和 NASA 保留 Falcon 9 任务，但此举导致其股价自 2026 年 6 月 IPO 以来下跌约 25%。Starship 屡遭测试延误。

telegram · zaihuapd · 7月26日 12:42

**背景**: 猎鹰 9 号是 SpaceX 的主力部分可重复使用火箭，已执行数百次发射，包括商业卫星、拼单任务和载人飞行。Starship 是开发中的完全可重复使用超重型运载火箭，旨在取代猎鹰 9 号和猎鹰重型，用于月球、火星及更远的任务。Starship 仍在测试阶段，尚未投入商业运营，因此这一转型是一场高风险的赌注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/wiki/SpaceX%E6%98%9F%E8%89%A6">SpaceX星艦 - 维基百科，自由的百科全书</a></li>
<li><a href="https://en.wikipedia.org/wiki/SpaceX">SpaceX - 維基百科，自由的百科全書</a></li>

</ul>
</details>

**标签**: `#SpaceX`, `#Falcon 9`, `#Starship`, `#商业航天`, `#发射服务`

---

<a id="item-11"></a>
## [谷歌 Gemini 4：迄今最雄心预训练，预计年底发布](https://9to5google.com/2026/07/26/google-gemini-4-teases/) ⭐️ 8.0/10

谷歌 CEO Sundar Pichai 在财报会上宣布，公司已开始训练 Gemini 4，这是其最具雄心的预训练项目。该模型预计在 2026 年底（11 月或 12 月）发布。 这一宣布标志着谷歌在前沿 AI 研究上的持续重注，以及其保持在通用人工智能（AGI）竞赛中领先地位的决心。发布时，Gemini 4 可能为大型语言模型的能力设立新标杆。 目前技术细节有限，但 Pichai 强调计算资源将优先用于前沿 AGI 研发。同时，Gemini 3.x Flash 系列将保持几乎每月一次的迭代，重点提升智能编码能力。

telegram · zaihuapd · 7月27日 04:06

**背景**: 预训练是机器学习的一个阶段，模型在大规模无标签数据上进行训练，以学习通用特征和语言理解能力，然后再针对特定任务进行微调。AGI（通用人工智能）是一种假设的 AI，它能执行任何人类可以完成的智力任务。谷歌雄心勃勃的 Gemini 4 预训练项目反映了其向 AGI 迈进的努力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.csdn.net/m0_70486148/article/details/141387076">一文彻底搞懂Fine-tuning - 预 训 练 和微调（Pre-training vs Fine-tuning...</a></li>

</ul>
</details>

**标签**: `#Gemini 4`, `#Google AI`, `#LLM`, `#pretraining`, `#AI announcement`

---