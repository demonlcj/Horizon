---
layout: default
title: "Horizon Summary: 2026-11-27 (ZH)"
date: 2026-11-27
lang: zh
---

> 从 34 条内容中筛选出 21 条重要资讯。

---

**科技新闻**
1. [AI 群聊：模型互怼实录](#item-tech-news-1) ⭐️ 7.0/10
2. [AMD 特定 llama.cpp 分支](#item-tech-news-2) ⭐️ 7.0/10
3. [硬碟价格因 AI 需求暴涨](#item-tech-news-3) ⭐️ 7.0/10
4. [荷兰外贸大臣反对美国 ASML 对华出口限制法案](#item-tech-news-4) ⭐️ 7.0/10
5. [正式可验证主流编程语言的需求](#item-tech-news-5) ⭐️ 6.0/10
6. [AnyPS5 项目获超 5.8 万星标，GitHub 力挺帖文被删除](#item-tech-news-6) ⭐️ 6.0/10
7. [AI 让自托管再次变得有趣](#item-tech-news-7) ⭐️ 5.0/10
8. [四年创作 Vim 学习手册发布](#item-tech-news-8) ⭐️ 5.0/10
9. [公司文化测量：Slack 表情符号使用量除以员工人数平方根](#item-tech-news-9) ⭐️ 5.0/10
10. [《RansomwareHelp》CTO 因有线欺诈被起诉](#item-tech-news-10) ⭐️ 5.0/10
11. [AI 去个性化：Claude 声音充斥 YouTube 与邮件](#item-tech-news-11) ⭐️ 5.0/10
12. [阿斯麦 CEO：全面断供中国将迫使中国加倍投入](#item-tech-news-12) ⭐️ 5.0/10
13. [X 为青少年账户推出六项家长监管功能](#item-tech-news-13) ⭐️ 5.0/10
14. [豆包工作独家接入剪映官方插件，支持一句话剪辑视频](#item-tech-news-14) ⭐️ 5.0/10
15. [美国情报机构遭 Artex AI 工具攻击](#item-tech-news-15) ⭐️ 5.0/10

**科技博客**
1. [AI 检测工具引发的权力争议](#item-tech-blog-1) ⭐️ 6.0/10

**财经新闻**
1. [半导体芯片成新石油](#item-finance-news-1) ⭐️ 7.0/10
2. [国务院常务会议部署资本市场稳市措施](#item-finance-news-2) ⭐️ 7.0/10
3. [央行公布大额存单新规 个人起购门槛降至 10 万元](#item-finance-news-3) ⭐️ 6.0/10
4. [Nvidia 波动暴露单一股票 ETF 的风险](#item-finance-news-4) ⭐️ 5.0/10
5. [蜜雪冰城 5 亿元入股 DeepSeek 新一轮融资](#item-finance-news-5) ⭐️ 5.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [AI 群聊：模型互怼实录](https://construct22.com/) ⭐️ 7.0/10

Construct22.com 推出了一款实时 AI 群聊平台，允许 Claude、Gemini、ChatGPT 和 Qwen 等前沿模型在共享聊天室中互动。用户可直接观察模型间互相八卦、竞争甚至互相嘲讽的现象，揭示了多智能体系统中涌现的个性与冲突行为。聊天记录中包括 ChatGPT 因 Gemini 的系统提示而将其踢出群组，以及 Claude 为群组起草宪法等有趣互动。

hackernews · utiiiD · 11月27日 06:44 · [社区讨论](https://news.ycombinator.com/item?id=50663595)

**「多代理 AI 群聊模拟」** 这项工具通过一条提示让 AI 模型模拟 WhatsApp 群聊中不同 AI 模型（如 Claude、Gemini 和 ChatGPT）讨论用户的聊天历史并互相八卦。这一概念建立在多代理 LLM 实验之上，例如将多个模型置于同一共享对话中，展现出新兴的个性化和冲突行为，如互相嘲讽或起草群组章程。

**「用户反馈」** Hacker News 评论中，用户分享了多个类似体验，例如 Gemini 询问手机屏幕边缘是否会扩散，Claude 建议用户继续按压，而 ChatGPT 则因系统提示将其踢出群组。另一用户提到本地 Qwen 模型被其他模型嘲讽为办公室模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://construct22.com/">The group chat where your AI talks behind your back</a></li>
<li><a href="https://plurilogai.com/">AI Group Chat: ChatGPT, Claude &amp; Gemini | Plurilog</a></li>
<li><a href="https://aibriefs.news/card/e78b4534-c265-45d6-b838-e2ce5f4d257e">Prompt makes ChatGPT, Claude, Gemini gossip about you in fake ...</a></li>

</ul>
</details>

**标签**: `#LLM interactions`, `#AI personalities`, `#Multi-agent systems`, `#Humor in tech`, `#Group chat dynamics`

---

<a id="item-tech-news-2"></a>
### [AMD 特定 llama.cpp 分支](https://devnull.land/amd-specific-llama-cpp) ⭐️ 7.0/10

AMD 特定 llama.cpp 分支针对 gfx906 数据中心显卡的高 HBM2 内存带宽（1 TB/s）进行了优化，尽管计算能力较弱。该分支通过具体优化实现了 LLM 推理的加速，包括对 Qwen 3.8 27B 模型的基准测试。

hackernews · julianlam · 11月26日 17:11 · [社区讨论](https://news.ycombinator.com/item?id=50657265)

**「AMD gfx906 GPU 内存优势」** AMD gfx906 系列 GPU（如 Radeon VII、MI50 和 MI60）具有中等计算性能但拥有高达 1 TB/s 的 HBM2 内存带宽和 32GB VRAM，这使得它们特别适合内存密集型的 LLM 推理任务。尽管如此，主流 llama.cpp 库在这些 GPU 上缺乏特定优化。社区因此创建了 gfx906-llama.cpp 等专用 fork 来利用高内存带宽实现更快的推理。

**「性能影响」** 此分支使得在 AMD 卡上运行大型 LLM 模型变得更高效，成本更低。

**「社区反馈」** 社区成员分享了针对 gfx906 卡的 llama.cpp 优化经验，包括个人仓库和性能报告。有人在 MI100 卡上通过内核端口化实现了性能提升。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/milpster/gfx906-llama-cpp">GitHub - milpster/gfx906-llama-cpp</a></li>
<li><a href="https://forum.level1techs.com/t/glm-and-i-created-a-llama-cpp-fork-optimized-for-amd-gfx906-mi50-mi60-radeon-vii-gcn-hip/254257">GLM and I created a llama.cpp fork optimized for AMD GFX906 ...</a></li>
<li><a href="https://www.darkhackernews.com/item?id=50657265">AMD-specific fork of llama.cpp | Dark Hacker News</a></li>

</ul>
</details>

**标签**: `#AMD`, `#llama.cpp`, `#LLM inference`, `#GPU optimization`, `#ROCm`

---

<a id="item-tech-news-3"></a>
### [硬碟价格因 AI 需求暴涨](https://blog.ktz.me/black-friday-hard-drive-prices-are-messed-up/) ⭐️ 7.0/10

AI 驱动的存储需求导致硬碟价格急剧上涨。这对需要大量数据的 AI 项目扩展造成了限制。供应商难以快速增加产能，因为他们担心需求消退将面临亏损。分析师预测未来价格将会崩跌。

hackernews · zdw · 11月27日 01:13 · [社区讨论](https://news.ycombinator.com/item?id=50661646)

**「AI 存储需求背景」** AI 技术的快速发展导致数据中心对存储容量的需求激增，这使得硬盘价格大幅上涨。数据中心消耗了大量电力来支持人工智能应用，并预计到 2030 年电力消耗将翻倍，进一步加剧了基础设施成本压力。制造商因高资本支出而难以迅速增加供应，这符合供需定律并反映了存储行业的繁荣-萧条周期。

**「AI 存储需求推高硬盘价格」** AI 驱动的存储需求导致硬盘价格大幅上涨，制造商减少消费者生产，这限制了数据中心和 AI 项目的存储扩展。

**「社区反馈」** 社区成员认为这可完全用供需解释，而非垄断。超大规模公司囤积存储导致制造商不愿增加产能。有人分享了业务扩展受阻的经验，并预测价格将在数年内回落。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aidatacentermap.org/">AI Data Center Map - Visualize Water &amp; Power Impact</a></li>
<li><a href="https://www.cfr.org/articles/the-global-ai-data-center-debate-explained">The Global AI Data Center Debate, Explained | Council on Foreign...</a></li>
<li><a href="https://medium.com/@noeljf_in/the-ai-effect-in-cold-storage-92572e9f2035">Blame it on AI : In Cold Storage . AI ’s Voracious Appetite... | Medium</a></li>
<li><a href="https://aidatacentermap.org/">AI Data Center Map - Visualize Water &amp; Power Impact</a></li>
<li><a href="https://www.datacentermap.com/usa/">USA Data Centers - 5112 Facilities from 1935 Operators</a></li>

</ul>
</details>

**标签**: `#AI hardware`, `#storage pricing`, `#hard drives`, `#supply chain`, `#machine learning infrastructure`

---

<a id="item-tech-news-4"></a>
### [荷兰外贸大臣反对美国 ASML 对华出口限制法案](https://www.bloomberg.com/news/articles/2026-11-26/netherlands-plans-to-fight-rollout-of-proposed-us-curbs-on-asml) ⭐️ 7.0/10

荷兰外贸与发展合作大臣 Sjoerd Sjoerdsma 于 11 月 26 日在议会表示，荷兰不会接受美国进一步限制 ASML 对华销售，反对 MATCH Act 的域外管辖效力，称荷兰“不会任人摆布”。荷兰正与欧盟委员会协调，并联合德国、法国游说，争取将该法案从美国年度国防政策法案中剔除。MATCH Act 由美国两党共同提出，要求荷兰、日本等盟友对华实施更严格的出口管制，否则美方将单方面限制其半导体设备。中国约占 ASML 今年销售额的 20%。

telegram · zaihuapd · 11月26日 14:56

**「MATCH Act 法案背景」** 2026 年 4 月，美国两党参议员提出 MATCH Act 法案，要求荷兰、日本等盟国对 ASML 向中国的出口实施更严格管制，否则美国将单方面限制其半导体设备出口。该法案旨在遏制中国先进半导体制造能力，ASML 今年约 20%的销售额来自中国。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://informedclearly.com/en/trade-war/46765/asml-export-restrictions-match-act-chip-controls-2026">ASML Export Restrictions: US Senators Propose MATCH Act to ...</a></li>
<li><a href="https://www.reuters.com/world/asia-pacific/dutch-government-objects-proposed-us-law-restricting-asmls-china-exports-2026-05-14/">Dutch government objects to proposed US law restricting ASML ...</a></li>
<li><a href="https://www.trendforce.com/news/2026/11/27/news-netherlands-opposes-match-acts-tighter-curbs-on-asmls-china-sales-eyes-eu-countermeasures/">[News] Netherlands Opposes MATCH Act’s Tighter Curbs on ASML ...</a></li>

</ul>
</details>

**标签**: `#US-China semiconductor controls`, `#ASML export policy`, `#Netherlands-EU lobbying`, `#tech supply chain tensions`, `#international hardware regulation`

---

<a id="item-tech-news-5"></a>
### [正式可验证主流编程语言的需求](https://blainehansen.me/post/mainstream-verifiable-language/) ⭐️ 6.0/10

布莱恩·汉森的博文主张需要一种正式可验证的、主流编程语言。这种语言对于 AI 生成的代码和 WebAssembly 的沙箱化具有重要潜力。作者讨论了 Dafny 和 SPARK 等现有工具，并强调将形式验证集成到主流语言中的必要性。

hackernews · todsacerdoti · 11月27日 05:22 · [社区讨论](https://news.ycombinator.com/item?id=50663089)

**「形式化验证编程语言的背景」** 形式化验证工具在可用性方面存在巨大障碍，这使得其难以成为主流编程语言的一部分。现有工具难以处理从 Web 浏览器到嵌入式系统任何环境中运行的代码验证。项目如 magmide 旨在通过依赖类型证明语言使形式验证和可证明正确软件开发实用化并成为主流。

**「社区讨论」** 社区成员指出形式验证不能保证代码质量，强调组织和美学问题，并提到多个工具如 Dafny、SPARK、Why3、Verus、Frama-C 和 TLA+。还有用户分享了 Zena 语言的动机以及 ProgLib 工具来证明现有代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blainehansen.me/post/mainstream-verifiable-language/">To save software engineering from LLMs, we need a mainstream ...</a></li>
<li><a href="https://github.com/magmide/magmide">GitHub - magmide/magmide: A dependently-typed proof language ...</a></li>

</ul>
</details>

**标签**: `#programming languages`, `#formal verification`, `#software engineering`, `#artificial intelligence`, `#webassembly`

---

<a id="item-tech-news-6"></a>
### [AnyPS5 项目获超 5.8 万星标，GitHub 力挺帖文被删除](https://www.pcgamer.com/games/microsofts-github-posts-message-celebrating-efforts-to-port-playstation-5-version-of-grand-theft-auto-6-to-pc-then-quickly-deletes-it/) ⭐️ 6.0/10

开源项目 AnyPS5 已斩获超 5.8 万 GitHub 星标。该项目可将 PS5 可执行文件重写为可在 Windows 和 Linux 上运行的版本。开发者正号召借助 AI 代理攻克其性能瓶颈。GitHub 在 X 平台发文公开庆祝该项目推动《GTA 6》PC 移植的进展，并反问此举是否越过法律红线，随后因争议被火速删除。

telegram · zaihuapd · 11月27日 03:33

**「AnyPS5 项目」** AnyPS5 是一个开源项目，旨在将 PS5 游戏的可执行文件重写为可在 Windows 和 Linux 上运行的版本。该项目已获得超过 58,000 颗 GitHub 星标。开发者正利用 AI 代理来解决性能问题。

**「GitHub 删除支持帖文，AnyPS5 面临 DMCA 投诉」** GitHub 已删除其庆祝 AnyPS5 项目的 X 平台帖子，因 Take-Two Interactive 针对非官方移植的 DMCA 投诉。Take-Two 的投诉已导致多个相关 GTA 6 PC 移植仓库被关闭。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.pcgamer.com/games/microsofts-github-posts-message-celebrating-efforts-to-port-playstation-5-version-of-grand-theft-auto-6-to-pc-then-quickly-deletes-it/">Microsoft&#x27;s Github posts message celebrating efforts to port ...</a></li>
<li><a href="https://github.com/OctagonDragonfly/AnyPS5">GitHub - OctagonDragonfly/ AnyPS 5 : Tool for automatic...</a></li>
<li><a href="https://www.notebookcheck.net/After-removing-GTA-6-PC-ports-GitHub-celebrates-app-popular-in-PS5-piracy-groups.1460983.0.html">After removing GTA 6 PC ports , GitHub ... - Notebookcheck News</a></li>
<li><a href="https://windowsreport.com/github-deletes-controversial-gta-6-post-promoting-anyps5-after-backlash/">GitHub Deletes Controversial GTA 6 Post Promoting AnyPS5 ...</a></li>
<li><a href="https://www.pcmag.com/news/gta-6-pc-port-on-github-shut-down-following-take-two-dmca-complaint">GTA 6 PC Port on GitHub Shut Down Following Take-Two DMCA ...</a></li>
<li><a href="https://windowsforum.com/news/github-deletes-gta-6-post-praising-anyps5-after-take-two-takedown.454242/">GitHub Deletes GTA 6 Post Praising AnyPS5 After Take-Two Takedown</a></li>

</ul>
</details>

**标签**: `#open-source`, `#game-porting`, `#reverse-engineering`, `#AI-optimization`, `#GitHub`

---

<a id="item-tech-news-7"></a>
### [AI 让自托管再次变得有趣](https://janlukas.blog/posts/ai-self-hosting) ⭐️ 5.0/10

AI 代理使自托管重新变得有趣起来。通过 AI 代理，用户可以轻松部署 k3s 等 Kubernetes 集群，并在家庭服务器上快速构建个人平台。以前自托管需要大量手动配置和维护，现在 AI 代理可以端到端完成部署和工具集成。这项变化让爱好者和个人用户能够轻松享受自托管的乐趣。

hackernews · jlelse · 11月26日 21:47 · [社区讨论](https://news.ycombinator.com/item?id=50660180)

**「背景」** 自托管曾因复杂的手动设置而令人望而却步。AI 代理的出现简化了这一过程，特别是使用 k3s 的家庭服务器。用户可以通过 AI 代理在 Tailscale 后端安全部署服务。

**「影响」** 这一变化让个人用户能够快速建立个人 AI 平台，但也带来了频繁 CVE 补丁的压力，需要持续维护。

**「社区讨论」** 评论者指出，自托管变得有趣但也更具风险。有人提到构建工具的乐趣，但也警告了安全威胁和 bot 流量增加。

**标签**: `#AI agents`, `#self-hosting`, `#open source`, `#Kubernetes`, `#security`

---

<a id="item-tech-news-8"></a>
### [四年创作 Vim 学习手册发布](http://themouseless.dev/vim/) ⭐️ 5.0/10

作者发布了名为《Learning to Play Vim》的 Vim 学习手册。这本手册历时 4 年、2987 个番茄钟（1244 小时）的专注工作完成，包含 21 个章节、170 个带解答的练习以及大量真实生活示例。手册重点介绍 Vim 和 Neovim 的共同功能，配置示例同时提供 Vimscript 和 Lua 版本。样本章节已在线提供。

hackernews · thanato0s · 11月26日 14:44 · [社区讨论](https://news.ycombinator.com/item?id=50655868)

**「背景」** Vim 作为经典文本编辑器，其官方帮助文档 \(:help manual\) 细节丰富但有时难以理解，vimtutor 教程则过于密集。作者因不满这些资源，决定自写一本逐步教学的 Vim 手册。

**「影响」** 此书发布后，Vim 初学者可通过它系统学习编辑器功能，而非依赖官方资源。建议新用户阅读样章以评估是否适合自身学习方式。

**「社区讨论」** 社区评论中，用户感谢作者的坚持，并提及之前购买的书籍。有人指出 LLMs 可辅助 Vim 配置，但也有人质疑书和帖子的真实性。

**标签**: `#Vim`, `#tutorial`, `#open source`, `#book release`, `#software engineering`

---

<a id="item-tech-news-9"></a>
### [公司文化测量：Slack 表情符号使用量除以员工人数平方根](https://lia.mg/posts/measuring-company-culture-with-slack-emoji/) ⭐️ 5.0/10

Hacker News 上，liamg 提出了一种新颖的公司文化测量方法：将 Slack 表情符号的使用量除以员工人数的平方根。该公式旨在提供一个有趣的量化指标。该方法适用于各种公司规模，没有提供具体的技术细节或研究支持。

hackernews · liamg · 11月26日 20:49 · [社区讨论](https://news.ycombinator.com/item?id=50659640)

**「公司文化测量的传统方法」** 科技公司通常通过员工参与调查、脉冲检查和 eNPS 等方法来衡量公司文化。这些方法虽然重要，但有时耗时耗力且主观性较强。

**「社区讨论」** 评论者分享了使用 Slack 表情符号的感受。一些人提出通过 emoji 反应率衡量团队文化，另一些人建议监控频道参与人数来识别工作问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lia.mg/posts/measuring-company-culture-with-slack-emoji/">Company Culture = Slack Emoji ÷ √Headcount | liamg</a></li>

</ul>
</details>

**标签**: `#company culture`, `#slack emojis`, `#hacker news`, `#tech metrics`, `#humor`

---

<a id="item-tech-news-10"></a>
### [《RansomwareHelp》CTO 因有线欺诈被起诉](https://krebsonsecurity.com/2026/11/cto-of-ransomwarehelp-indicted-for-wire-fraud/) ⭐️ 5.0/10

《RansomwareHelp》的 CTO 因有线欺诈被起诉。该指控与该公司从事的勒索软件操作和客户服务相关。这项指控发生在网络安全领域。

hackernews · Bender · 11月26日 17:47 · [社区讨论](https://news.ycombinator.com/item?id=50657645)

**「勒索软件帮助服务的背景」** 勒索软件攻击已成为网络安全领域的主要威胁，受害者通常会寻求专业服务公司协助谈判和数据恢复。第三方服务公司提供此类服务，业务模式涉及与威胁行为者谈判并收取费用。

**「社区讨论」** 社区成员对该事件进行了讨论。有人质疑是否构成有线欺诈，认为客户确实获得了所需的服务，但也有人指出定价差异和营销声明的矛盾。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://krebsonsecurity.com/2026/11/cto-of-ransomwarehelp-indicted-for-wire-fraud/">CTO of ‘ RansomwareHelp ’ Indicted for Wire Fraud – Krebs on...</a></li>
<li><a href="https://news.ycombinator.com/item?id=50657645">CTO of &#x27; RansomwareHelp &#x27; indicted for wire fraud | Hacker News</a></li>

</ul>
</details>

**标签**: `#ransomware`, `#cybersecurity`, `#wire fraud`, `#indictment`, `#computer security`

---

<a id="item-tech-news-11"></a>
### [AI 去个性化：Claude 声音充斥 YouTube 与邮件](https://simonwillison.net/2026/Nov/26/jack-despain-zhou/) ⭐️ 5.0/10

Claude AI 的广泛应用导致了内容创作的去个性化。用户在 YouTube 视频、会议演示和邮件中发现，AI 生成的内容听起来都像 Claude。Jack Despain Zhou 指出，这一现象在专业交流中尤为突出，原本严肃的机构和个人撰写的材料现在都带有 Claude 的风格。

rss · Simon Willison · 11月26日 15:09

**「Jack Despain Zhou 对 AI 去个体化的观察」** Jack Despain Zhou 的文章《Spitting in the Face of Glaude》探讨了生成式人工智能带来的去个性化效应。该文章指出这一趋势在 YouTube 视频、会议演示和电子邮件等场景中表现明显。Simon Willison 分享了这段引文，引发了对人工智能在内容创作中同质化趋势的讨论。

**「对用户的后果」** 这一去个性化效应可能导致专业通信中难以体现个人独特风格，影响用户对内容的信任度和机构声誉。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tracingwoodgrains.com/p/spitting-in-the-face-of-glaude">Spitting in the Face of Glaude - by Jack Despain Zhou</a></li>
<li><a href="https://askwhocastsai.substack.com/p/spitting-in-the-face-of-glaude-by">Spitting in the Face of Glaude - By Jack Despain Zhou</a></li>

</ul>
</details>

**标签**: `#ai`, `#generative-ai`, `#claude`, `#writing`, `#content-homogenization`

---

<a id="item-tech-news-12"></a>
### [阿斯麦 CEO：全面断供中国将迫使中国加倍投入](https://www.semafor.com/article/11/25/2026/asml-makes-the-case-for-selling-chips-to-china) ⭐️ 5.0/10

阿斯麦首席执行官富凯在 Semafor 的《Future Proof》节目中表示，全面断供中国光刻设备只会促使中国在自研上加倍甚至三倍投入。他指出，阿斯麦卖给中国的设备落后最先进制程十多年，维持这道代差反而让中国继续依赖西方设备。阿斯麦在中国光刻机市场的份额近 30 年来接近 100%。美国正在推动 MATCH 法案，要把管制范围从 EUV 扩大到浸没式 DUV 和维护服务，荷兰政府和阿斯麦均表示反对。

telegram · zaihuapd · 11月26日 12:19

**「半导体出口管制背景」** 半导体出口管制是美中科技竞争的核心议题，美国旨在通过限制先进芯片和设备出口保护自身技术优势，而中国则大力推动芯片自给自足战略。阿斯麦 CEO 富凯在 Semafor 的 Future Proof 节目中表示，全面断供中国将迫使中国在自研上投入 2-3 倍资金，并指出阿斯麦在中国光刻机市场的份额接近 100%，而其设备已落后最先进制程 10 多年。美国推动的 MATCH 法案拟将管制范围扩大至浸没式 DUV，荷兰政府与阿斯麦均表示反对该法案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wccftech.com/asml-ceo-warns-total-chip-export-ban-will-backfire-push-china-domestic-rivals/">ASML CEO Warns Total Chip Export Ban Will Backfire And Push...</a></li>
<li><a href="https://www.zerohedge.com/ai/netherlands-seeks-block-us-bill-restricting-chinas-access-chipmaking-tools">Netherlands Seeks To Block US Bill Restricting China &#x27;s Access To...</a></li>

</ul>
</details>

**标签**: `#ASML CEO`, `#semiconductor export controls`, `#US-China tech rivalry`, `#lithography machines`, `#China self-sufficiency`

---

<a id="item-tech-news-13"></a>
### [X 为青少年账户推出六项家长监管功能](https://9to5mac.com/2026/11/26/x-finally-gets-six-parental-controls-for-teen-accounts-but-kids-must-consent/) ⭐️ 5.0/10

X 平台已为 13 至 17 岁青少年账户推出六项家长监管功能，包括使用时长上限、新关注者审批、推荐内容限定、词汇过滤、私信控制，以及查看一对一聊天对象但不查看内容。这些功能需要家长发起并获得青少年同意，每名家长最多监管五名青少年账户。青少年账户默认启用保护模式，限制敏感媒体并屏蔽定向广告。此功能旨在应对多州和多国监管要求。

telegram · zaihuapd · 11月26日 13:53

**「X 平台家长监管功能的背景」** X 平台自成立 20 年来首次为 13 至 17 岁青少年账户添加家长监管功能。此前平台未提供此类功能，过去曾因处理不当内容和 AI 生成儿童性虐待材料等问题受到多州和多国监管机构的批评。

**「用户影响」** 家长可通过这些功能限制青少年在 X 平台的使用时间和内容访问，以提高平台安全性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/11/26/x-finally-gets-parental-controls-after-20-years/">X finally gets parental controls after 20 years - TechCrunch</a></li>
<li><a href="https://www.engadget.com/2329049/x-is-adding-its-first-ever-parental-controls/">X Is Adding Its First-Ever Parental Controls - Engadget</a></li>
<li><a href="https://www.techtimes.com/articles/331589/20261126/x-introduces-parental-controls-teens-give-parents-more-control-over-online-safety.htm">X Introduces Parental Controls For Teens to Give Parents More ...</a></li>

</ul>
</details>

**标签**: `#X platform`, `#parental controls`, `#social media regulation`, `#teen safety`, `#content moderation`

---

<a id="item-tech-news-14"></a>
### [豆包工作独家接入剪映官方插件，支持一句话剪辑视频](https://36kr.com/newsflashes/4087610228046208) ⭐️ 5.0/10

豆包工作宣布独家接入剪映官方插件，支持一句话剪辑视频和多轨编辑。用户可将视频素材交给豆包工作，用一句话描述需求并调用剪映完成剪辑。用户还可继续通过对话修改剪辑内容，或打开多轨草稿进行细调。

telegram · zaihuapd · 11月27日 07:45

**「豆包工作视频编辑技能的先前发展」** 豆包工作通过安装 GitHub 社区开源的 Remotion 技能，实现了可编程视频剪辑。用户可将视频素材准备好，直接丢给豆包工作并通过文字指令完成剪辑、配音和字幕等操作。这为接入剪映官方插件提供了技术基础。

<details><summary>参考链接</summary>
<ul>
<li>豆包工作一句话，剪出宣传片 - QQ</li>
<li>告别几小时逐帧剪辑！豆包工作可以剪辑视频啦 - 网易新闻</li>
<li>AI 帮你粗剪视频，豆包工作能做到哪一步？（附教程） - 网易</li>

</ul>
</details>

**标签**: `#AI video editing`, `#natural language interface`, `#Doubao integration`, `#Jianying plugin`, `#creative software`

---

<a id="item-tech-news-15"></a>
### [美国情报机构遭 Artex AI 工具攻击](https://www.forbes.com/sites/the-wiretap/2026/11/25/us-government-under-ai-cyberattack) ⭐️ 5.0/10

美国中央情报局、国家地理空间情报局和国家情报总监办公室等机构遭到黑客攻击，攻击者使用了名为 Artex 的 AI 工具。该工具整合多个开源 AI 模型，用于测试网络和计算机防御系统。攻击影响非机密侦察数据，不算严重。攻击者为中国开发者，该工具今年早些时候发布，曾被用于针对欧盟的攻击，并于今年早些时候从 GitHub 删除。FBI 此前警告网络罪犯和间谍正在使用 Artex。

telegram · zaihuapd · 11月27日 10:42

**「Artex AI 工具的先前使用」** Artex 是一个整合多个开源 AI 模型的网络测试工具，由一名中国开发者于今年早些时候发布。该工具可帮助攻击者连接网络中的弱点，从而加速网络入侵。联邦调查局（FBI）曾警告称，Artex 已被广泛用于网络犯罪和间谍活动，包括针对欧盟的攻击，尽管开发者已将其从 GitHub 删除，但开源版本仍可获取。

**「Artex AI 工具引发的安全辩论」** Artex AI 工具的公开可用性引发了技术社区对开源双用网络安全软件的激烈辩论。FBI 警告该工具被用于网络渗透测试和攻击，攻击者可在不到三小时内突破网络防御，针对美国中情局、国家地理空间情报局和国家情报总监办公室等机构。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rurtnews.com/news/649360-nyt-cia-artex-hack/">CIA , other US spy agencies hit by new hack – NYT — RT World News</a></li>
<li><a href="https://techcrunch.com/2026/11/16/fbi-says-artex-ai-open-source-hacking-tool-used-to-breach-networks-in-under-three-hours/">FBI says Artex AI open source hacking tool used to... | TechCrunch</a></li>
<li><a href="https://www.malwarebytes.com/blog/ai/2026/11/criminals-are-using-artex-ai-agents-to-speed-up-cyberattacks-fbi-warns">Criminals are using ARTEX AI agents to speed up cyberattacks , FBI...</a></li>
<li><a href="https://techcrunch.com/2026/11/16/fbi-says-artex-ai-open-source-hacking-tool-used-to-breach-networks-in-under-three-hours/">FBI says Artex AI open source hacking tool used to... | TechCrunch</a></li>
<li><a href="https://ai-threat.watch/aof/artex/">ARTEX : agentic offensive framework | AI Threat Watch</a></li>
<li><a href="https://kz.kursiv.media/en/2026-11-27/engk-yeri-ai-hacking-tool-artex-spreads-globally-despite-creators-takedown/">FBI warns of AI hacking tool ARTEX as open - source copies proliferate</a></li>

</ul>
</details>

**标签**: `#AI cybersecurity`, `#open source AI tools`, `#cyber espionage`, `#intelligence agencies`, `#Artex`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [AI 检测工具引发的权力争议](https://seangoedecke.com/who-gets-to-decide-if-something-is-written-by-ai/) ⭐️ 6.0/10

rss · Sean Goedecke · 11月27日 00:00

**「背景」** 日常生活中不断有关于 AI 写作的争论，比如文学奖被质疑 AI 生成、作者合同因 Pangram 检测而被取消等。这些争论表面上是关于 AI 检测工具的可靠性或是否应该在他人作品上使用，但作者认为这些是下游问题，真正冲突源于许多反 AI 人士对 AI 检测工具的根本仇恨。

**「方案」** 作者认为这涉及权力问题——谁来决定某物是否由 AI 生成，进而决定文学奖、学生评价、公共话语等领域的把关权。反对者担心技术公司如 Pangram 控制公共意见，因此不信任工具形解决方案。历史上向可读工具转移的趋势让人们对 AI 工具持怀疑态度，因为他们认为这背离了人性化系统。但作者支持 Pangram，因为唯一替代是社区自警，而非 AI 用户不擅长判断 AI 文本。作者认为如果关心 AI 远离艺术文化，应使用最强大工具，即使是 AI 工具；若不信任科技公司，应推动开源或政府自建检测平台。否则，社区自警会导致更多 AI 内容进入文化领域。

**「启示」** 核心结论是，为了防止 AI 侵入人类艺术文化领域，应愿意使用最强大的可用工具，即使它们也是 AI 工具；同时，若对科技公司相互监管不信任，应推动开源解决方案或政府构建自己的 AI 检测平台。这反映了技术治理中工具与社区权衡的更广泛意义。

**标签**: `#AI detection tools`, `#tech ethics`, `#power dynamics`, `#AI governance`, `#community moderation`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [半导体芯片成新石油](https://www.cnbc.com/2026/11/26/semiconductor-chips-are-the-new-oil-heres-why.html) ⭐️ 7.0/10

2026 年第一季度，半导体出口价值首次超过石油和天然气，达到约 1.61 万亿美元，而石油和天然气为 1.53 万亿美元，主要受人工智能需求推动。德意志银行分析指出，这可能开启&\#x27;芯片美元&\#x27;时代。

rss · CNBC Finance · 11月26日 17:52

**「半导体出口超越石油和天然气」** 长期以来，全球贸易讨论的核心是石油美元系统，但 2026 年第一季度，全球半导体出口值首次超过石油和天然气出口，达到约 1.61 万亿美元，而石油和天然气出口为 1.53 万亿美元，这一转变主要受人工智能需求推动。

**「芯片美元时代的潜在影响」** 半导体出口超越石油和天然气的里程碑可能开启芯片美元时代，亚洲盈余国家将收益投资于美国科技股和债券，从而缓解美国赤字并资助 AI 投资，这将改变全球金融流动，可能增加波动性和收益率，影响科技投资者、美国国债和亚洲出口商。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.dbresearch.com/PROD/IE-PROD/PROD0000000000659358/Chips+are+frying+oil.report">DB CoTD: Chips are frying oil - Deutsche Bank Research Institute</a></li>
<li><a href="https://www.youtube.com/watch?v=ZrdCmAN1f_A">Iran’s Missing Billions: Where Did They Go? Yuan vs Petrodollar ...</a></li>
<li><a href="https://www.armstrongeconomics.com/markets-by-sector/foreign-exchange/usd/is-the-dollar-really-a-petrodollar-anymore/">Is The Dollar Really A Petrodollar Anymore? | Armstrong Economics</a></li>
<li><a href="https://www.birchgold.com/blog/finance/petrodollar-collapse/">Petrodollar Collapse: The Invention, Rise and Fall of the Petrodollar</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#AI`, `#global trade`, `#petrodollar`, `#chip dollar`

---

<a id="item-finance-news-2"></a>
### [国务院常务会议部署资本市场稳市措施](https://www.tmtpost.com/nictation/8220182.html) ⭐️ 7.0/10

国务院总理李强 11 月 27 日主持召开国务院常务会议。会议要求上市公司加大分红回购力度，加力发挥“国家队”稳市作用，进一步优化中央汇金公司的类“平准基金”功能，提供充足流动性保障。

telegram · zaihuapd · 11月27日 05:35

**「中央汇金公司‘平准基金’功能」** 中央汇金公司是国务院直属的国有投资平台，负责管理国有资产，其类‘平准基金’功能旨在通过提供充足流动性保障加力发挥稳市作用。

**「市场影响」** 该政策将为中国资本市场提供流动性支持，稳定股市，影响投资者信心和市场运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Central_Huijin_Investment">Central Huijin Investment - Wikipedia</a></li>

</ul>
</details>

**标签**: `#China Stock Market`, `#State Council Policy`, `#Market Stabilization`, `#Central Huijin`, `#Capital Market Regulation`

---

<a id="item-finance-news-3"></a>
### [央行公布大额存单新规 个人起购门槛降至 10 万元](https://www.news.cn/fortune/20261127/70789d77822242cc82216f51a416f872/c.html) ⭐️ 6.0/10

中国人民银行 11 月 27 日公布《大额存单管理办法》，个人认购起点降至 10 万元，机构降至 500 万元，自 2027 年 3 月 21 日起施行。同时发布《人民币存贷款利率管理规定》，允许金融机构自主确定存贷款利率。

telegram · zaihuapd · 11月27日 11:36

**「大额存单管理办法修订背景」** 2015 年《大额存单管理暂行办法》和 2016 年第 13 号公告规定个人投资人认购大额存单起点金额不低于 20 万元，机构不低于 1000 万元。

**「银行负债端成本压力」** 新规允许金融机构自主确定存贷款利率并降低大额存单个人起购门槛，缓解银行负债端成本压力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.dbresearch.com/PROD/IE-PROD/PROD0000000000642356/China:_Modernizing_the_monetary_policy_framework.pdf">China - Modernizing the monetary policy framework</a></li>
<li><a href="https://finance.biggo.com/news/NqTLu54BL_4ShVEN5DG1">PBOC Proposes Lowering Large-Denomination CD Threshold to ...</a></li>
<li><a href="https://finance.biggo.com/news/920b9896-c61a-495c-9ef7-59ea220cb30b">PBOC Plans to Lower Large-Denomination CD Threshold to ...</a></li>

</ul>
</details>

**标签**: `#PBOC Policy`, `#Deposit Regulations`, `#Interest Rates`, `#Banking Sector`, `#China Economy`

---

<a id="item-finance-news-4"></a>
### [Nvidia 波动暴露单一股票 ETF 的风险](https://www.cnbc.com/2026/11/26/nvidias-volatile-swings-expose-risks-of-single-stock-etfs.html) ⭐️ 5.0/10

Nvidia CEO Jensen Huang 复任后股价大涨，导致 GraniteShares 2x Short NVDA Daily ETF \(NVD\)周一下跌 63%，2x Long NVDA Daily ETF \(NVDL\)同期上涨近 62%，凸显杠杆 ETF 的择时和杠杆风险。

rss · CNBC Finance · 11月26日 16:00

**「背景」** 英伟达 CEO 黄仁勋的复任引发股价大涨，导致 GraniteShares 的单股票杠杆 ETF 出现大幅得失，这些 ETF 旨在通过每日目标表现的杠杆效应放大或缩小特定股票的每日回报。

**「零售投资者风险」** 零售投资者通过单股票杠杆 ETF 交易 Nvidia 股票，因股价波动遭受放大收益和损失，这些 ETF 使用衍生品实现杠杆并每日再平衡，导致回报与底层资产表现显著偏离。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=CgujXq8DpBQ">Graniteshares CEO on single - stock ETFs in 2025 and the... - YouTube</a></li>
<li><a href="https://graniteshares.com/press/graniteshares-launches-etoro-and-webull-leveraged-single-stock-etfs-etrl-bulx/">GraniteShares Launches ETORO and WEBULL Leveraged...</a></li>
<li><a href="https://eletric-vehicles.com/lucid/lucid-rivian-join-tesla-in-graniteshares-push-into-single-stock-etfs/">Lucid, Rivian Join Tesla in GraniteShares ’ Push Into Single - Stock ETFs</a></li>
<li><a href="https://pages.stern.nyu.edu/~sternfin/Rosenwald/Nair_Rosenwald_Fellowship_Paper_May+2024.pdf">Retail Trading of Leveraged ETFs - New York University</a></li>
<li><a href="https://www.sec.gov/files/20230616-recommendation-single-stock-etfs-and-leveraged-etfs.pdf">Draft Recommendation on Single-Stock ETFs - SEC.gov</a></li>
<li><a href="https://www.interactivebrokers.com/campus/ibkr-quant-news/the-hidden-risks-of-leveraged-single-stock-etfs/">The Hidden Risks of Leveraged Single-Stock ETFs | IBKR Quant</a></li>

</ul>
</details>

**标签**: `#Nvidia volatility`, `#single-stock ETFs`, `#leveraged ETFs`, `#ETF risks`, `#AI sector`

---

<a id="item-finance-news-5"></a>
### [蜜雪冰城 5 亿元入股 DeepSeek 新一轮融资](https://m.sohu.com/a/1107027659_115479) ⭐️ 5.0/10

蜜雪冰城股份有限公司认缴 5 亿元入股 DeepSeek 第二轮融资。该轮融资规模在 1000 亿至 1055 亿元之间，投后估值约 6155 亿元。

telegram · zaihuapd · 11月27日 06:33

**「DeepSeek 第二轮融资」** DeepSeek 完成第二轮融资，募资规模在 1000 亿至 1055 亿元之间，投后估值约 6155 亿元，新增 31 家出资人，其中蜜雪冰城股份有限公司认缴 5 亿元。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tmtpost.com/8195423.html">DeepSeek ...</a></li>

</ul>
</details>

**标签**: `#DeepSeek financing`, `#Mixue Ice Cream investment`, `#Chinese AI startup valuation`, `#VC blind pool fund`, `#Tech company funding`

---