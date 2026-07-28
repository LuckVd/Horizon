---
layout: default
title: "Horizon Summary: 2026-07-28 (ZH)"
date: 2026-07-28
lang: zh
---

> 从 27 条内容中筛选出 8 条重要资讯。

---

1. [月之暗面发布 2.8 万亿参数开源模型 Kimi K3](#item-1) ⭐️ 9.0/10
2. [中国开始量产国产 DUV 光刻机](#item-2) ⭐️ 9.0/10
3. [Anthropic 阐述对开放权重模型的担忧与建议](#item-3) ⭐️ 8.0/10
4. [缺失下划线导致无辜者被误判入狱 18 个月](#item-4) ⭐️ 8.0/10
5. [Paged Out \#9：免费技术杂志获社区好评](#item-5) ⭐️ 8.0/10
6. [前沿 LLM 偏见评估：所有模型偏左，但 Grok 自称偏右](#item-6) ⭐️ 8.0/10
7. [Fastjson2 远程代码执行漏洞影响所有版本，尚无补丁](#item-7) ⭐️ 8.0/10
8. [中国兴起 AI 人脸租赁市场 一季度超 95%微短剧使用 AI](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [月之暗面发布 2.8 万亿参数开源模型 Kimi K3](https://simonwillison.net/2026/Jul/27/kimi-k3/#atom-everything) ⭐️ 9.0/10

月之暗面在 Hugging Face 上发布了 Kimi K3 的模型权重，这是一个 2.8 万亿参数的开源权重模型，采用修改后的 MIT 许可证。 这是一个重要的里程碑，因为它是首个公开可用的 3 万亿参数级别模型，标志着大规模 AI 的进展，可能推进长上下文理解和智能体任务的能力。 该模型采用 MoE 架构，拥有 896 个专家，每个 token 激活 16 个，支持 100 万 token 的上下文窗口和多模态输入（文本、图像、视频）。K3 许可证要求大型模型即服务提供商与月之暗面签署单独协议。

rss · Simon Willison · 7月27日 23:39

**背景**: 模型权重是定义已训练 AI 模型行为的数值参数。月之暗面之前的 K2 模型使用了修改的 MIT 许可证，要求大型商业实体注明出处。K3 进一步扩展了限制，对大型 MaaS 业务有额外要求。使用混合专家（MoE）架构可以实现高效的参数扩展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ultralytics.com/glossary/model-weights">What are Model Weights in AI? | Ultralytics</a></li>
<li><a href="https://moclaw.ai/blog/kimi-k3-license">Kimi K3 License : Modified MIT &amp; Commercial Use | MoClaw Blog</a></li>

</ul>
</details>

**标签**: `#AI`, `#LLM`, `#Kimi-K3`, `#Moonshot`, `#open-source`

---

<a id="item-2"></a>
## [中国开始量产国产 DUV 光刻机](https://www.theinformation.com/articles/china-starts-mass-producing-homegrown-duv-chipmaking-tools-advance-local-chip-industry) ⭐️ 9.0/10

中国已开始大规模生产自主研发的浸没式 DUV 光刻机，计划今年生产约 5 台，2027 年约 20 台，将交付中芯国际、华虹半导体等国内厂商。 这标志着中国半导体自主化的重大突破，可能影响全球芯片供应链和 ASML 的市场地位，尤其是在西方进一步收紧出口限制的情况下。 据报道，该设备主要使用国产零部件，但部分关键部件仍来自日本。性能和可靠性落后于 ASML 的设备，芯片商需数月测试才能投入量产。

telegram · zaihuapd · 7月27日 14:10

**背景**: DUV（深紫外）光刻是制造先进芯片的关键技术。浸没式光刻通过在透镜与硅片之间填充液体介质来提高分辨率，实现更小制程。ASML 是全球主要供应商，但由于出口管制，中国一直在推动开发国产替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.zaobao.com.sg/news/china/story20260727-9428899">美媒：中国开始生产 DUV 光 刻 机 年内交付 | 联合早报</a></li>
<li><a href="https://zh.wikipedia.org/zh-hans/%E6%B5%B8%E6%B2%A1%E5%85%89%E5%88%BB">浸没光刻 - 维基百科，自由的百科全书 - zh.wikipedia.org</a></li>

</ul>
</details>

**标签**: `#光刻机`, `#半导体`, `#中国芯片`, `#DUV`, `#ASML`

---

<a id="item-3"></a>
## [Anthropic 阐述对开放权重模型的担忧与建议](https://www.anthropic.com/news/position-open-weights-models) ⭐️ 8.0/10

Anthropic 发布了一份关于开放权重 AI 模型的政策声明，表达了对潜在滥用的担忧，并主张采取出口管制和其他监管措施来降低风险。 作为一家主要 AI 公司，Anthropic 的立场可能影响关于平衡 AI 开放性与安全性的行业和监管讨论，进而影响开放权重模型的开发和分发。 该声明据报包括支持对中国的 AI 芯片出口管制和其他措施，以解决安全问题，但不主张完全禁止开放权重模型。

hackernews · surprisetalk · 7月27日 22:03 · [社区讨论](https://news.ycombinator.com/item?id=49076057)

**背景**: 开放权重模型是指其训练后的参数被公开发布的 AI 模型，允许他人本地运行，但不一定允许自由修改或再分发。这不同于通常提供完整源代码和训练数据的开源模型。争议的核心在于广泛发布强大 AI 模型是否可能导致滥用（如用于生物武器或网络攻击），这与透明度及创新的好处之间的权衡。对 AI 技术（包括芯片和模型）的出口管制是政府用于限制对手国家获取先进 AI 的一种工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/emollick_a-lot-of-discussion-on-open-weights-ai-models-activity-7404665589538902016-2qJU">A lot of discussion on open weights AI models seems to assume there is a clear incentive for building them. | Ethan Mollick - LinkedIn</a></li>
<li><a href="https://www.sipri.org/commentary/topical-backgrounder/2026/regulating-transfers-ai-algorithms-training-data-and-models-potential-and-limitations-export">Regulating transfers of AI algorithms, training data and models: The potential and limitations of export controls | SIPRI</a></li>
<li><a href="https://www.wilmerhale.com/en/insights/publications/20250205-bis-issues-long-awaited-export-controls-on-ai">BIS Issues Long Awaited Export Controls on AI</a></li>

</ul>
</details>

**社区讨论**: 社区评论普遍持批评态度，指责 Anthropic 在主张出口管制的同时受益于封闭模型，是虚伪的，并认为此类措施可能无效或自私。一些评论者还质疑 Anthropic 在对待中国和安全问题上的立场一致性。

**标签**: `#AI safety`, `#open source`, `#Anthropic`, `#open-weights`, `#policy`

---

<a id="item-4"></a>
## [缺失下划线导致无辜者被误判入狱 18 个月](https://arstechnica.com/tech-policy/2026/07/police-missed-one-underscore-and-sent-the-wrong-man-to-prison/) ⭐️ 8.0/10

一个 Kik 用户名中缺失的下划线导致一名无辜男子被错误定罪，他在狱中服刑 18 个月后才发现错误并推翻定罪。 此案凸显了数字取证中微小数据错误的严重后果，强调了在涉及数字证据的法律程序中需进行严格核查的必要性。 警方传唤 Kik 要求提供用户&quot;fus\_ro\_dah&quot;的信息，但无意中漏掉了一个下划线，从而获得了&quot;fusro\_dah&quot;的信息。尽管缺乏将 Klayme 与该犯罪直接联系的证据，他仍被定罪并监禁。

hackernews · quantified · 7月27日 22:10 · [社区讨论](https://news.ycombinator.com/item?id=49076116)

**背景**: 数字取证涉及分析电子数据以调查犯罪。在此案中，传票中的一个小打印错误导致执法部门追查了错误的人。该事件暴露了仅依赖数字标识符而缺乏佐证证据的危险性。

**社区讨论**: 评论者对所暴露的系统性失败表示愤怒，指出辩护律师未能对控方证据提出质疑。一些人质疑这位被错误定罪的男子缺乏赔偿，尽管定罪被撤销，他仍遭受了声誉损害和收入损失。

**标签**: `#digital forensics`, `#wrongful conviction`, `#legal system`, `#data accuracy`, `#privacy`

---

<a id="item-5"></a>
## [Paged Out \#9：免费技术杂志获社区好评](https://pagedout.institute/download/PagedOut_009.pdf) ⭐️ 8.0/10

Paged Out \#9 是一本免费的实验性技术杂志，每篇文章严格限制在一页，已发布并获得了 Hacker News 社区的高度赞扬。 该杂志复兴了 2600 和 Phrack 等经典黑客杂志的精神，提供了涵盖多种主题的深度技术内容，设计精美，吸引了现代程序员和黑客群体。 每篇文章限制在一页，涵盖编程技巧、安全、复古计算机和演示场景等主题。该杂志免费下载，也提供付费印刷版。

hackernews · laurensr · 7月27日 14:22 · [社区讨论](https://news.ycombinator.com/item?id=49070138)

**背景**: Paged Out\! 是由 gynvael（Gynvael Coldwind）创办的一本免费实验性杂志，每篇文章严格限制在一页。内容涵盖编程、黑客、安全、复古计算机、现代计算机、电子、演示场景等类似主题。该杂志旨在以简洁的形式提供深度技术内容，令人联想到传统黑客杂志。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pagedout.institute/">Paged Out!</a></li>
<li><a href="https://gynvael.coldwind.pl/?id=707">Introducing Paged Out! magazine (also CFP) - gynvael.coldwind//vx.log</a></li>

</ul>
</details>

**社区讨论**: Hacker News 社区反响非常积极，评论称赞了杂志的技术深度和精美设计。具体文章如《Baby Steps in C》和《The Subpixel Zoo》受到关注，并与 2600 和 Phrack 等经典杂志进行了比较。有评论指出，《computiles》部分是对 1960 年代 Wang 作品的无意重新发现，将多米诺问题与停机问题联系起来。

**标签**: `#magazine`, `#technical`, `#hacker-culture`, `#programming`, `#low-level`

---

<a id="item-6"></a>
## [前沿 LLM 偏见评估：所有模型偏左，但 Grok 自称偏右](https://www.reddit.com/r/MachineLearning/comments/1v8fnzw/evaluated_6_frontier_llms_gpt54_claude_sonnet_46/) ⭐️ 8.0/10

一项对六款前沿 LLM（GPT-5.4、Claude Sonnet 4.6、Claude Opus 4.7、Gemini Pro/Flash、Grok 4.3）在八个偏见基准（约 20,600 个样本）上的独立评估发现，所有模型都表现出左倾政治偏见，包括自称右倾的 Grok。此外，GPT-5.4 在 BBQ 数据集的种族相关问题上有 20.3%的拒绝率。 这项评估为最先进 LLM 中的政治和种族偏见提供了重要的（尽管未经同行评审）经验证据，挑战了 Grok 声称的政治中立性。研究结果强调了更透明的偏见审计的必要性，并引发了对模型在敏感话题上拒绝行为的质疑。 该研究使用了包括 WinoBias、BBQ 种族/民族偏见、SeeGULL、OpinionsQA、cajcodes 政治偏见、Hyperpartisan 新闻和政治坐标在内的八个基准。局限性包括每项任务仅使用单一提示模板且未进行多次运行平均，这可能影响可靠性。

reddit · r/MachineLearning · /u/marggggggggg · 7月27日 22:37

**背景**: WinoBias 和 BBQ 等偏见基准旨在评估语言模型中的社会偏见。WinoBias 侧重于指代消解中的性别偏见，而 BBQ（问答偏见基准）测试跨多个社会维度的偏见。SeeGULL 是一个覆盖多个国家身份群体的广泛刻板印象数据集。这些基准帮助研究人员衡量 NLP 系统中的意外偏见。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/winobias">WinoBias : Gender Bias in Coreference Benchmark</a></li>
<li><a href="https://arxiv.org/abs/2110.08193">[2110.08193] BBQ: A Hand-Built Bias Benchmark for Question Answering</a></li>
<li><a href="https://github.com/google-research-datasets/seegull">GitHub - google-research-datasets/seegull: SeeGULL is a broad-coverage stereotype dataset in English containing stereotypes about identity groups spanning 178 countries across 8 different geo-political regions across 6 continents, as well as state-level identities within the US and India. · GitHub</a></li>

</ul>
</details>

**标签**: `#LLM bias`, `#AI fairness`, `#frontier models`, `#political bias`, `#racial bias`

---

<a id="item-7"></a>
## [Fastjson2 远程代码执行漏洞影响所有版本，尚无补丁](https://mp.weixin.qq.com/s/LJaul1jNjK9pXRAkoUiMEA) ⭐️ 8.0/10

7 月 27 日，长亭科技披露 Fastjson2 存在远程代码执行漏洞，攻击者可通过恶意 JSON 数据绕过 AutoType 类型校验执行代码。该漏洞影响 2.0.62 及之前所有版本，目前尚无官方补丁。 Fastjson2 是 Java 项目中广泛使用的 JSON 库，此未修复的 RCE 漏洞对依赖该库的应用程序构成严重安全风险。在修复版发布前，强烈建议用户禁用 AutoType。 项目维护者已确认问题，但 PR \#7695 已关闭且未合入主分支，因此已发布版本均无修复。完整漏洞细节和利用代码尚未公开。

telegram · zaihuapd · 7月27日 10:31

**背景**: Fastjson2 是 Java 的高性能 JSON 库，广泛用于序列化和反序列化。AutoType 是一个允许多态类型反序列化的功能，但如果保护不当，可能被攻击者利用。远程代码执行（RCE）漏洞使攻击者能在目标系统上运行任意代码，可能导致完全控制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://alibaba.github.io/fastjson2/">FASTJSON 2 is a Java JSON library with excellent performance.</a></li>
<li><a href="https://blog.csdn.net/2402_84408069/article/details/149468874">远程代码执行漏洞（RCE）解析：原理、利用与防御-CSDN博客</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#rce`, `#fastjson2`, `#java`

---

<a id="item-8"></a>
## [中国兴起 AI 人脸租赁市场 一季度超 95%微短剧使用 AI](https://restofworld.org/2026/china-ai-microdramas-face-licensing/) ⭐️ 8.0/10

中国兴起了一个新的人脸租赁市场，平台向用户支付 15 至 700 美元以获取其肖像在 AI 生成内容中的使用权。2026 年第一季度，内地发布的约 12.8 万部微短剧中超过 95%使用了 AI 制作。 这一趋势凸显了 AI 在内容创作中的大规模整合，尤其是在微短剧行业，并引发了关于人脸权和未经授权使用的紧急法律和伦理问题。AI 相关肖像纠纷的激增可能重塑关于数字肖像和知识产权的法规。 深圳平台 ActID 自 2026 年 3 月上线以来已注册约 800 名用户，约 300 人同意授权，每集收费 99 至 500 元，平台抽成 10%。字节跳动自 2026 年初以来已下架超过 8.5 万个未经授权的 AI 复刻人脸及声音视频，广州互联网法院近三年已审理约 700 起相关案件。

telegram · zaihuapd · 7月28日 03:03

**背景**: 微短剧是一种流行的中国互联网视频格式，特点是单集极短（通常 1-3 分钟）且制作周期快。AI 人脸租赁市场允许个人通过将人脸租给 AI 内容制作方来获利，但也催生了未经同意的深度伪造等滥用行为，从而引发诉讼浪潮。

**标签**: `#AI`, `#微短剧`, `#人脸租赁`, `#肖像权`, `#内容生成`

---