---
layout: default
title: "Horizon Summary: 2026-07-21 (EN)"
date: 2026-07-21
lang: en
---

> From 41 items, 9 important content pieces were selected

---

1. [Incremental: OCaml Library for Incremental Computations](#item-1) ⭐️ 8.0/10
2. [AI Outpaces Mathematicians in Generating Counterexamples](#item-2) ⭐️ 8.0/10
3. [Agent Swarms Hit 1,000 Commits/s, Require Custom VCS](#item-3) ⭐️ 8.0/10
4. [Claude Code Team Reveals Internal Metrics in Fireside Chat](#item-4) ⭐️ 8.0/10
5. [Ben Thompson Proposes US Law to Boost Open Models Against Chinese AI](#item-5) ⭐️ 8.0/10
6. [Z.ai Completes Giant Data Center with Chinese Chips](#item-6) ⭐️ 8.0/10
7. [Google&\#x27;s Frozen v2 Chip Hardwires Gemini AI for 6-10x Efficiency](#item-7) ⭐️ 8.0/10
8. [Alibaba to Launch Qianwen Office, Integrating Three AI Agents](#item-8) ⭐️ 8.0/10
9. [Google releases Gemini 3.6 Flash, starts Gemini 4 pre-training](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Incremental: OCaml Library for Incremental Computations](https://github.com/janestreet/incremental) ⭐️ 8.0/10

Jane Street has released Incremental, an OCaml library that enables efficient partial re-evaluation of computation graphs when input data changes. This library brings incremental computation to OCaml, improving performance in applications like spreadsheet recalculation, UI updates, and derived data synchronization, connecting with broader trends in reactive programming and build systems. Incremental is built on self-adjusting computation research and supports use cases such as spreadsheet-style calculations and GUI view updates; it is also used by Jane Street&\#x27;s Bonsai UI library.

hackernews · handfuloflight · Jul 21, 03:50 · [Discussion](https://news.ycombinator.com/item?id=48987822)

**Background**: Incremental computation is a technique that saves time by recomputing only outputs that depend on changed data, commonly used in spreadsheets and build systems. The Incremental library implements this in OCaml, inspired by self-adjusting computation research.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Incremental_computation">Incremental computation</a></li>
<li><a href="https://github.com/janestreet/incremental">GitHub - janestreet/incremental: A library for incremental ...</a></li>

</ul>
</details>

**Discussion**: Commenters noted the similarity of Incremental to reactive programming signals in JavaScript frameworks and compared it to build systems and differential dataflow systems like Materialize. One commenter mentioned a similar approach used by Goldman Sachs for instrument pricing. The discussion was positive and insightful, highlighting various applications and connections.

**Tags**: `#incremental computation`, `#reactive programming`, `#OCaml`, `#janestreet`, `#signals`

---

<a id="item-2"></a>
## [AI Outpaces Mathematicians in Generating Counterexamples](https://xenaproject.wordpress.com/2026/07/20/human-mathematicians-are-being-outcounterexampled/) ⭐️ 8.0/10

AI systems now generate 97% of counterexamples in mathematics, surpassing human mathematicians and transforming research practices. This shift allows mathematicians to quickly disprove false conjectures, saving time and focusing efforts on proving true statements. It also reassigns the role of human intuition in mathematical discovery. Techniques involve reformulating conjectures as optimization or search tasks for AI, using machine learning and computational search to explore vast possibility spaces.

hackernews · artninja1988 · Jul 20, 19:03 · [Discussion](https://news.ycombinator.com/item?id=48983382)

**Background**: Counterexamples are specific instances that disprove a conjecture, playing a crucial role in refining definitions and sharpening proofs. Automated theorem proving has been a long-standing goal in computer science, but recent advances in AI and machine learning have significantly accelerated the discovery of counterexamples.

<details><summary>References</summary>
<ul>
<li><a href="https://math.duke.edu/mathplus/2025/ai-powered-discovery-counterexamples-combinatorics">AI powered discovery of counterexamples in combinatorics</a></li>
<li><a href="https://www.youtube.com/watch?v=vxeSjfwJQRE">97% of Counterexamples Are Now AI-Generated! - YouTube Images</a></li>
<li><a href="https://en.wikipedia.org/wiki/Automated_theorem_proving">Automated theorem proving</a></li>

</ul>
</details>

**Discussion**: Commenters generally view the trend positively, noting it saves time wasted on false conjectures and allows mathematicians to focus on fruitful research. Some draw parallels to chess computers, which initially excelled at calculation but later inspired creative moves. A reference to the Jacobian conjecture illustrates the human cost of undetected errors.

**Tags**: `#mathematics`, `#AI`, `#theorem proving`, `#counterexamples`, `#research methodology`

---

<a id="item-3"></a>
## [Agent Swarms Hit 1,000 Commits/s, Require Custom VCS](https://cursor.com/blog/agent-swarm-model-economics) ⭐️ 8.0/10

Cursor&\#x27;s blog reports experiments with agent swarms that achieve commit rates of up to 1,000 per second, necessitating a purpose-built version control system \(VCS\) to manage the throughput and coordination. This demonstrates the extreme scaling potential of AI agents while revealing infrastructure bottlenecks like VCS that must be overcome for real-world use, sparking community debate about the validity of such benchmarks. The new system peaks at 1,000 commits per second, a thousand-fold increase over the prior browser swarm&\#x27;s 1,000 commits per hour. The custom VCS was built from scratch to handle collision detection and coordination at high speed.

hackernews · jlaneve · Jul 20, 18:06 · [Discussion](https://news.ycombinator.com/item?id=48982535)

**Background**: Agent swarms coordinate multiple AI agents to work in parallel on complex tasks. Traditional version control systems like Git are not designed for the high commit rates and autonomous coordination needs of such swarms. Cursor&\#x27;s experiment pushes the limits of agent swarm capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.swarms.ai/">Swarms AI — Multi- Agent Framework &amp; Agent Marketplace</a></li>
<li><a href="https://www.freestyle.sh/blog/engineering/version-control-for-ai-agents">Version Control for AI Agents - Freestyle Blog</a></li>

</ul>
</details>

**Discussion**: Commenters like anthonypasq appreciate the forward-looking nature, while notahan dismisses the results as &\#x27;benchmaxxing&\#x27; and questions real-world applicability. Handfuloflight notes that SQLite source code may have been in the training data, casting doubt on test validity.

**Tags**: `#agent swarms`, `#AI`, `#version control`, `#software engineering`, `#benchmarking`

---

<a id="item-4"></a>
## [Claude Code Team Reveals Internal Metrics in Fireside Chat](https://simonwillison.net/2026/Jul/21/cat-and-thariq/#atom-everything) ⭐️ 8.0/10

In a fireside chat at AI Engineer World&\#x27;s Fair, Cat Wu and Thariq Shihipar from Anthropic&\#x27;s Claude Code team disclosed that Claude Tag now handles 65% of their product engineering pull requests and that the Claude Code system prompt was reduced by 80% due to newer models like Fable 5. This demonstrates high internal trust and adoption of AI coding agents at Anthropic, and the shift in best practices \(fewer examples and explicit prohibitions in prompts\) signals how models have matured, impacting developers using Claude Code and similar tools. Claude Tag is a collaborative Slack integration that relies on auto mode; Anthropic calls internal dogfooding &\#x27;ant fooding&\#x27;; Fable was used to edit its own launch video; Thariq advises developers to become more ambitious to offset productivity gains from coding agents.

rss · Simon Willison · Jul 21, 12:54

**Background**: Claude Code is Anthropic&\#x27;s AI-powered coding agent that assists developers in writing code. Claude Tag is a collaborative integration that allows teams to work with Claude in Slack channels. Fable 5, released in June 2026, is Anthropic&\#x27;s most capable model for ambitious coding projects. This fireside chat provided insider perspectives on how the team uses its own products.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_%28AI%29">Claude (AI)</a></li>
<li><a href="https://www.anthropic.com/news/introducing-claude-tag">Introducing Claude Tag \ Anthropic</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#Claude Code`, `#AI coding agents`, `#Anthropic`, `#developer tools`, `#productivity`

---

<a id="item-5"></a>
## [Ben Thompson Proposes US Law to Boost Open Models Against Chinese AI](https://simonwillison.net/2026/Jul/20/afraid-of-chinese-models/#atom-everything) ⭐️ 8.0/10

Ben Thompson proposes that the U.S. should pass a law making training data collection fair use and barring terms of service that prohibit distillation, to help American open models compete with Chinese models like Qwen 3.8 Max. This proposal directly addresses the hypocrisy of AI labs that train on unlicensed data while banning distillation, and could shift U.S. copyright policy to favor openness and accelerate AI innovation. The proposal includes two pillars: explicit fair use for training data and a ban on anti-distillation ToS clauses. Ben Thompson also notes that Alibaba&\#x27;s release of Qwen 3.8 Max with open weights may have been influenced by Xi Jinping&\#x27;s call for open source collaboration.

rss · Simon Willison · Jul 20, 17:09

**Background**: AI distillation is a technique where a smaller model learns from a larger model&\#x27;s outputs, often via API queries. The legal status of using copyrighted data for training is ambiguous; some courts have found it to be fair use. Open weights models allow users to run the model but not necessarily modify or redistribute it, unlike true open source.

<details><summary>References</summary>
<ul>
<li><a href="https://intellibytes.substack.com/p/ai-distillation-explained-what-it">AI Distillation Explained: What It Is, How It Works, Legality Concerns</a></li>
<li><a href="https://neysa.ai/blog/open-weights-open-source/">Open Weights vs Open Source: What’s the Real Difference?</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#distillation`, `#copyright`, `#Chinese AI models`, `#open models`

---

<a id="item-6"></a>
## [Z.ai Completes Giant Data Center with Chinese Chips](https://www.bloomberg.com/news/articles/2026-07-20/z-ai-completes-giant-data-center-with-chinese-chips-to-train-ai) ⭐️ 8.0/10

Chinese AI lab Z.ai has completed construction of a 1-gigawatt data center powered entirely by domestic chips to support development of its GLM platform, with partial operations already underway. This milestone demonstrates the scalability of domestic chips for large-scale AI training, reducing reliance on foreign hardware and advancing China&\#x27;s goal of AI self-sufficiency. The facility, one of the largest built by a Chinese AI lab, has enough capacity to power about 750,000 homes and joins multiple clusters each housing over 10,000 chips.

telegram · zaihuapd · Jul 20, 15:43

**Background**: Z.ai \(Zhìpǔ\) is a leading Chinese AI company known for its GLM series of large language models. The data center uses exclusively Chinese-made chips, reflecting China&\#x27;s push to develop a self-reliant semiconductor ecosystem amid export restrictions on advanced foreign chips like Nvidia&\#x27;s.

<details><summary>References</summary>
<ul>
<li><a href="https://open.bigmodel.cn/">bigmodel - 智谱AI开放平台</a></li>

</ul>
</details>

**Tags**: `#国产芯片`, `#数据中心`, `#AI`, `#智谱`, `#中国科技`

---

<a id="item-7"></a>
## [Google&\#x27;s Frozen v2 Chip Hardwires Gemini AI for 6-10x Efficiency](https://www.quiverquant.com/news/Google+Reportedly+Developing+%E2%80%98Frozen+v2%E2%80%99+AI+Chip+to+Boost+Gemini+Efficiency) ⭐️ 8.0/10

Google is reportedly developing a server chip codenamed &\#x27;Frozen v2&\#x27; that embeds parts of its Gemini AI model directly into hardware, achieving 6 to 10 times the inference efficiency of its latest TPU. The chip is expected to be deployed by 2028. This approach dramatically reduces computational overhead and power consumption, potentially easing Google&\#x27;s internal compute shortage and enabling more efficient AI services. It represents a shift toward model-specific hardware, which could influence the broader AI chip industry. The chip is designed to complement, not replace, Google&\#x27;s TPU line, focusing on inference for Gemini models. It cuts data movement by baking the neural network architecture into circuitry, a technique described as &\#x27;frozen&\#x27;.

telegram · zaihuapd · Jul 21, 01:01

**Background**: Current AI chips like GPUs and TPUs are general-purpose accelerators that store models in memory and shuttle data back and forth, consuming power and time. Google&\#x27;s TPU is its own custom ASIC for machine learning. The Frozen v2 concept takes specialization further by locking a specific model architecture into silicon, limiting flexibility but maximizing efficiency for that model. This is analogous to how ASICs for Bitcoin mining outperform general-purpose hardware for their specific task.

<details><summary>References</summary>
<ul>
<li><a href="https://qz.com/google-gemini-chip-frozen-tpu-efficiency-072026">Google developing Gemini-specific chip called Frozen v 2</a></li>
<li><a href="https://techcrunch.com/2026/07/20/google-is-working-on-a-new-ai-chip-designed-to-make-gemini-more-efficient/">Google is working on a new AI chip designed to make Gemini ...</a></li>
<li><a href="https://thenextweb.com/news/google-frozen-chip-gemini-silicon">Google Frozen chip : Gemini baked into the silicon</a></li>

</ul>
</details>

**Tags**: `#AI芯片`, `#Google`, `#Gemini`, `#硬件优化`, `#推理效率`

---

<a id="item-8"></a>
## [Alibaba to Launch Qianwen Office, Integrating Three AI Agents](https://finance.sina.com.cn/roll/2026-07-21/doc-iniiqefa9222987.shtml) ⭐️ 8.0/10

Alibaba is set to launch &\#x27;Qianwen Office&\#x27;, a new product that integrates three AI agents — QoderWork, Wukong, and MuleRun — into a unified office platform. The initiative is led by DingTalk&\#x27;s new CEO Chen Yusen, positioning Qianwen Office as Alibaba&\#x27;s flagship offering in the AI agent office market. This consolidation signals Alibaba&\#x27;s strategic push to dominate the emerging AI agent office market, shifting competition from traditional collaboration tools to AI-driven ecosystems. With rival companies like Tencent and ByteDance also integrating their agent products, the move could reshape the competitive landscape in enterprise productivity. Qianwen Office will be built upon QoderWork, a desktop AI agent capable of autonomous task planning and execution. The product targets the &\#x27;Agent Office&\#x27; market, aiming to provide a comprehensive AI assistant for enterprise workflows.

telegram · zaihuapd · Jul 21, 10:11

**Background**: AI agents are autonomous software programs that can understand goals and execute multi-step tasks without constant human intervention. Companies like Alibaba, Tencent, and ByteDance are racing to integrate such agents into office productivity suites, moving beyond traditional collaboration tools like DingTalk and Feishu. The trend toward &\#x27;Agent Office&\#x27; represents a shift from human-driven workflows to AI-orchestrated productivity.

<details><summary>References</summary>
<ul>
<li><a href="https://qoder.com/qoderwork">QoderWork - AI Desktop Assistant | Intelligent Task Automation Tool | Qoder</a></li>
<li><a href="https://blog.csdn.net/2301_76268839/article/details/146032147">智能办公文具：AI Agent的工作效率追踪_ai agent办公-CSDN博客</a></li>

</ul>
</details>

**Tags**: `#阿里`, `#千问办公`, `#智能体`, `#钉钉`, `#Agent办公`

---

<a id="item-9"></a>
## [Google releases Gemini 3.6 Flash, starts Gemini 4 pre-training](https://9to5google.com/2026/07/21/gemini-3-6-flash-launch/) ⭐️ 8.0/10

Google released Gemini 3.6 Flash, which uses 17% fewer output tokens and improves reasoning steps and tool use. Google also announced the pre-training of Gemini 4 and introduced new models including Gemini 3.5 Flash-Lite and 3.5 Flash Cyber. This release shows Google&\#x27;s continued investment in AI, offering more efficient and specialized models. The pre-training of Gemini 4 signals the next generation of their flagship model, which could further advance the capabilities of AI assistants and enterprise tools. Gemini 3.6 Flash has a knowledge cut-off date of March 2026 and is priced at $1.5 per million input tokens and $7.5 per million output tokens. Additionally, Gemini 3.5 Pro is being tested with partners, and DeepMind has begun large-scale pre-training of Gemini 4.

telegram · zaihuapd · Jul 21, 15:23

**Background**: Tokens are units of text that AI models process, typically parts of words or punctuation. Reasoning steps refer to the process where models break down complex problems into intermediate steps, often using chain-of-thought prompting, to improve accuracy and transparency. A knowledge cut-off date indicates the last time the model&\#x27;s training data was updated, affecting its awareness of recent events.

<details><summary>References</summary>
<ul>
<li><a href="https://blogs.nvidia.com/blog/ai-tokens-explained/">What Are AI Tokens ? The Language and Currency... | NVIDIA Blog</a></li>
<li><a href="https://www.ibm.com/think/topics/chain-of-thoughts">What is chain of thought (CoT) prompting? | IBM</a></li>
<li><a href="https://www.linkedin.com/posts/arista-witty_knowledge-cut-off-in-ai-what-it-means-activity-7439630888201687040-3fkf">AI Knowledge Cutoff Dates and RAG Technology | Arista... | LinkedIn</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Google`, `#Gemini`, `#model release`, `#DeepMind`

---