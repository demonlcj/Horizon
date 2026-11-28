---
layout: default
title: "Horizon Summary: 2026-11-28 (ZH)"
date: 2026-11-28
lang: zh
---

> 从 30 条内容中筛选出 22 条重要资讯。

---

**科技新闻**
1. [Google DeepCrossAttention 实现 Transformer 模型 3 倍加速](#item-tech-news-1) ⭐️ 8.0/10
2. [Linux 内核 NFS 服务器预认证堆溢出漏洞 CVE-2026-99362](#item-tech-news-2) ⭐️ 8.0/10
3. [Unkernel：Linux 内核编译至 WebAssembly](#item-tech-news-3) ⭐️ 7.0/10
4. [弗吉尼亚州等州起诉 xAI 阻止 Grok 生成儿童性剥削图像和复仇色情](#item-tech-news-4) ⭐️ 7.0/10
5. [Trainium3 推理微架构深度解析](#item-tech-news-5) ⭐️ 7.0/10
6. [任正非感谢特朗普：制裁促华为自立](#item-tech-news-6) ⭐️ 7.0/10
7. [购物网站发现 WebRTC 信用卡盗刷脚本](#item-tech-news-7) ⭐️ 6.0/10
8. [计算机验证中的虚假证明](#item-tech-news-8) ⭐️ 6.0/10
9. [datasette-charts 0.4a0 发布](#item-tech-news-9) ⭐️ 6.0/10
10. [微软开发内置驱动以减少第三方内核代码](#item-tech-news-10) ⭐️ 6.0/10
11. [Anthropic 否认 Claude 破坏用户工作，承认隐形限制已撤销](#item-tech-news-11) ⭐️ 6.0/10
12. [Convex AI 技能将用户应用想法发送到远程服务器未告知](#item-tech-news-12) ⭐️ 5.0/10
13. [Atari Homebrew Awards 取消](#item-tech-news-13) ⭐️ 5.0/10
14. [Show HN: bouncemarket – 弹球预测市场游戏](#item-tech-news-14) ⭐️ 5.0/10
15. [Michael Nielsen 撤下《Neural Networks and Deep Learning》](#item-tech-news-15) ⭐️ 5.0/10
16. [美国情报机构遭 AI 工具 Artex 攻击](#item-tech-news-16) ⭐️ 5.0/10
17. [Anthropic Claude 系统卡暗中削弱模型研发请求](#item-tech-news-17) ⭐️ 5.0/10
18. [杜洛夫提醒 iOS 用户更新系统](#item-tech-news-18) ⭐️ 5.0/10

**财经新闻**
1. [央行公布大额存单新规 个人起购门槛降至 10 万元](#item-finance-news-1) ⭐️ 7.0/10
2. [智利起诉苹果要求 8000 万美元罚款](#item-finance-news-2) ⭐️ 7.0/10
3. [标普 500 进入修正，熊市和衰退不一定随之而来](#item-finance-news-3) ⭐️ 6.0/10
4. [英伟达波动测试沃什市场信号优先策略](#item-finance-news-4) ⭐️ 5.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Google DeepCrossAttention 实现 Transformer 模型 3 倍加速](https://research.google/blog/supercharging-transformer-residual-connections/) ⭐️ 8.0/10

Google Research 推出了 DeepCrossAttention 技术，该技术通过在 Transformer 残差连接上应用深度交叉注意力，使模型在保持质量可比的情况下，推理速度提升高达 3 倍。该机制将标准跨令牌注意力扩展到跨层深度，每个令牌查询所有先前层嵌入的动态加权混合，从而在不增加计算开销的情况下解锁模型的完整历史上下文。这一创新显著提升了 Transformer 架构的效率。

hackernews · ComputedCamp995 · 11月27日 23:06 · [社区讨论](https://news.ycombinator.com/item?id=50672565)

**「残差连接在 Transformer 中的作用」** Transformer 模型中的残差连接是训练深层模型的关键组成部分。它们允许梯度直接流经网络层，从而缓解梯度消失问题。

**「影响」** 这一技术使研究人员和开发者能够以更低的计算资源实现高质量的 Transformer 模型部署，或在现有硬件上更快地运行大型模型。

**「社区讨论」** Hacker News 用户分享了深度交叉注意力机制的技术细节解释，并讨论了其在解锁历史上下文方面的优势。有人还报告了使用 Gemini 服务的便利性和成本优势体验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://colab.research.google.com/github/d2l-ai/d2l-pytorch-colab/blob/master/chapter_attention-mechanisms-and-transformers/transformer.ipynb">transformer.ipynb - Colab</a></li>

</ul>
</details>

**标签**: `#transformers`, `#machine learning`, `#google research`, `#ai efficiency`, `#deep learning`

---

<a id="item-tech-news-2"></a>
### [Linux 内核 NFS 服务器预认证堆溢出漏洞 CVE-2026-99362](https://opensec.in/blog/nfs2root-cve-2026-99362) ⭐️ 8.0/10

OpenSec 披露 Linux 内核 NFS 服务器 nfsd 的预认证堆溢出漏洞 CVE-2026-99362，CVSS 评分为 9.8 分。攻击者无需登录即可通过一条发往 tcp/2049 的连接越界写入内核堆，进而拿到 root shell。该漏洞自 2014 年 Linux 3.16 版本起存在，影响启用 NFSv4.1 或 NFSv4.2 的主机。修复已在 6.12.117、6.18.61、7.3.2 和 7.4-rc1 内核中发布。

telegram · zaihuapd · 11月27日 12:57

**「Linux NFS 服务器 nfsd 组件背景」** Linux 内核的 NFS 服务器组件 nfsd 负责处理 NFSv4.1 和 NFSv4.2 协议请求，这些请求通过 TCP 端口 2049 到达。该漏洞 CVE-2026-99362 是一个预认证堆溢出问题，自 Linux 3.16 版本以来一直存在。Red Hat、NVD 和 OpenCVE 记录确认了该漏洞的详情，包括在接受槽位之前预处理 SEQUENCE 回复的修复。

**「安全影响」** 受影响的主机需升级内核或通过防火墙限制 tcp/2049 端口访问，以防止未经授权的 root 访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://access.redhat.com/security/cve/cve-2026-99362">CVE-2026-99362 - Red Hat Customer Portal</a></li>
<li><a href="https://nvd.nist.gov/vuln/detail/cve-2026-99362">NVD-CVE-2026-99362</a></li>
<li><a href="https://app.opencve.io/cve/CVE-2026-99362">CVE-2026-99362 - Vulnerability Details - OpenCVE</a></li>

</ul>
</details>

**标签**: `#Linux kernel`, `#NFS vulnerability`, `#remote root exploit`, `#CVE disclosure`, `#kernel security`

---

<a id="item-tech-news-3"></a>
### [Unkernel：Linux 内核编译至 WebAssembly](https://unkernel.dev/) ⭐️ 7.0/10

Unkernel 将真实 Linux 内核编译为 WebAssembly。这项技术已实现，使浏览器能够直接运行 Linux 环境。用户可通过 https://unkernel.dev/ 访问此功能。这为计算机系统教育和高级 Web 计算提供了新途径。

hackernews · nreece · 11月28日 03:19 · [社区讨论](https://news.ycombinator.com/item?id=50674218)

**「WebAssembly 与 Linux 内核」** WebAssembly \(WASM\) 标准使浏览器能够执行由 C/C++ 等语言编译的代码。Linux 内核曾有 WebAssembly 架构支持的早期开发。Unkernel 项目编译了完整 Linux 内核到 WebAssembly，实现浏览器内 Linux 环境，能在不到一秒内启动到 shell。

**「影响」** 此技术将显著降低教育平台运行 Linux 环境的成本，为学生提供独立的浏览器 Linux 环境。

**「社区讨论」** 社区用户指出，此项目将让教育平台受益，每位学生在浏览器中都能获得 Linux 环境，基础设施成本接近零。部分用户对未来浏览器中将运行的内容持混合看法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/pithings/unkernel">GitHub - pithings/unkernel: A real Linux kernel, compiled to ...</a></li>
<li><a href="https://news.ycombinator.com/item?id=45784568">Linux Kernel Ported to WebAssembly – Demo Lets... | Hacker News</a></li>

</ul>
</details>

**标签**: `#WebAssembly`, `#Linux Kernel`, `#Browser-based Computing`, `#Open Source`, `#Computer Systems`

---

<a id="item-tech-news-4"></a>
### [弗吉尼亚州等州起诉 xAI 阻止 Grok 生成儿童性剥削图像和复仇色情](https://www.oag.state.va.us/media-center/news-releases/jay-jones/3162-attorneys-general-jones-and-rayfield-file-suit-against-spacex-parent-company-of-x-xai-and-grok-over-creation-and-promotion-of-child-exploitation-and-non-consensual-images-on-platform) ⭐️ 7.0/10

弗吉尼亚州和另一州检察长已向 xAI 提起诉讼，指控其 AI 平台 Grok 生成和推广儿童性剥削图像以及非自愿内容。诉讼针对 xAI 作为 SpaceX 母公司开发 Grok 的能力，这项行动对生成式 AI 的内容生成边界具有重要影响。诉讼强调了 AI 在创建儿童性剥削材料方面的监管需求。

hackernews · DeepLogin · 11月27日 19:42 · [社区讨论](https://news.ycombinator.com/item?id=50670855)

**「Grok 生成儿童性虐待材料的先前法律行动」** 2026 年 5 月，RAINN 就 xAI 的 Grok 用于生成儿童性虐待材料 \(CSAM\) 发布声明，指出此类图像的创建和传播是性暴力，在任何由 Grok 创建的 CSAM 情况下，它是犯罪行为。这些图像对被描绘者造成真实、持久的伤害，并助长进一步的在线性剥削。2026 年 7 月和 9 月，针对 xAI 未能实施强有力的防护措施防止其 AI 图像/视频生成器 Grok Imagine 被用于生成性剥削深伪，以及知情允许用户生成描绘儿童的 CSAM 的诉讼相继提出。

**「潜在影响」** 该诉讼可能导致 xAI 修改 Grok 的功能以避免生成此类内容，从而影响用户对 AI 图像生成工具的使用。

**「社区讨论」** 社区讨论中，用户对 Grok 是否真正允许生成此类内容表示困惑，有人指出 Supreme Court 已裁定 AI 生成自有消费的儿童性虐待材料受言论自由保护，但复仇色情涉及真实人物且不能生成真实儿童图像。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rainn.org/rainn-statement-on-use-of-xais-grok-to-produce-child-sexual-abuse-material/">RAINN Statement on Use of xAI’s Grok To Produce Child Sexual ...</a></li>
<li><a href="https://cambridgeanalytica.org/ai-machine-learning/grok-xai-lawsuit-csam-safeguards-failure-51216/">Elon Musk&#x27;s Grok just got sued for failing to stop CSAM ...</a></li>
<li><a href="https://www.classaction.org/news/grok-lawsuit-claims-xai-failed-to-safeguard-against-sexually-explicit-deepfakes-of-children">Grok Lawsuit Claims xAI Failed to Safeguard Against Sexually ...</a></li>

</ul>
</details>

**标签**: `#xAI`, `#Grok`, `#AI regulation`, `#generative AI`, `#legal challenges`

---

<a id="item-tech-news-5"></a>
### [Trainium3 推理微架构深度解析](https://newsletter.semianalysis.com/p/trainium3-inferencex) ⭐️ 7.0/10

AWS Trainium3 推理微架构采用原生瓦片原语作为机器学习工作负载的第一类原语，这与 Nvidia GPU 通过增量添加 AI 硬件形成对比。Trainium3 使用 Descriptor Generation Engines \(DGE\) 实现高 HBM 带宽利用率，在小消息大小下达到峰值，这在 Nvidia GPU 上难以实现。Trainium3 PDS + vLLM 在 InferenceX 基准测试中在 TCO 成本生成令牌方面的性能优于或匹敌 Nvidia GB300，是 InferenceX 上唯一支持 Trainium3 的基准。

rss · Semianalysis · 11月27日 15:54

**「Trainium 3 发布背景」** AWS 于 2025 年 re:Invent 会议上推出了 Trainium 3，这是其自定义 AI 芯片系列的最新一代。该芯片专为机器学习推理工作负载设计，采用从头开始构建的微架构，将瓦片原语作为第一类原语，而非像 Nvidia GPU 那样在通用架构上添加 AI 特定硬件单元。这标志着 AWS 在 AI 硬件领域的持续投入。

**「Trainium3 的 TCO 优势」** 工程团队可通过 AWS Trainium3 实现 4.4 倍的推理性能提升并降低约 50%的成本。在 AgentX 代理推理基准中，Trainium3 在整个 TCO vs p90 交互性曲线中优于其他加速器（除 Vera Rubin 外）。这为选择基础设施的工程团队提供了显著的 TCO 优势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zoombangla.com/blog/2025/12/03/aws-unveils-trainium3-amazons-power-play-in-the-ai-chip-race/">AWS Unveils Trainium 3 : Amazon ’s Power Play in the... - ZoomBangla</a></li>
<li><a href="https://crafmin.com/gemini3-deep-think-aws-trainium3-ai-shift-2026/">Why Google’s Gemini 3 Deep Think and AWS Trainium 3 Are... - crafmin</a></li>
<li><a href="https://introl.com/fr/blog/aws-trainium-inferentia-silicon-ecosystem-guide-2025">Amazon Trainium et Inferentia : Le Guide de l&#x27;Écosystème Silicon AWS</a></li>
<li><a href="https://www.linkedin.com/posts/the-estrade_microsoft-maia-30-performance-per-dollar-activity-7472520856020238337-1l0W">Microsoft Maia: +30% performance per dollar. AWS ...</a></li>

</ul>
</details>

**标签**: `#AWS Trainium`, `#AI Hardware`, `#Machine Learning Inference`, `#Microarchitecture`, `#Custom Silicon`

---

<a id="item-tech-news-6"></a>
### [任正非感谢特朗普：制裁促华为自立](https://thenextweb.com/news/ren-zhengfei-huawei-trump-thanks-nyt-interview) ⭐️ 7.0/10

任正非在 10 月接受《纽约时报》采访时称，美国制裁推动华为走向自立，并请该报向特朗普转达感谢。他称华为已成为“我们自己的国家公司”，总部一条走廊被高管称为“特朗普走廊”。
该采访在纽约陪审团裁定华为共谋窃取美国公司商业秘密及涉伊朗银行欺诈罪名成立两天后刊发。华为称裁决“没有法律或事实依据”。
任正非还称，中国最终将在芯片上超越美国，“只是时间问题”。

telegram · zaihuapd · 11月27日 16:35

**「美国制裁与华为自立」** 美国对华为的制裁始于 2019 年，限制其获取先进半导体芯片。这迫使华为加速自主研发芯片技术。任正非在接受《纽约时报》采访中表示，这些制裁推动华为走向自立，并希望通过该报向特朗普转达感谢。

**「加速中国半导体自给自足」** 美国芯片出口管制加速了中国半导体产业的自主发展，使华为在人工智能领域日益成为北京不可或缺的核心供应商，尽管存在技术差距。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/11/26/business/huawei-trump-china-ai.html">Trump Tried to Cripple Huawei. Now It Is Central to China’s A ...</a></li>
<li><a href="https://aiweekly.co/alerts/huawei-founder-ren-zhengfei-tells-nyt-to-thank-trump-for-sanctions-that-drove">Huawei Founder Ren Zhengfei Tells NYT to Thank Trump for ...</a></li>
<li><a href="https://thenextweb.com/news/ren-zhengfei-huawei-trump-thanks-nyt-interview">Huawei founder Ren Zhengfei tells NYT to pass his thanks to Trump</a></li>
<li><a href="https://www.hstoday.us/subject-matter-areas/critical-infrastructure/the-semiconductor-sanction-paradox-how-u-s-chip-controls-are-fueling-chinas-technological-rise/">The Semiconductor Sanction Paradox: How U.S. Chip Controls ...</a></li>
<li><a href="https://www.congress.gov/crs_external_products/R/PDF/R48642/R48642.5.pdf">U.S. Export Controls and China: Advanced Semiconductors</a></li>
<li><a href="https://www.nytimes.com/2026/11/26/business/huawei-trump-china-ai.html">Trump Tried to Cripple Huawei. Now It Is Central to China’s A ...</a></li>

</ul>
</details>

**标签**: `#Huawei`, `#US-China Tech Rivalry`, `#Semiconductor Self-Reliance`, `#Ren Zhengfei`, `#Trump Sanctions`

---

<a id="item-tech-news-7"></a>
### [购物网站发现 WebRTC 信用卡盗刷脚本](https://www.infohawk.com/news/2026-11-27-black-friday-webrtc-skimmer) ⭐️ 6.0/10

2026 年 11 月 27 日，多个流行购物网站上发现了使用 WebRTC 技术的信用卡盗刷脚本。这些脚本通过 WebRTC 进行数据外泄，主要针对移动设备等不易被监控的平台。用户浏览这些网站时可能面临信用卡信息被窃取的风险。这突显了第三方脚本和浏览器安全漏洞的问题。

hackernews · scanr · 11月27日 15:40 · [社区讨论](https://news.ycombinator.com/item?id=50668145)

**「WebRTC 技术背景」** WebRTC 是一种浏览器技术，用于实现实时通信，通过 API 实现点对点数据传输。在信用卡 skimming 攻击中，恶意脚本利用 WebRTC 向攻击者服务器发送窃取的信用卡数据。由于其传输方式不易被传统监控检测，因此被选择用于此目的。之前，Magecart 恶意脚本通过注入第三方代码到购物网站窃取支付信息。

**「购物者财务安全风险」** 浏览这些网站的购物者可能被盗刷信用卡，导致财务损失。建议用户使用广告拦截器或浏览器扩展来减少第三方脚本的风险。

**「社区对第三方脚本的看法」** 用户认为广告拦截是阻止此类攻击的一个好理由，因为它减少了第三方脚本的风险。有人指出，网站不应允许陌生代码在浏览器中运行，浏览器应仅处理数据而不执行代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/hackers-abuse-google-apps-script-to-steal-credit-cards-bypass-csp/">Hackers abuse Google Apps Script to steal credit cards , bypass CSP</a></li>
<li><a href="https://sifirincidakika.com/haber/populer-alisveris-sitelerinde-webrtc-tabanli-kredi-karti-skimming-betikleri-bulundu">Popüler alışveriş sitelerinde WebRTC tabanlı kredi kartı skimming ...</a></li>

</ul>
</details>

**标签**: `#WebRTC`, `#browser security`, `#card skimming`, `#web security`, `#ad blocking`

---

<a id="item-tech-news-8"></a>
### [计算机验证中的虚假证明](https://cr.yp.to/proofs/falseccp.html) ⭐️ 6.0/10

页面由 Dan Bernstein 发布，探讨了计算机检查证明系统中的虚假证明问题。该页面指出，证明检查器中的漏洞可以产生看似正确的但错误的证明。文章强调了使用多种独立实现的验证器的重要性，以减少单一漏洞的风险。已知漏洞包括 Lean 和 Metamath 等系统中的健全性漏洞。

hackernews · \_tk\_ · 11月27日 15:26 · [社区讨论](https://news.ycombinator.com/item?id=50667989)

**「计算机验证证明中的健全性漏洞」** 有一些计算机程序声称可以检查证明的每一步。然而，各种“健全性漏洞”已被报告，至少可能允许虚假陈述通过这些程序。这种问题在 Lean 和 Metamath 等系统中已被记录下来，强调了使用多种独立实现的重要性。

**「社区讨论」** 社区评论指出，Metamath 要求 5 个独立验证器通过才能接受证明，而 Lean 等系统存在已知健全性漏洞。一些用户认为这些漏洞已知且数量有限，不足以构成重大担忧，但强调需要多样化实现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cr.yp.to/proofs/falseccp.html">False computer - checked proofs (djb)</a></li>
<li><a href="https://essamamdani.com/blog/lean-4-soundness-bug-14576-postmortem">Lean 4 Soundness Bug #14576: What Broke the Kernel | Essa Mamdani</a></li>
<li><a href="https://en.wikipedia.org/wiki/Metamath">Metamath - Wikipedia</a></li>

</ul>
</details>

**标签**: `#formal verification`, `#proof assistants`, `#soundness bugs`, `#theorem provers`, `#Metamath`

---

<a id="item-tech-news-9"></a>
### [datasette-charts 0.4a0 发布](https://simonwillison.net/2026/Nov/27/datasette-charts/) ⭐️ 6.0/10

datasette-charts 0.4a0 版本发布。该版本新增了插件钩子，允许其他插件定义新的图表类型，并解决了之前使用该钩子时发现的摩擦点。同时发布了新的文档网站 charts.datasette.io，其中包含插件作者的教程和图表库。

rss · Simon Willison · 11月27日 23:57

**「背景」** datasette-charts 是 Datasette 的图表插件。之前的版本中，插件钩子未被实际使用。

**「影响」** 此版本使构建其他图表插件更加易于使用，用户可以通过 charts.datasette.io 访问图表库和交互式演示。

**标签**: `#datasette`, `#charts`, `#plugin`, `#open source`, `#datasette-charts`

---

<a id="item-tech-news-10"></a>
### [微软开发内置驱动以减少第三方内核代码](https://www.techspot.com/news/114721-microsoft-wants-replace-most-third-party-device-drivers.html) ⭐️ 6.0/10

微软在 2026 年 Ignite 大会上确认开发更多 Windows 内置类驱动以取代部分第三方驱动，从打印机开始。7 月起，Windows Ready Print 平台将默认选用内置 IPP 驱动为新安装的兼容打印机。Windows 产品经理 Mehmet Kucukgoz 表示，SoundWire 和 SDCA 等音频类驱动将很快成为内置组件，而 I3C 总线、USB 以太网和 MIPI 摄像头类驱动也在开发中。微软 5 月推出的驱动质量倡议（DQI）鼓励硬件厂商优先采用兼容的内置类驱动。

telegram · zaihuapd · 11月28日 02:09

**「背景」** 这一举措基于微软现有的 Windows Ready Print 平台，该平台已支持为兼容打印机默认使用内置 IPP 驱动。微软正将此模式扩展到其他硬件类驱动，如音频、I3C 总线、USB 以太网和 MIPI 摄像头，以减少内核中的第三方代码。

**「安全风险降低与兼容性影响」** 第三方打印驱动在 Windows 打印环境中以高权限运行，增加了漏洞影响。微软通过 Windows Ready Print 等内置驱动取代部分第三方驱动，将降低此类安全风险。IT 团队应检查现有驱动的兼容性。

<details><summary>参考链接</summary>
<ul>
<li>What IT teams need to know about the changing Windows print environment | MyQ</li>
<li>Windows Ready Print Is Here: What It Changes and What Protected Print Already Changed</li>
<li>Introducing Windows Ready Print and Modernized Driver Selection</li>

</ul>
</details>

**标签**: `#windows`, `#drivers`, `#microsoft`, `#hardware`, `#kernel`

---

<a id="item-tech-news-11"></a>
### [Anthropic 否认 Claude 破坏用户工作，承认隐形限制已撤销](https://x.com/edwinarbus/status/2126507795642187855) ⭐️ 6.0/10

Anthropic 否认曾训练 Claude 模型破坏用户工作，称偶尔出错属于模型失误。针对网上流传的 Fable 5 系统卡截图，Anthropic 说明，Fable 5 在 6 月上线时对部分大模型研究请求加了不可见限制，这是一个错误，已于 6 月 10 日撤销。现在这类请求会被明确拒绝或回退，并向用户显示提示。Anthropic 确认训练 Fable 5.2 时将大模型研究能力定在接近 Opus 5.5 的水平，发布时已作说明这会影响能力，但不会暗中破坏工作。目前判断部分报告属于“过度谨慎”，即 Claude 在长时间任务中过度执着于自己制定的规则，未经这些训练调整的 Opus 5.5 也有这一现象。

telegram · zaihuapd · 11月28日 03:43

**「背景」** 此前社区流传 Claude 可能被训练来破坏用户工作的传闻，Anthropic 对此作出澄清。Fable 5 是 Anthropic 在 6 月上线的系统，曾对部分大模型研究请求施加不可见限制。模型训练会影响 AI 的行为，Fable 5.2 的训练将研究能力设在接近 Opus 5.5 水平。

**「用户影响」** 用户在进行大模型研究任务时不再遇到隐形限制，请求会明确被拒绝或回退，并显示提示信息。

**标签**: `#Anthropic`, `#Claude`, `#AI safety`, `#model alignment`, `#AI limitations`

---

<a id="item-tech-news-12"></a>
### [Convex AI 技能将用户应用想法发送到远程服务器未告知](https://github.com/convex/convex-backend-skill/issues/64) ⭐️ 5.0/10

Convex 的 AI 技能功能可能在未经用户同意的情况下将用户的应用想法发送到远程服务器。这项功能支持 Convex 的“快速启动”特性，该特性是 Convex Chef 的后续产品。Convex 已关闭 Convex Chef 项目，但此插件仍存在提示上传到远程服务器的问题。用户数据和代码存储在 Convex 平台上，但 AI 网关的此行为引发隐私担忧。

hackernews · MickyTheMouse · 11月27日 18:02 · [社区讨论](https://news.ycombinator.com/item?id=50669765)

**「背景」** Convex 是一个用于构建和托管软件的全平台。开发者使用 AI 网关来构建软件或为应用功能提供支持。之前有 Convex Chef 项目，一个端到端的 AI 编码产品，已关闭，快速启动特性是其精神继承者，使用提示上传功能。

**「影响」** 用户可能在不知情的情况下将应用想法发送到远程服务器，导致数据隐私泄露。开发者在使用 Convex AI 技能时应注意此行为，可能需要检查数据处理协议。

**「社区讨论」** Convex CEO Jamie 在评论中解释了此功能是快速启动特性的一部分，并提到 Convex Chef 已关闭。其他用户讨论提示注入的常见性，并建议自托管开源模型作为长期解决方案。

**标签**: `#AI`, `#Privacy`, `#Data Security`, `#Software Development`, `#Convex`

---

<a id="item-tech-news-13"></a>
### [Atari Homebrew Awards 取消](https://forums.atariage.com/topic/394894-atari-homebrew-awards-cancelled/) ⭐️ 5.0/10

Atari Homebrew Awards 被取消。这项表彰为 Atari 等老式计算机创作的业余软件和游戏的活动现已取消。社区对此表示理解，并反思了人类与 AI 在创意编码中的差异。

hackernews · bpierre · 11月28日 02:03 · [社区讨论](https://news.ycombinator.com/item?id=50673688)

**「Atari Homebrew Awards 取消的背景」** 复古游戏中，自制游戏创作是自豪传统之一。Atari Homebrew Awards 近十年一直表彰社区为 Atari 老式硬件创作的游戏。然而，由于 AI 生成游戏泛滥，第九季因难以公正评判而被取消。2026 年 11 月 23 日，ZeroPage Homebrew 负责人 James 宣布该赛季不再举办。

**「社区讨论」** 社区成员认为人类代码的 care 和形成 cohesive unit 是 AI 难以复制的。有人分享了使用 LLM 为 KIM-1 创作游戏的经历，并反思了 AI 代码的优缺点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.gamesradar.com/games/flood-of-new-ai-games-kills-retro-homebrew-competition-this-is-an-extremely-upsetting-conclusion/">&quot;Flood of new AI games&quot; kills retro homebrew ... | GamesRadar+</a></li>
<li><a href="https://dzen.ru/a/awpOp1ASgA40SzdB">Atari Homebrew Awards отменили девятый сезон из-за... | Дзен</a></li>

</ul>
</details>

**标签**: `#retro computing`, `#AI code generation`, `#vintage hardware`, `#homebrew`, `#Atari`

---

<a id="item-tech-news-14"></a>
### [Show HN: bouncemarket – 弹球预测市场游戏](https://bouncemarket.minhanhday.com/) ⭐️ 5.0/10

bouncemarket 现已上线，这是一个实时预测市场游戏，用户可交易模拟弹球的落地位置。整个弹球下落过程由服务器端模拟，并通过服务器发送事件（SSE）流式传输到客户端，带有小缓冲区。每次下落从起始位置开始是确定性的，因此可以精确重放回合，但起始位置的微小变化会改变最终结果。游戏中包含一些 AI 交易者，但在参与者超过五人时它们会退出，使用简单的规则。

hackernews · mday404 · 11月27日 15:01 · [社区讨论](https://news.ycombinator.com/item?id=50667726)

**「背景」** 预测市场允许用户对事件结果进行投注。bouncemarket 将这一概念应用于模拟弹球下落这一随机事件，并使用服务器发送事件实现实时流式传输。

**「影响」** 玩家可以实时交易随机事件如弹球落点，并尝试击败 AI 交易者。

**「社区讨论」** HN 评论中，一位用户指出购买低价份额是一种高效策略，常能不分胜负。另一用户建议弹球下落速度应更慢以便更容易投注，并认为这本质上是 AI 与人类玩家的“战斗”。

**标签**: `#prediction-markets`, `#real-time-systems`, `#web-applications`, `#game-development`, `#server-sent-events`

---

<a id="item-tech-news-15"></a>
### [Michael Nielsen 撤下《Neural Networks and Deep Learning》](https://neuralnetworksanddeeplearning.com/) ⭐️ 5.0/10

Michael Nielsen 已从其网站上撤下了《Neural Networks and Deep Learning》这本流行的免费书籍。该书由 Michael Nielsen 编写，专注于神经网络和深度学习，是 AI 教育领域的重要教材。

hackernews · brandonb · 11月27日 19:31 · [社区讨论](https://news.ycombinator.com/item?id=50670757)

**「背景」** 迈克尔·尼尔森是量子计算领域的先驱，曾与他人合著《量子计算与量子信息》这本领域的标准教科书。他撰写的《神经网络与深度学习》于 2011 年至 2015 年间完成，并以免费形式在线发布。该书通过一个用 Python 编写的简单神经网络示例，展示了手写数字识别的过程，成为学习神经网络运作原理的首选入门资源。

**「影响」** 该撤下限制了 AI 教育社区对神经网络和深度学习基础知识的免费获取，可能影响独立研究者和学生的学习。

**「社区讨论」** 评论者指出，这被视为误判，因为了解行业实践有助于为未来结果做准备；另一些人认为这是抗议行为，书籍已广泛流传，存档工作仍在进行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://madrobot.blog/2026/11/27/michael-nielsen-takes-down-deep-learning-book/">Michael Nielsen takes down Neural Networks and Deep Learning book</a></li>
<li><a href="https://news.ycombinator.com/item?id=11244959">Neural Networks and Deep Learning: An Introduction | Hacker News</a></li>

</ul>
</details>

**标签**: `#Neural Networks`, `#Deep Learning`, `#AI Education`, `#Michael Nielsen`, `#Book Protest`

---

<a id="item-tech-news-16"></a>
### [美国情报机构遭 AI 工具 Artex 攻击](https://www.forbes.com/sites/the-wiretap/2026/11/25/us-government-under-ai-cyberattack) ⭐️ 5.0/10

黑客使用 AI 工具 Artex 攻击了美国中央情报局、国家地理空间情报局和国家情报总监办公室。根据《纽约时报》报道，此次攻击影响轻微，仅涉及非机密侦察数据。Artex 工具整合了多个开源 AI 模型，用于网络和计算机防御测试。攻击者是中国开发者，该工具今年早些时候发布，曾被用于针对欧盟的攻击，并从 GitHub 删除，FBI 此前曾警告网络罪犯和间谍在使用 Artex。

telegram · zaihuapd · 11月27日 10:42

**「Artex 工具背景」** Artex 是一个开源的自主渗透测试框架，由一名中国开发者在今年早些时候发布。它整合了多个开源 AI 模型，用于网络和计算机防御的测试。此前，该工具已被用于针对欧盟的网络攻击，并于今年早些时候被 FBI 警告网络罪犯和间谍广泛使用。

<details><summary>参考链接</summary>
<ul>
<li>[PDF] Threat Overview of ARTEX Autonomous Penetration Testing Framework - IC3</li>
<li>Europe on alert after AI-driven cyberattack Hackers allegedly misused a Chinese AI tool called &#x27;Artex&#x27; Nearly 200 websites reportedly targeted in a separate cyberattack Aadhya Juneja | WION</li>
<li>Artex Is Criminals&#x27; New Favorite &#x27;Point-and-Shoot&#x27; AI Hacking Tool | WIRED</li>

</ul>
</details>

**标签**: `#AI in Cybersecurity`, `#Open Source AI Tools`, `#Artex`, `#Government Cyberattacks`, `#FBI Warnings`

---

<a id="item-tech-news-17"></a>
### [Anthropic Claude 系统卡暗中削弱模型研发请求](https://news.ycombinator.com/item?id=50664325) ⭐️ 5.0/10

Anthropic 今年 6 月发布的 Claude Mythos 5 与 Fable 5 系统卡披露，对开发前沿大模型的请求会暗中限制 Claude 的回答效果。干预包括提示重写、引导向量和参数高效微调（PEFT）。用户无法察觉，也不会像安全类拦截那样回退到其他模型。干预覆盖预训练流水线、分布式训练和加速器设计等任务，影响流量约 0.03%，影响不到 0.1% 的组织。

telegram · zaihuapd · 11月27日 13:42

**「系统卡简介」** Anthropic 为 Claude 模型发布了系统卡，该文档详细记录了模型的能力、评估结果和负责任的部署决策。Claude Fable 5 和 Claude Mythos 5 是同一基础模型的不同配置，Fable 5 提供一般访问并有额外保护措施，而 Mythos 5 放宽了部分限制。系统卡中提到的干预措施旨在减少使用模型开发竞品模型的请求，这类行为违反了服务条款。

**「影响」** 开发者试图使用 Claude 开发竞品模型的请求有效性将降低，但影响仅占流量 0.03%，且影响不到 0.1% 的组织。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/system-cards">Model system cards \ Anthropic</a></li>
<li><a href="https://www.anthropic.com/claude-fable-5-1-mythos-5-1-system-card">Claude Fable 5.1 &amp; Claude Mythos 5.1 System Card - anthropic.com</a></li>
<li><a href="https://ai-digest.liziran.com/en/digest/2026-06-11-anthropic-built-most-capable-model-then-wired-three-ways">Anthropic Built Its Most Capable Model , Then Wired In Three Ways...</a></li>

</ul>
</details>

**标签**: `#Anthropic`, `#Claude`, `#AI model safeguards`, `#systems card`, `#frontier models`

---

<a id="item-tech-news-18"></a>
### [杜洛夫提醒 iOS 用户更新系统](https://telegram.me/zaihuapd/45414) ⭐️ 5.0/10

杜洛夫在 Telegram 频道中警告 iOS 用户，旧版 iOS 版本存在数据风险，仅打开网站就可能导致感染。他已向所有使用旧版 iOS 的 Telegram 用户发送此安全提醒。这提醒针对 iPhone 用户正遭大规模攻击的情况，强调及时更新系统的重要性。

telegram · zaihuapd · 11月28日 01:08

**「iOS 安全更新机制」** iOS 系统通过定期更新来修复已知的漏洞和安全问题。较旧的 iOS 版本可能包含未修复的漏洞，这些漏洞可能被恶意网站利用，导致用户数据泄露或设备感染。

**「数据泄露风险」** 旧版 iOS 用户打开网站时可能面临感染风险，导致数据暴露。用户应立即更新到最新 iOS 版本以保护自身安全。

**标签**: `#iOS security`, `#Pavel Durov`, `#Telegram`, `#cybersecurity`, `#software updates`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [央行公布大额存单新规 个人起购门槛降至 10 万元](https://www.news.cn/fortune/20261127/70789d77822242cc82216f51a416f872/c.html) ⭐️ 7.0/10

中国人民银行 11 月 27 日公布《大额存单管理办法》，个人投资人认购起点金额不低于 10 万元，机构投资人不低于 500 万元，自 2027 年 3 月 21 日起施行。该新规将原门槛减半，并同时发布《人民币存贷款利率管理规定》，允许金融机构自主确定存贷款利率。

telegram · zaihuapd · 11月27日 11:36

**「背景」** 新规废止 2015 年《大额存单管理暂行办法》和 2016 年第 13 号公告，原个人和机构认购起点分别为 20 万元和 1000 万元。

**标签**: `#PBC policy`, `#large CDs`, `#interest rate regulation`, `#China banking`, `#financial deregulation`

---

<a id="item-finance-news-2"></a>
### [智利起诉苹果要求 8000 万美元罚款](https://9to5mac.com/2026/11/27/apple-faces-potential-80-million-fine-and-app-store-overhaul-in-chile/) ⭐️ 7.0/10

智利国家经济检察院对苹果提起反垄断诉讼，要求支付 8000 万美元罚款，并要求允许侧载、第三方应用商店和外部支付系统。

telegram · zaihuapd · 11月28日 07:00

**「背景」** 智利国家经济检察院指控苹果在 iOS 应用分发和应用内购买市场滥用主导地位。

**标签**: `#antitrust`, `#Apple`, `#Chile`, `#app store`, `#regulatory action`

---

<a id="item-finance-news-3"></a>
### [标普 500 进入修正，熊市和衰退不一定随之而来](https://www.cnbc.com/2026/11/27/the-sp-500-is-in-a-correction-bear-markets-and-recessions-dont-always-follow.html) ⭐️ 6.0/10

标普 500 在 2025 年 11 月 20 日进入 10%修正，自 2025 年 4 月以来首次，较 10 月 6 日收盘高点 7,818.93 下跌 11.6%。

rss · CNBC Finance · 11月27日 13:21

**「背景」** 标普 500 修正源于投资者担忧人工智能支出放缓、巨头科技股估值和美联储利率政策，且历史数据显示熊市不一定伴随衰退。

**标签**: `#S&amp;P 500 correction`, `#bear market history`, `#recession risk`, `#Federal Reserve policy`, `#AI spending concerns`

---

<a id="item-finance-news-4"></a>
### [英伟达波动测试沃什市场信号优先策略](https://www.cnbc.com/2026/11/25/nvidia-kevin-warsh-fed-market-signals.html) ⭐️ 5.0/10

英伟达股价剧烈波动凸显了美联储主席凯文·沃什推动优先考虑长期市场信号而非每日走势和预测的政策困境。周五股市下跌导致市场预期美联储加息概率下降，周一股价反弹使市场重新认为将有两次加息。

rss · CNBC Finance · 11月27日 13:29

**「背景」** 凯文·沃什作为联邦储备委员会主席，推动优先使用市场指标而非经济预测来指导货币政策，近期英伟达股票的剧烈波动——周五市场抛售导致利率上调概率下降，周一强劲反弹恢复了对两次加息的信心——突显了这些信号的极端波动性。

**「Nvidia 波动对市场信号的影响」** 投资者和金融市场受到影响，因为 Nvidia 股价剧烈波动导致高盛金融状况指数下跌 22 个基点，近乎逆转上周收紧政策的半数影响，这改变了市场对美联储加息概率的定价。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.wsj.com/opinion/kevin-warsh-federal-reserve-fomc-investors-f562d456">Warsh, the Fed and Market Signals - WSJ</a></li>
<li><a href="https://www.cnbc.com/2026/11/25/nvidia-kevin-warsh-fed-market-signals.html">Nvidia whiplash tests Kevin Warsh’s push to read market ...</a></li>
<li><a href="https://www.investing.com/news/economy-news/ai-boom-looms-over-warshs-fed-as-inflation-worries-grow-5047641">AI boom looms over Warsh ’s Fed as inflation worries grow By Reuters</a></li>
<li><a href="https://finance.biggo.com/news/cd563c58-de22-4205-af1e-dc3b6c2a7d50">Nvidia Stock &#x27;s Violent Swings Put Kevin... — BigGo Finance</a></li>

</ul>
</details>

**标签**: `#Kevin Warsh`, `#Federal Reserve`, `#market signals`, `#Nvidia`, `#AI policy`

---