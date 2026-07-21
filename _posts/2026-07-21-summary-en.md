---
layout: default
title: "Horizon Summary: 2026-07-21 (EN)"
date: 2026-07-21
lang: en
---

> From 42 items, 14 important content pieces were selected

---

1. [Critical RCE Without Gadget Found in Fastjson 1.x](#item-1) ⭐️ 9.0/10
2. [Z.AI Completes 1GW Data Center with All Domestic Chips](#item-2) ⭐️ 9.0/10
3. [Jane Street&\#x27;s Incremental library enables efficient recomputation.](#item-3) ⭐️ 8.0/10
4. [Human mathematicians are being outcounterexampled](#item-4) ⭐️ 8.0/10
5. [Agent Swarms Achieve 1,000 Commits per Second with Custom VCS](#item-5) ⭐️ 8.0/10
6. [China’s Open-Weights AI Strategy Is Winning](#item-6) ⭐️ 8.0/10
7. [Why I Stopped Creating Content](#item-7) ⭐️ 8.0/10
8. [Jellyfin founder Andrew steps down citing burnout](#item-8) ⭐️ 8.0/10
9. [Claude Code Team Reveals Internal AI Tool Adoption Metrics](#item-9) ⭐️ 8.0/10
10. [Reverse-engineering is cheap now](#item-10) ⭐️ 8.0/10
11. [Ben Thompson proposes fair use law to boost US AI models](#item-11) ⭐️ 8.0/10
12. [X Android client rebuilt from scratch for speed and stability](#item-12) ⭐️ 8.0/10
13. [Cloudflare Internal DNS Service Goes GA](#item-13) ⭐️ 8.0/10
14. [All Three Jellyfin Co-Founders Resign](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Critical RCE Without Gadget Found in Fastjson 1.x](https://x.com/k_firsov/status/2078872293745570032) ⭐️ 9.0/10

Security researcher Kirill Firsov disclosed a critical remote code execution vulnerability in Fastjson versions 1.2.68 through 1.2.83. The vulnerability does not require enabling autoType or relying on classpath gadgets and is exploitable on JDK 8, 17, and 21. This vulnerability is critical because it affects a widely-used JSON library without needing special configurations, and the Fastjson 1.x branch is end-of-life, forcing users to urgently migrate to Fastjson2 or enable SafeMode. It could impact many Java applications that rely on Fastjson for JSON processing. The vulnerability does not require the autoType feature or any classpath gadget, making it easier to exploit. Fastjson 1.x has been end-of-life since October 2024, so no official patch is expected from the maintainers.

telegram · zaihuapd · Jul 20, 14:32

**Background**: Fastjson is a popular Java library for JSON parsing and serialization developed by Alibaba. The autoType feature allows automatic type resolution during deserialization, which can be exploited if not properly secured. A &\#x27;gadget&\#x27; is a class in the classpath that can be used as part of an attack chain. This vulnerability bypasses both autoType and gadget requirements, making it especially dangerous.

<details><summary>References</summary>
<ul>
<li><a href="https://cloud.tencent.com/developer/information/fastjson+autotype">fastjson autotype - 腾讯云开发者社区 - 腾讯云</a></li>
<li><a href="https://yq1ng.github.io/2021/10/19/java-fan-xu-lie-hua-lou-dong-wu-xue-xi-di-yi-ge-gadget-urldns/">Java 反 序 列 化 漏洞(五)--学习第一个 gadget -URLDNS | 会下雪的晴天</a></li>

</ul>
</details>

**Tags**: `#fastjson`, `#rce`, `#vulnerability`, `#security`, `#json`

---

<a id="item-2"></a>
## [Z.AI Completes 1GW Data Center with All Domestic Chips](https://www.bloomberg.com/news/articles/2026-07-20/z-ai-completes-giant-data-center-with-chinese-chips-to-train-ai) ⭐️ 9.0/10

Z.AI has completed a 1-gigawatt data center powered entirely by domestically produced chips, and it has begun partial operation to support the development of its GLM platform. This milestone demonstrates the feasibility of large-scale AI training using domestic chips, marking strategic progress toward self-sufficient compute infrastructure for China&\#x27;s AI industry. The data center has a power capacity of 1 GW, enough to power about 750,000 homes. Z.AI already operates multiple clusters with over 10,000 chips each, and this new facility is one of the largest built by a Chinese AI lab.

telegram · zaihuapd · Jul 20, 15:43

**Background**: GLM \(General Language Model\) is a series of open-weight large language models developed by Z.AI, one of China&\#x27;s leading AI companies. The models power the ChatGLM chatbot and are released under permissive licenses. Building data centers with domestic chips is crucial for China&\#x27;s AI industry due to export restrictions on advanced semiconductors, and Z.AI&\#x27;s achievement shows progress in overcoming these challenges.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GLM_%28AI%29">GLM (AI)</a></li>
<li><a href="https://aishare.jizhiku.net/archives/27993">国产芯片数据中心落地：智谱的这步棋，能改变什么？ - Ai技能智慧站</a></li>
<li><a href="https://glm5.app/zh-CN">GLM 5 — 新一代前沿大模型 | AI 聊天、图像与视频生成</a></li>

</ul>
</details>

**Tags**: `#AI`, `#数据中心`, `#国产芯片`, `#智谱`, `#算力基础设施`

---

<a id="item-3"></a>
## [Jane Street&\#x27;s Incremental library enables efficient recomputation.](https://github.com/janestreet/incremental) ⭐️ 8.0/10

Jane Street has open-sourced Incremental, a library for incremental computation in OCaml that efficiently recomputes results when inputs change. Incremental computation is a key technique in reactive frameworks, build systems, and data processing; this library from Jane Street provides a robust, production-tested implementation that can influence the broader community. Incremental uses a directed acyclic graph \(DAG\) to model dependencies and recomputations, making it well-suited for functional programming patterns in OCaml.

hackernews · handfuloflight · Jul 21, 03:50 · [Discussion](https://news.ycombinator.com/item?id=48987822)

**Background**: Incremental computation is a software technique that, when input data changes, only recomputes outputs depending on the changed data, avoiding full recomputation. This approach is common in spreadsheets, build systems, and reactive programming. The Incremental library provides a principled OCaml implementation using a dependency graph to track which computations need updating.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/janestreet/incremental">GitHub - janestreet / incremental : A library for incremental ...</a></li>
<li><a href="https://blog.janestreet.com/introducing-incremental/">Jane Street Blog - Introducing Incremental</a></li>
<li><a href="https://en.wikipedia.org/wiki/Incremental_computation">Incremental computation</a></li>

</ul>
</details>

**Discussion**: Commenters compare Incremental to JavaScript signals, build systems, and differential dataflow, noting its similarity to approaches in Clojure and Goldman Sachs&\#x27;s historical practices. The discussion highlights its relevance to reactive programming and mentions alternative implementations like MobX and Jotai.

**Tags**: `#incremental-computation`, `#reactive-programming`, `#functional-programming`, `#jane-street`, `#build-systems`

---

<a id="item-4"></a>
## [Human mathematicians are being outcounterexampled](https://xenaproject.wordpress.com/2026/07/20/human-mathematicians-are-being-outcounterexampled/) ⭐️ 8.0/10

A recent blog post argues that AI systems are now better at generating counterexamples to mathematical conjectures than human mathematicians, potentially reshaping mathematical research. This trend is exemplified by new AI methods that can propose and verify counterexamples in formal theorem provers. This is significant because it can accelerate mathematical discovery by quickly refuting false conjectures, allowing mathematicians to focus on promising directions. It also raises questions about the future role of human intuition and the nature of mathematical proof. The AI systems can generate candidate counterexamples through informal reasoning and then produce formal proofs in Lean 4 for verification. However, the methods are not yet foolproof and still benefit from human oversight.

hackernews · artninja1988 · Jul 20, 19:03 · [Discussion](https://news.ycombinator.com/item?id=48983382)

**Background**: In mathematics, a counterexample is an example that disproves a conjecture. Finding counterexamples is a crucial part of mathematical research, often leading to refined conjectures. Automated theorem proving \(ATP\) has long been a field of AI, and recent advances in large language models have enabled new methods for counterexample generation. For instance, a 2026 paper introduced &\#x27;Learning to Disprove,&\#x27; using LLMs to generate counterexamples that are formally verified in the Lean theorem prover.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Automated_theorem_proving">Automated theorem proving</a></li>
<li><a href="https://arxiv.org/abs/2603.19514">[2603.19514] Learning to Disprove: Formal Counterexample Generation with Large Language Models</a></li>

</ul>
</details>

**Discussion**: The comments generally welcome the development, noting that AI counterexample generation can save mathematicians years of wasted effort, as illustrated by the anecdote of Yitang Zhang&\#x27;s thesis mistake. Some users stress the importance of counterexamples in mathematics and recommend the book &\#x27;Proofs and Refutations.&\#x27;

**Tags**: `#AI`, `#mathematics`, `#theorem proving`, `#automated reasoning`, `#counterexamples`

---

<a id="item-5"></a>
## [Agent Swarms Achieve 1,000 Commits per Second with Custom VCS](https://cursor.com/blog/agent-swarm-model-economics) ⭐️ 8.0/10

Cursor has developed agent swarms that can produce thousands of commits per second using a custom-built version control system \(VCS\), significantly exceeding the previous peak of 1,000 commits per hour on Git. This breakthrough challenges conventional assumptions about AI-assisted coding at scale, demonstrating dramatic speed improvements while raising questions about the practical value of such high-frequency commit patterns versus real-world software engineering integration. The new VCS was built from scratch to handle the throughput, and it also serves as a coordination mechanism for detecting collisions. Early results indicate that a combination of Opus and Composer can achieve comparable results to the Fable system at about 1/19th the cost and half the lines of code.

hackernews · jlaneve · Jul 20, 18:06 · [Discussion](https://news.ycombinator.com/item?id=48982535)

**Background**: Agent swarms are coordinated groups of AI agents that work together to solve complex tasks. In software engineering, they can be used to autonomously write and revise code. A custom version control system \(VCS\) is necessary to manage the extreme rate of changes generated by such swarms, as traditional Git cannot handle thousands of commits per second.

<details><summary>References</summary>
<ul>
<li><a href="https://relevanceai.com/learn/agent-swarms-orchestrating-the-future-of-ai-collaboration">What is an AI Agent Swarm - Relevance AI</a></li>

</ul>
</details>

**Discussion**: The community expressed mixed reactions. Some users praised the experimental approach as a glimpse into the future, while others criticized it as &\#x27;benchmaxxing&\#x27; that may not translate to real-world integration challenges. Notable comparisons highlighted cost efficiency differences, and questions were raised about whether the training data already contained the target source code.

**Tags**: `#agent swarms`, `#AI coding`, `#version control`, `#cost efficiency`, `#software engineering`

---

<a id="item-6"></a>
## [China’s Open-Weights AI Strategy Is Winning](https://werd.io/american-ai-is-locked-down-and-proprietary-its-losing/) ⭐️ 8.0/10

A blog post argues that China&\#x27;s open-weights AI strategy is outperforming the proprietary American approach, igniting a community debate on the validity of this claim. This debate is significant because it reflects a potential shift in the AI industry’s competitive landscape, where openness and cost efficiency may challenge the dominance of proprietary US models. The article cites statistics such as 80% of startups using Chinese models, but commenters question this figure and note enterprises prioritize zero data retention and existing vendor relationships.

hackernews · benwerd · Jul 20, 14:21 · [Discussion](https://news.ycombinator.com/item?id=48979269)

**Background**: Open-weight AI models are those whose trained parameters \(weights\) are publicly released, allowing download and use, but they may not include full training code or data. This is distinct from open-source AI, which typically provides complete access to code, data, and methodology. China has adopted an open-weights strategy for AI, releasing computationally efficient models that compete directly with US frontier models.

<details><summary>References</summary>
<ul>
<li><a href="https://opensource.org/ai/open-weights">Open Weights : not quite what you’ve been told – Open Source Initiative</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://hai.stanford.edu/policy/beyond-deepseek-chinas-diverse-open-weight-ai-ecosystem-and-its-policy-implications">Beyond DeepSeek: China&#x27;s Diverse Open-Weight AI ...</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some support the historical trend of free/open winning, citing past market disruptions, while others are skeptical of the claimed startup adoption and note that enterprises care more about data retention. There are also concerns about intellectual property violations and the fact that Meta&\#x27;s Llama has not led to commercial success for Meta.

**Tags**: `#AI`, `#open-weights`, `#China`, `#AI strategy`, `#open-source`

---

<a id="item-7"></a>
## [Why I Stopped Creating Content](https://refactoringenglish.com/blog/why-i-stopped-creating-content/) ⭐️ 8.0/10

The author of Refactoring English explains why they reject the label &\#x27;content creator&\#x27; and instead focus on producing meaningful work such as essays, focusing on quality over algorithmic performance. This article challenges the pervasive &\#x27;content creation&\#x27; mindset in digital media, encouraging creators to think beyond metrics and commodification, and to value genuine craftsmanship and human connection. The term &\#x27;content&\#x27; reduces creative works to interchangeable commodities, a stance previously echoed by Richard Stallman. The author distinguishes between creating &\#x27;content&\#x27; for algorithms and creating &\#x27;works&\#x27; for an audience.

hackernews · mtlynch · Jul 20, 15:47 · [Discussion](https://news.ycombinator.com/item?id=48980520)

**Background**: In recent years, the term &\#x27;content creator&\#x27; has become ubiquitous on platforms like YouTube, TikTok, and Instagram, often implying a focus on engagement metrics and monetization. Critics argue that it devalues artistic and intellectual work by framing it as filler for distribution channels.

**Discussion**: Commenters express mixed reactions: some agree that &\#x27;content&\#x27; trivializes creative work, drawing on Stallman&\#x27;s similar critique; others defend the term as a neutral description that removes artificial boundaries between mediums. One commenter notes that Seth Godin frames sharing ideas as a privilege rather than commodity creation.

**Tags**: `#content creation`, `#writing`, `#digital media`, `#philosophy`, `#Hacker News discussion`

---

<a id="item-8"></a>
## [Jellyfin founder Andrew steps down citing burnout](https://forum.jellyfin.org/t-project-leadership-changes) ⭐️ 8.0/10

Jellyfin founder Andrew has left the project due to severe burnout, as announced in a forum post. The transition appears peaceful, with the project continuing under other maintainers. Andrew&\#x27;s departure highlights the sustainability challenges of free and open-source software \(FLOSS\), especially volunteer-driven projects like Jellyfin that compete with proprietary giants like Plex. This event also sparks community reflection on the importance of maintainer well-being and the need for more contributors to share the workload. Andrew mentioned in the announcement that he could no longer provide the effort required and faced severe burnout and risks to his mental health. The project is expected to continue under existing maintainers, with a &\#x27;peaceful transition&\#x27; as per the post.

hackernews · swat535 · Jul 20, 23:15 · [Discussion](https://news.ycombinator.com/item?id=48986091)

**Background**: Jellyfin is a free and open-source media server that allows users to host and stream their own media libraries to any device. It emerged as a fork of Emby in 2018 and has become a popular alternative to proprietary solutions like Plex. The project is entirely volunteer-run, relying on community contributions for development and maintenance.

<details><summary>References</summary>
<ul>
<li><a href="https://jellyfin.org/">The Free Software Media System | Jellyfin</a></li>
<li><a href="https://jellyfin.org/docs/">Introduction | Jellyfin</a></li>

</ul>
</details>

**Discussion**: Comments show strong support for Andrew and appreciation for his work. Users thank the team for offering an alternative to Plex, especially after Plex raised its lifetime pass price to $750. Some commenters note that they&\#x27;ve used Jellyfin for years without issues, while others still rely on Plex due to hardware compatibility but acknowledge Jellyfin&\#x27;s progress. A discussion also emerged about burnout in FLOSS projects, with users referencing other recent cases like Filebrowser.

**Tags**: `#Jellyfin`, `#open-source`, `#leadership change`, `#media server`, `#burnout`

---

<a id="item-9"></a>
## [Claude Code Team Reveals Internal AI Tool Adoption Metrics](https://simonwillison.net/2026/Jul/21/cat-and-thariq/#atom-everything) ⭐️ 8.0/10

In a fireside chat, Anthropic&\#x27;s Claude Code team revealed that their Slack-based tool Claude Tag now drives 65% of their product engineering pull requests. They also disclosed that features are first shipped to employees and only retained if they demonstrate positive user retention. These metrics demonstrate the high level of trust and integration of AI coding tools within the team that builds them, providing strong validation of their effectiveness. The development practices, such as employee dogfooding and automated code review, offer valuable lessons for the broader software engineering community on integrating AI assistants. The Claude Code team increasingly uses automated code review for outer product layers but still manually reviews critical changes. Additionally, the team noted that adding examples to system prompts is no longer best practice for newer models, and their system prompt was reduced in size by 80%.

rss · Simon Willison · Jul 21, 12:54

**Background**: Claude Code is an AI-powered coding assistant from Anthropic, and Claude Tag is a Slack integration that allows teams to collaborate with the AI in channels. Anthropic also recently released Fable, a powerful model for ambitious coding projects that can handle multi-day autonomous sessions. The team practices &\#x27;dogfooding&\#x27; \(internally called &\#x27;ant fooding&\#x27;\) by using their own tools extensively before public release.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_%28AI%29">Claude (AI)</a></li>
<li><a href="https://claude.com/docs/claude-tag/overview">Work with Claude Tag - Claude .ai Documentation</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#AI coding tools`, `#Claude Code`, `#Anthropic`, `#software engineering`, `#developer productivity`

---

<a id="item-10"></a>
## [Reverse-engineering is cheap now](https://simonwillison.net/2026/Jul/20/cheap-reverse-engineering/#atom-everything) ⭐️ 8.0/10

AI coding agents have drastically reduced the cost and psychological commitment of reverse-engineering home devices, making it feasible for hobbyists to automate devices that were previously not worth the effort. This lowers the barrier for hobbyists to experiment with reverse-engineering, altering the cost-benefit analysis and encouraging more innovation in home automation and device interoperability. Reverse-engineering home devices often involves dealing with undocumented and unstable APIs that may change, requiring ongoing maintenance. Coding agents reduce the initial effort and the psychological baggage of maintenance, as code can be cheaply rewritten if it breaks.

rss · Simon Willison · Jul 20, 19:24

**Background**: AI coding agents are tools that use large language models to automatically generate or modify code based on natural language prompts. Examples include Cursor and Zencoder. They have become increasingly capable, allowing developers to quickly prototype automations and reverse-engineer protocols with minimal manual effort. This reduces the cost of experimentation and makes previously marginal projects viable.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/Hybrid_Mac_mini_and_RTX_4090_setup_for_local_AI_coding_agents">Hybrid Mac mini and RTX 4090 setup for local AI coding agents</a></li>
<li><a href="https://zencoder.ai/">Zencoder | The AI Coding Agent</a></li>
<li><a href="https://cursor.com/">Cursor: AI coding agent</a></li>

</ul>
</details>

**Tags**: `#reverse-engineering`, `#AI coding agents`, `#software engineering`, `#automation`, `#cost of code`

---

<a id="item-11"></a>
## [Ben Thompson proposes fair use law to boost US AI models](https://simonwillison.net/2026/Jul/20/afraid-of-chinese-models/#atom-everything) ⭐️ 8.0/10

Ben Thompson proposed a U.S. law to explicitly make collecting data for AI training fair use and to prohibit terms of service that forbid model distillation. Meanwhile, Alibaba released Qwen 3.8 Max, a 2.4 trillion parameter open-weights model, following a speech by Xi Jinping encouraging openness. The proposal could significantly reshape U.S.-China AI competition by clarifying copyright law and enabling U.S. open models to leverage distillation from proprietary models. It also highlights the tension between training on unlicensed data and banning distillation of one&\#x27;s own model. The proposed law would explicitly make training data collection fair use and bar terms of service that prohibit distillation. Qwen 3.8 Max has 2.4 trillion parameters, almost as large as Kimi K3&\#x27;s 2.8 trillion, and its reasoning trace included human-like deliberation such as &\#x27;Could add helmet? No.&\#x27;

rss · Simon Willison · Jul 20, 17:09

**Background**: Model distillation is a technique where a smaller &\#x27;student&\#x27; model learns to mimic a larger &\#x27;teacher&\#x27; model by querying its API. Fair use for AI training data is a legal concept that using copyrighted works for training may be permissible. Open weights models release the final trained weights publicly, allowing anyone to download and use them. Ben Thompson&\#x27;s proposal aims to clarify these legal ambiguities to help U.S. open models compete with Chinese counterparts.

<details><summary>References</summary>
<ul>
<li><a href="https://avahi.ai/glossary/model-distillation/">What is Model Distillation in AI ?</a></li>
<li><a href="https://www.forbes.com/sites/roomykhan/2024/10/04/ai-training-data-dilemma-legal-experts-argue-for-fair-use/">AI Training Data Dilemma: Legal Experts Argue For &#x27;Fair Use&#x27;</a></li>
<li><a href="https://www.analyticsvidhya.com/blog/2025/04/open-weight-models/">What are Open Source and Open Weight Models ? | Analytics Vidhya</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#open models`, `#distillation`, `#fair use`, `#Chinese AI`

---

<a id="item-12"></a>
## [X Android client rebuilt from scratch for speed and stability](https://x.com/i/status/2079273272274026718) ⭐️ 8.0/10

X&\#x27;s product lead Nikita Bier announced that the Android client has been completely rebuilt from scratch, a project that took over a year. The new version is faster, smoother, and more stable, laying the groundwork for rapid feature iteration. This rebuild demonstrates X&\#x27;s commitment to improving the Android experience, which has often lagged behind iOS. It will enable faster rollout of new features like Cashtags and custom timelines, and could attract more users to the platform. The rebuild addresses performance on older devices and still lacks some features like Spaces hosting, but Cashtags and custom timelines are already available. Video responses and a video editor are coming soon.

telegram · zaihuapd · Jul 21, 02:27

**Background**: Cashtags are a feature that embeds real-time price charts for stocks and cryptocurrencies into posts. Custom timelines allow users to create personalized feeds based on topics, keywords, or lists. Spaces is X&\#x27;s live audio chat feature.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/elon-musks-x-launches-cashtags-150207451.html">Elon Musk&#x27;s X Launches Cashtags Feature As It Aims To Bring &#x27;Real-Time Financial Data&#x27; To Platform: Here&#x27;s How It Will Work</a></li>
<li><a href="https://www.ibtimes.co.uk/x-custom-timelines-personalised-user-experience-1793037">X &#x27; Custom Timelines &#x27; Explained: Here&#x27;s How to Build... | IBTimes ...</a></li>
<li><a href="https://help.x.com/en/using-x/spaces">Spaces is a place to come together, built around the voices of the...</a></li>

</ul>
</details>

**Tags**: `#Android`, `#X \(Twitter\)`, `#app rewrite`, `#engineering`, `#performance`

---

<a id="item-13"></a>
## [Cloudflare Internal DNS Service Goes GA](https://blog.cloudflare.com/internal-dns/) ⭐️ 8.0/10

On July 20, 2026, Cloudflare announced the general availability of its Internal DNS service, which provides authoritative and recursive DNS resolution for private networks integrated with public DNS and Zero Trust. This simplifies enterprise split-horizon DNS management by unifying public and private DNS on a single platform, reducing configuration drift and extending Zero Trust policies to DNS resolution. Existing Cloudflare Gateway customers can enable Internal DNS at no additional cost; administrators can define resolver policies and use DNS views to control which internal records different users and devices see.

telegram · zaihuapd · Jul 21, 03:49

**Background**: Split-horizon DNS allows organizations to serve different DNS responses based on the source of the query, typically separating internal and external names. Cloudflare&\#x27;s Internal DNS integrates this capability with its Zero Trust network, enabling a unified control plane without the need for separate DNS infrastructure.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Split-horizon_DNS">Split-horizon DNS</a></li>
<li><a href="https://developers.cloudflare.com/dns/internal-dns/dns-views/">Manage DNS views · Cloudflare DNS docs</a></li>

</ul>
</details>

**Tags**: `#Cloudflare`, `#DNS`, `#Zero Trust`, `#Networking`, `#Enterprise`

---

<a id="item-14"></a>
## [All Three Jellyfin Co-Founders Resign](https://cybernews.com/tech/jellyfin-founders-step-down-future-uncertain/) ⭐️ 8.0/10

The three co-founders of Jellyfin have all stepped down within one week, citing burnout, mental health risks, and development direction disagreements. The project&\#x27;s future is uncertain as no succession plan has been announced. This leadership vacuum could destabilize Jellyfin, a widely used open-source media server, and affect its community and development pace. It also highlights the burnout challenges faced by volunteer-driven open-source projects. Despite the departures, former co-founder Joshua Boniface stated the handover is friendly and a malicious fork is unlikely. The team had previously complained in May that AI code submissions were exacerbating development burnout.

telegram · zaihuapd · Jul 21, 11:06

**Background**: Jellyfin is a free and open-source media server forked from Emby in 2018 after Emby became closed-source. It allows users to organize, manage, and stream personal media to various devices. Open-source projects often rely on volunteer maintainers, which can lead to burnout when demands exceed capacity.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Jellyfin">Jellyfin</a></li>
<li><a href="https://jellyfin.org/">The Free Software Media System | Jellyfin</a></li>

</ul>
</details>

**Tags**: `#Jellyfin`, `#open source`, `#media server`, `#co-founder departure`, `#community impact`

---