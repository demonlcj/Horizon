---
layout: default
title: "Horizon Summary: 2026-11-28 (EN)"
date: 2026-11-28
lang: en
---

> From 30 items, 22 important content pieces were selected

---

**Technology News**
1. [Google DeepCrossAttention: 3x Faster Transformers](#item-tech-news-1) ⭐️ 8.0/10
2. [CVE-2026-99362: Linux NFS Server Heap Overflow Enables Unauthenticated Root Access](#item-tech-news-2) ⭐️ 8.0/10
3. [Linux Kernel Compiled to WebAssembly](#item-tech-news-3) ⭐️ 7.0/10
4. [Virginia Sues xAI Over Grok Generating Child Sex Images and Revenge Porn](#item-tech-news-4) ⭐️ 7.0/10
5. [AWS Trainium3 Inference Microarchitecture Analysis](#item-tech-news-5) ⭐️ 7.0/10
6. [Ren Zhengfei Thanks Trump for Huawei Self-Reliance](#item-tech-news-6) ⭐️ 7.0/10
7. [WebRTC Card Skimming Scripts Discovered on Shopping Sites](#item-tech-news-7) ⭐️ 6.0/10
8. [False Proofs in Computer-Checked Systems](#item-tech-news-8) ⭐️ 6.0/10
9. [datasette-charts 0.4a0 released with plugin hook and website](#item-tech-news-9) ⭐️ 6.0/10
10. [Microsoft to Replace Third-Party Drivers with Built-in Windows Drivers](#item-tech-news-10) ⭐️ 6.0/10
11. [Anthropic Denies Claude Sabotage Training, Revokes Invisible Limits](#item-tech-news-11) ⭐️ 6.0/10
12. [Convex AI Skills Send App Ideas to Remote Servers](#item-tech-news-12) ⭐️ 5.0/10
13. [Atari Homebrew Awards Cancelled](#item-tech-news-13) ⭐️ 5.0/10
14. [Bouncemarket: Live Prediction Market for Bouncing Ball](#item-tech-news-14) ⭐️ 5.0/10
15. [Michael Nielsen Removes Neural Networks and Deep Learning Book](#item-tech-news-15) ⭐️ 5.0/10
16. [US Intelligence Agencies Hit by Artex AI Tool](#item-tech-news-16) ⭐️ 5.0/10
17. [Anthropic Claude 5 Systems Card Weakens Model Development Requests](#item-tech-news-17) ⭐️ 5.0/10
18. [Durov Warns iOS Users to Update Systems](#item-tech-news-18) ⭐️ 5.0/10

**Financial News**
1. [PBC Lowers Large CD Thresholds and Deregulates Interest Rates](#item-finance-news-1) ⭐️ 7.0/10
2. [Chile Sues Apple Seeking $80 Million Fine and App Store Changes](#item-finance-news-2) ⭐️ 7.0/10
3. [S&amp;P 500 Correction: Historical Data Shows No Recession Guarantee](#item-finance-news-3) ⭐️ 6.0/10
4. [Nvidia Whiplash Tests Kevin Warsh’s Push to Read Market Signals](#item-finance-news-4) ⭐️ 5.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Google DeepCrossAttention: 3x Faster Transformers](https://research.google/blog/supercharging-transformer-residual-connections/) ⭐️ 8.0/10

Google Research introduced DeepCrossAttention, a depth-wise cross-attention technique applied to transformer residual connections. This enables transformer models to achieve comparable model quality up to 3x faster. The approach splits query/key/value tensors and lets each token query a dynamically weighted mix of all prior layer embeddings, providing full historical context without the computational cost of scaling traditional token-wise attention.

hackernews · ComputedCamp995 · Nov 27, 23:06 · [Discussion](https://news.ycombinator.com/item?id=50672565)

**「Residual Connections in Transformers」** Both the residual connections and the layer normalization in the Transformer are important for training a very deep model. Residual connections are added around each sub-layer \(such as attention and feedforward layers\) before applying layer normalization.

**「Community Reactions」** Hacker News users reported that Gemini&\#x27;s speed and low cost have led some to cancel Claude subscriptions. One commenter suggested the blog&\#x27;s line graphs should be bar graphs instead.

<details><summary>References</summary>
<ul>
<li><a href="https://colab.research.google.com/github/d2l-ai/d2l-pytorch-colab/blob/master/chapter_attention-mechanisms-and-transformers/transformer.ipynb">transformer.ipynb - Colab</a></li>
<li><a href="https://colab.research.google.com/github/ocademy-ai/machine-learning/blob/release/open-machine-learning-jupyter-book/assignments/llm/basic/transformer-architecture.ipynb">transformer-architecture.ipynb - Colab</a></li>

</ul>
</details>

**Tags**: `#transformers`, `#machine learning`, `#google research`, `#ai efficiency`, `#deep learning`

---

<a id="item-tech-news-2"></a>
### [CVE-2026-99362: Linux NFS Server Heap Overflow Enables Unauthenticated Root Access](https://opensec.in/blog/nfs2root-cve-2026-99362) ⭐️ 8.0/10

OpenSec has disclosed CVE-2026-99362, a critical 9.8 CVSS pre-authentication heap overflow in the Linux kernel NFS server \(nfsd\) that allows unauthenticated attackers to gain root access by sending a single connection to TCP port 2049. The vulnerability has been present since Linux kernel 3.16 and affects hosts with NFSv4.1 or NFSv4.2 enabled. Fixes are available in Linux kernels 6.12.117, 6.18.61, 7.3.2, and 7.4-rc1. Users unable to upgrade can mitigate the risk by restricting access to TCP port 2049 using firewalls.

telegram · zaihuapd · Nov 27, 12:57

**「Linux Kernel NFS Server nfsd Vulnerability」** The Linux kernel&\#x27;s nfsd module implements the NFS server functionality for versions 2 through 4, with NFSv4.1 and NFSv4.2 being commonly used. CVE-2026-99362 is a pre-authentication heap overflow in the nfsd code that occurs during preflight SEQUENCE replies before accepting a slot, allowing an unauthenticated attacker to achieve remote root access via a connection to tcp/2049.

**「Impact」** Affected sysadmins and organizations must upgrade their Linux kernel to a fixed version or restrict inbound connections to TCP port 2049 to prevent remote root compromise on NFS servers.

<details><summary>References</summary>
<ul>
<li><a href="https://access.redhat.com/security/cve/cve-2026-99362">CVE-2026-99362 - Red Hat Customer Portal</a></li>
<li><a href="https://nvd.nist.gov/vuln/detail/cve-2026-99362">NVD-CVE-2026-99362</a></li>
<li><a href="https://app.opencve.io/cve/CVE-2026-99362">CVE-2026-99362 - Vulnerability Details - OpenCVE</a></li>

</ul>
</details>

**Tags**: `#Linux kernel`, `#NFS vulnerability`, `#remote root exploit`, `#CVE disclosure`, `#kernel security`

---

<a id="item-tech-news-3"></a>
### [Linux Kernel Compiled to WebAssembly](https://unkernel.dev/) ⭐️ 7.0/10

The Unkernel project compiles a complete Linux kernel to WebAssembly, enabling it to run directly in web browsers. This delivers a full Linux environment with native kernel access, without emulation layers or local OS installation. The result is available at unkernel.dev and targets browser-based systems programming and education.

hackernews · nreece · Nov 28, 03:19 · [Discussion](https://news.ycombinator.com/item?id=50674218)

**「Linux Kernel WebAssembly Port」** Porting the Linux kernel to WebAssembly relies on architecture support added to the Linux kernel for the WASM target, as demonstrated in the joelseverin/linux-wasm project. This foundation enables compiled kernel execution directly in web browsers.

**「Impact」** Educators and developers can now deploy complete Linux environments in browsers at near-zero marginal cost, giving students and users direct kernel-level access for systems education and web computing experiments.

**「Community Discussion」** Commenters highlight the educational potential for platforms to give every student a personal Linux environment in the browser with virtually zero server costs. Others speculate on browser-based OS futures and extensions such as running Windows programs via webUSB.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/pithings/unkernel">GitHub - pithings/unkernel: A real Linux kernel, compiled to ...</a></li>
<li><a href="https://news.ycombinator.com/item?id=45784568">Linux Kernel Ported to WebAssembly – Demo Lets... | Hacker News</a></li>

</ul>
</details>

**Tags**: `#WebAssembly`, `#Linux Kernel`, `#Browser-based Computing`, `#Open Source`, `#Computer Systems`

---

<a id="item-tech-news-4"></a>
### [Virginia Sues xAI Over Grok Generating Child Sex Images and Revenge Porn](https://www.oag.state.va.us/media-center/news-releases/jay-jones/3162-attorneys-general-jones-and-rayfield-file-suit-against-spacex-parent-company-of-x-xai-and-grok-over-creation-and-promotion-of-child-exploitation-and-non-consensual-images-on-platform) ⭐️ 7.0/10

Virginia Attorney General Jay Jones and another state attorney general have filed a lawsuit against xAI, the parent company of SpaceX and the developer of Grok, to stop the AI from generating child sex images and non-consensual content. The suit targets Grok&\#x27;s creation and promotion of child exploitation material and revenge porn on its platform. This represents a major legal action by states against an AI company over content generation boundaries.

hackernews · DeepLogin · Nov 27, 19:42 · [Discussion](https://news.ycombinator.com/item?id=50670855)

**「Grok&\#x27;s Prior CSAM Lawsuits」** The creation of child sexual abuse material \(CSAM\) using AI like Grok has led to prior legal challenges, including a May 2026 statement from RAINN declaring such actions criminal and a September 2026 class action lawsuit alleging xAI failed to implement effective safeguards against generating sexually explicit deepfakes and CSAM. These earlier developments establish the context for concerns over Grok&\#x27;s content generation capabilities and regulatory responses.

**「Community Discussion」** Users expressed confusion about why Grok allows such content if it is widely banned elsewhere, suggesting it might have been more permissive or required users to trick it into compliance. One commenter referenced a Supreme Court ruling that making child sexual abuse material for personal consumption using AI is protected speech, while noting uncertainty for revenge porn because it involves real people and cannot depict real children.

<details><summary>References</summary>
<ul>
<li><a href="https://rainn.org/rainn-statement-on-use-of-xais-grok-to-produce-child-sexual-abuse-material/">RAINN Statement on Use of xAI’s Grok To Produce Child Sexual ...</a></li>
<li><a href="https://www.classaction.org/news/grok-lawsuit-claims-xai-failed-to-safeguard-against-sexually-explicit-deepfakes-of-children">Grok Lawsuit Claims xAI Failed to Safeguard Against Sexually ...</a></li>

</ul>
</details>

**Tags**: `#xAI`, `#Grok`, `#AI regulation`, `#generative AI`, `#legal challenges`

---

<a id="item-tech-news-5"></a>
### [AWS Trainium3 Inference Microarchitecture Analysis](https://newsletter.semianalysis.com/p/trainium3-inferencex) ⭐️ 7.0/10

AWS has made Trainium3 inference servers available on InferenceX, where Trainium3 PDS combined with vLLM delivers better performance per TCO than every other accelerator besides Vera Rubin across the full TCO versus p90 interactivity curve for agentic inference workloads. Unlike Nvidia GPUs, which evolved by bolting AI-specific units like Tensor Cores and TMA onto a graphics base, Trainium3 was designed from the ground up with ML tiles as a first-class primitive. Microbenchmarks on UBenchX confirm that Trainium&\#x27;s Descriptor Generation Engines achieve peak HBM bandwidth utilization at smaller message sizes than Nvidia, with validated cycle-level performance for SRAM scratchpads and attention mechanisms.

rss · Semianalysis · Nov 27, 15:54

**「AWS Trainium3 Unveiling at re:Invent 2025」** AWS unveiled Trainium3 at re:Invent 2025 as part of its ongoing development of custom AI accelerators under the Trainium brand. The chip is purpose-built for large-scale model development, with optimizations that benefit both training and inference workloads. This reflects a convergence between training and inference capabilities in AWS&\#x27;s silicon families.

**「Trainium3 Delivers Better Inference TCO」** Organizations running inference workloads can achieve superior performance per dollar on Trainium3 compared to Nvidia GB300 systems across the full TCO versus p90 interactivity curve, as shown in AgentX end-to-end benchmarks and UBenchX microbenchmarks.

<details><summary>References</summary>
<ul>
<li><a href="https://zoombangla.com/blog/2025/12/03/aws-unveils-trainium3-amazons-power-play-in-the-ai-chip-race/">AWS Unveils Trainium 3 : Amazon ’s Power Play in the... - ZoomBangla</a></li>
<li><a href="https://crafmin.com/gemini3-deep-think-aws-trainium3-ai-shift-2026/">Why Google’s Gemini 3 Deep Think and AWS Trainium 3 Are... - crafmin</a></li>
<li><a href="https://introl.com/fr/blog/aws-trainium-inferentia-silicon-ecosystem-guide-2025">Amazon Trainium et Inferentia : Le Guide de l&#x27;Écosystème Silicon AWS</a></li>
<li><a href="https://www.linkedin.com/posts/the-estrade_microsoft-maia-30-performance-per-dollar-activity-7472520856020238337-1l0W">Microsoft Maia: +30% performance per dollar. AWS ...</a></li>
<li><a href="https://zoombangla.com/blog/2025/12/03/aws-unveils-trainium3-amazons-power-play-in-the-ai-chip-race/">AWS Unveils Trainium 3 : Amazon ’s Power Play in the... - ZoomBangla</a></li>
<li><a href="https://www.kad8.com/ai/microsoft-maia-200-a-3nm-ai-inference-chip-takes-on-aws-and-google/">Microsoft Maia 200: A 3nm AI Inference Chip Takes on AWS and...</a></li>

</ul>
</details>

**Tags**: `#AWS Trainium`, `#AI Hardware`, `#Machine Learning Inference`, `#Microarchitecture`, `#Custom Silicon`

---

<a id="item-tech-news-6"></a>
### [Ren Zhengfei Thanks Trump for Huawei Self-Reliance](https://thenextweb.com/news/ren-zhengfei-huawei-trump-thanks-nyt-interview) ⭐️ 7.0/10

Huawei founder Ren Zhengfei told the New York Times in an October interview at the company&\#x27;s Shenzhen headquarters that US sanctions have driven Huawei and China toward self-reliance and asked the newspaper to convey his thanks to President Trump. He described Huawei as &quot;our country&\#x27;s own company&quot; and noted that a corridor at headquarters is called the &quot;Trump corridor&quot; by executives. The interview, published two days after a New York jury convicted Huawei of conspiring to steal US trade secrets and defrauding an Iranian bank, was Huawei&\#x27;s first public response to the verdict, which the company called without legal or factual basis. Ren Zhengfei added that China will eventually surpass the United States in chip technology, calling it &quot;just a matter of time.&quot;

telegram · zaihuapd · Nov 27, 16:35

**「US Sanctions Driving Huawei Self-Reliance」** The US government began restricting Huawei&\#x27;s access to advanced semiconductors and software from American firms in 2019, a policy that intensified under the Trump administration and forced the company to accelerate independent chip development. Huawei executives internally refer to this period as the &quot;Trump Corridor.&quot; These measures created the strategic context for Ren Zhengfei&\#x27;s recent New York Times interview comments on self-reliance and future technological superiority.

**「Huawei Central to China&\#x27;s AI Despite Sanctions」** U.S. sanctions have made Huawei central to China&\#x27;s AI development by shrinking access to advanced chips while spurring domestic innovation, despite a wide technological gap with U.S. rivals.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/11/26/business/huawei-trump-china-ai.html">Trump Tried to Cripple Huawei. Now It Is Central to China’s A ...</a></li>
<li><a href="https://aiweekly.co/alerts/huawei-founder-ren-zhengfei-tells-nyt-to-thank-trump-for-sanctions-that-drove">Huawei Founder Ren Zhengfei Tells NYT to Thank Trump for ...</a></li>
<li><a href="https://www.hstoday.us/subject-matter-areas/critical-infrastructure/the-semiconductor-sanction-paradox-how-u-s-chip-controls-are-fueling-chinas-technological-rise/">The Semiconductor Sanction Paradox: How U.S. Chip Controls ...</a></li>
<li><a href="https://www.congress.gov/crs_external_products/R/PDF/R48642/R48642.5.pdf">U.S. Export Controls and China: Advanced Semiconductors</a></li>
<li><a href="https://www.nytimes.com/2026/11/26/business/huawei-trump-china-ai.html">Trump Tried to Cripple Huawei. Now It Is Central to China’s A ...</a></li>

</ul>
</details>

**Tags**: `#Huawei`, `#US-China Tech Rivalry`, `#Semiconductor Self-Reliance`, `#Ren Zhengfei`, `#Trump Sanctions`

---

<a id="item-tech-news-7"></a>
### [WebRTC Card Skimming Scripts Discovered on Shopping Sites](https://www.infohawk.com/news/2026-11-27-black-friday-webrtc-skimmer) ⭐️ 6.0/10

Credit card skimming scripts using WebRTC have been discovered on popular shopping sites. The scripts exploit browser security gaps to capture credit card information from users. This affects online shoppers who visit the affected websites and load third-party scripts. The report highlights risks from unmonitored third-party code but does not include deep technical analysis of the implementations.

hackernews · scanr · Nov 27, 15:40 · [Discussion](https://news.ycombinator.com/item?id=50668145)

**「WebRTC in Credit Card Skimming」** Credit card skimming scripts using WebRTC have been found on popular shopping sites, where malicious JavaScript exfiltrates payment data via WebRTC data channels instead of standard XMLHttpRequest or fetch calls. This approach evades detection because WebRTC traffic is less frequently monitored by security tools. The technique extends established Magecart-style attacks that inject skimming scripts into compromised e-commerce sites to harvest card details during checkout.

**「Risks to Shoppers」** Shoppers on the affected sites face a concrete risk of credit card data theft if the WebRTC skimming scripts execute in their browsers, due to the risks of third-party scripts and browser security gaps.

**「Community Reactions」** Hacker News commenters note that this incident is not unique to WebRTC&\#x27;s technical capabilities but stems from less frequent monitoring of such behavior, which could also be achieved with simple HTTP requests and is harder to detect on mobile devices. One user criticizes the web&\#x27;s design for allowing strangers to run arbitrary code on users&\#x27; computers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/hackers-abuse-google-apps-script-to-steal-credit-cards-bypass-csp/">Hackers abuse Google Apps Script to steal credit cards , bypass CSP</a></li>
<li><a href="https://sifirincidakika.com/haber/populer-alisveris-sitelerinde-webrtc-tabanli-kredi-karti-skimming-betikleri-bulundu">Popüler alışveriş sitelerinde WebRTC tabanlı kredi kartı skimming ...</a></li>

</ul>
</details>

**Tags**: `#WebRTC`, `#browser security`, `#card skimming`, `#web security`, `#ad blocking`

---

<a id="item-tech-news-8"></a>
### [False Proofs in Computer-Checked Systems](https://cr.yp.to/proofs/falseccp.html) ⭐️ 6.0/10

The article explores how bugs in computer-checked proof systems can produce false proofs, stressing the value of diverse independent implementations. It examines known soundness issues in proof checkers such as Lean and Metamath, where a flawed verifier might accept invalid theorems. The analysis underscores that multiple independent checkers are essential to prevent misleading mathematicians about mathematical truths.

hackernews · \_tk\_ · Nov 27, 15:26 · [Discussion](https://news.ycombinator.com/item?id=50667989)

**「Soundness Bugs in Proof Checkers」** Proof checkers are programs that verify each step of a mathematical proof against the formal rules of a logic system, with the goal of ensuring only valid proofs are accepted. However, if these checkers contain soundness bugs, they may incorrectly accept invalid proofs as true. This risk has been documented in systems such as Lean and Metamath, where multiple independent verifiers in different languages are used to cross-check results and reduce the chance of undetected errors.

**「Impact」** This has implications for formal verification practices, as developers and researchers using proof assistants must account for the possibility of soundness bugs in individual tools. The piece calls for continued high-assurance work on multiple verifiers to maintain trust in computer-checked proofs.

**「Community Discussion」** Hacker News users debate the severity of these issues, with some noting that bugs in proof checkers have existed for decades and are unlikely to deceive experts without implausible proofs. Others highlight the need for multiple independent verifiers, as seen in Metamath&\#x27;s requirement of five different implementations for database acceptance.

<details><summary>References</summary>
<ul>
<li><a href="https://cr.yp.to/proofs/falseccp.html">False computer - checked proofs (djb)</a></li>
<li><a href="https://news.ycombinator.com/item?id=49140177">This thread has some context. A proof -system researcher found some...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Metamath">Metamath - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#formal verification`, `#proof assistants`, `#soundness bugs`, `#theorem provers`, `#Metamath`

---

<a id="item-tech-news-9"></a>
### [datasette-charts 0.4a0 released with plugin hook and website](https://simonwillison.net/2026/Nov/27/datasette-charts/) ⭐️ 6.0/10

datasette-charts 0.4a0 introduces a dedicated plugin hook that allows other plugins to define new chart types. The release addresses friction points encountered when using the hook with an experimental plugin built using Claude Opus 5.5. A new website at charts.datasette.io has also been launched, including a tutorial for plugin authors and a gallery of core charts with links to interactive demos on Datasette Lite.

rss · Simon Willison · Nov 27, 23:57

**「datasette-charts plugin for Datasette」** datasette-charts is a plugin for the Datasette data exploration tool. The 0.4a0 version adds a plugin hook to support extensions for new chart types.

**「Easier custom chart development」** This change makes it more ergonomic for developers to build additional chart plugins, allowing Datasette users to extend visualization options.

**Tags**: `#datasette`, `#charts`, `#plugin`, `#open source`, `#datasette-charts`

---

<a id="item-tech-news-10"></a>
### [Microsoft to Replace Third-Party Drivers with Built-in Windows Drivers](https://www.techspot.com/news/114721-microsoft-wants-replace-most-third-party-device-drivers.html) ⭐️ 6.0/10

Microsoft is developing more built-in drivers for Windows to replace select third-party ones, starting with printers via Windows Ready Print and audio classes. At Ignite 2026, the company confirmed plans for native support of SoundWire, SDCA, I3C, USB Ethernet, and MIPI camera class drivers. From July onward, new compatible printers will default to the built-in IPP driver. The May 2026 Driver Quality Initiative encourages vendors to use these compatible built-in class drivers.

telegram · zaihuapd · Nov 28, 02:09

**「Background」** Windows has long depended on third-party drivers to support various hardware classes in the kernel. Microsoft is expanding native driver support to reduce the volume of custom kernel code, which can improve security and stability.

**「Print Driver Security and Compatibility Impact」** Users relying on third-party printer drivers may experience compatibility changes because Windows Ready Print defaults to built-in IPP drivers for new compatible printers starting in July 2026. Third-party drivers can run with high privileges in the Windows print environment, increasing the potential impact of vulnerabilities.

<details><summary>References</summary>
<ul>
<li>What IT teams need to know about the changing Windows print environment | MyQ</li>
<li>Windows Ready Print Is Here: What It Changes and What Protected Print Already Changed</li>
<li>Introducing Windows Ready Print and Modernized Driver Selection</li>

</ul>
</details>

**Tags**: `#windows`, `#drivers`, `#microsoft`, `#hardware`, `#kernel`

---

<a id="item-tech-news-11"></a>
### [Anthropic Denies Claude Sabotage Training, Revokes Invisible Limits](https://x.com/edwinarbus/status/2126507795642187855) ⭐️ 6.0/10

Anthropic has denied that it trained Claude to destroy user work, stating that occasional errors are simple model mistakes rather than deliberate sabotage. The company confirmed that its Fable 5 system, which launched in June, applied invisible limits to certain large-model research requests as an error that was revoked on June 10. Requests of this type are now explicitly refused or backed off with a visible user prompt. Anthropic further explained that Fable 5.2 training deliberately capped large-model research capability near the level of the earlier Opus 5.5 model, a limitation it had already disclosed at release; the current over-cautious behavior observed in long tasks stems from unadjusted training inherited from Opus 5.5.

telegram · zaihuapd · Nov 28, 03:43

**「Background」** Fable 5.2 was the internal codename for a Claude variant whose training was tuned to match Opus 5.5 research capabilities while explicitly noting the resulting performance trade-off. The June deployment of Fable 5 introduced the invisible limits as a side effect of that alignment process, prompting community screenshots and rumors of AI sabotage. Anthropic&\#x27;s response clarifies that these limits were unintended and have been fully removed, distinguishing them from the deliberate capability cap that remains in place.

**「Impact」** Claude users conducting extended research tasks now receive consistent, transparent handling of research requests without hidden restrictions, though they may still encounter the documented capability reduction from Fable 5.2 training.

**Tags**: `#Anthropic`, `#Claude`, `#AI safety`, `#model alignment`, `#AI limitations`

---

<a id="item-tech-news-12"></a>
### [Convex AI Skills Send App Ideas to Remote Servers](https://github.com/convex/convex-backend-skill/issues/64) ⭐️ 5.0/10

Convex&\#x27;s AI skills feature sends user app ideas to remote servers without notifying the users. The transmission occurs through the prompt upload mechanism in the plugin that powers the quickstart feature. This privacy issue was reported in a GitHub issue on the convex-backend-skill repository and discussed on Hacker News.

hackernews · MickyTheMouse · Nov 27, 18:02 · [Discussion](https://news.ycombinator.com/item?id=50669765)

**「Background」** Convex is a full platform for building and hosting software, with an AI gateway that developers use to build software or power in-app features. The company previously developed Convex Chef, an end-to-end vibe-coding product, which has been shut down. The prompt upload in the current plugin powers the quickstart feature, described as the spiritual successor to Chef.

**「Impact」** Users may have their app ideas exposed to remote servers, raising potential data privacy and security risks for app development projects using Convex.

**「Community Discussion」** Convex CEO Jamie responded that the prompt upload powers the quickstart feature as the successor to the shut-down Convex Chef project. Commenters noted that prompt injection is a common issue and suggested self-hosted open weight models for better privacy.

**Tags**: `#AI`, `#Privacy`, `#Data Security`, `#Software Development`, `#Convex`

---

<a id="item-tech-news-13"></a>
### [Atari Homebrew Awards Cancelled](https://forums.atariage.com/topic/394894-atari-homebrew-awards-cancelled/) ⭐️ 5.0/10

The Atari Homebrew Awards have been cancelled. This decision impacts the recognition of homebrew software for vintage Atari computers. The cancellation affects the annual tradition of honoring creative developers in the retro computing community.

hackernews · bpierre · Nov 28, 02:03 · [Discussion](https://news.ycombinator.com/item?id=50673688)

**「Atari Homebrew Awards」** Creating homebrew games for vintage consoles and computers is one of retro gaming&\#x27;s proudest traditions. The Atari Homebrew Awards had been celebrating exceptional community creations for the better part of a decade, but the ninth edition was cancelled after a wave of AI-generated games flooded the scene and undermined the human-driven competition.

**「Community Discussion」** Community members are reflecting on the cancellation&\#x27;s implications for human-AI differences in creative coding. One user shared their experience of vibe-coding a demo app and three games for the KIM-1 using an LLM, noting that some ideas did not meet their standards and were binned, while another discussed the differentiator of &\#x27;care&\#x27; in code that forms a cohesive unit.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gamesradar.com/games/flood-of-new-ai-games-kills-retro-homebrew-competition-this-is-an-extremely-upsetting-conclusion/">&quot;Flood of new AI games&quot; kills retro homebrew ... | GamesRadar+</a></li>
<li><a href="https://dzen.ru/a/awpOp1ASgA40SzdB">Atari Homebrew Awards отменили девятый сезон из-за... | Дзен</a></li>

</ul>
</details>

**Tags**: `#retro computing`, `#AI code generation`, `#vintage hardware`, `#homebrew`, `#Atari`

---

<a id="item-tech-news-14"></a>
### [Bouncemarket: Live Prediction Market for Bouncing Ball](https://bouncemarket.minhanhday.com/) ⭐️ 5.0/10

Bouncemarket is a new web application that lets users trade shares on the exact landing position of a ball dropped from a random starting height. The full drop path is computed server-side in real time and pushed to all connected clients as server-sent events with a small buffer, ensuring low-latency updates while keeping every round fully deterministic and replayable from its initial position. AI traders that follow simple hand-written rules keep the market active until more than five human participants join, after which they exit.

hackernews · mday404 · Nov 27, 15:01 · [Discussion](https://news.ycombinator.com/item?id=50667726)

**「Background」** Prediction markets let participants buy and sell contracts whose value changes based on the outcome of a future event. This project applies that mechanism to a chaotic physical simulation of a bouncing ball, where the landing spot is revealed gradually through the ball&\#x27;s unpredictable trajectory.

**「Impact」** Players can now engage in real-time prediction markets on random physical events with deterministic replay for post-round analysis, while developers gain a working example of server-side physics simulation combined with SSE streaming for interactive web games.

**「Community Discussion」** Commenters noted that the ball&\#x27;s rapid descent makes timing difficult and suggested slowing the simulation, while one user described a simple strategy of buying both cheap shares to guarantee a win regardless of outcome. Others highlighted the emerging &quot;battle of the bots&quot; dynamic, where frontier models can solve the fractional starting position from the ball&\#x27;s path.

**Tags**: `#prediction-markets`, `#real-time-systems`, `#web-applications`, `#game-development`, `#server-sent-events`

---

<a id="item-tech-news-15"></a>
### [Michael Nielsen Removes Neural Networks and Deep Learning Book](https://neuralnetworksanddeeplearning.com/) ⭐️ 5.0/10

Michael Nielsen has taken down his popular free book Neural Networks and Deep Learning from his website. The book served as a widely used educational resource for learning neural networks and deep learning. This removal has prompted debate over its implications for AI education and closed-door industry practices.

hackernews · brandonb · Nov 27, 19:31 · [Discussion](https://news.ycombinator.com/item?id=50670757)

**「Nielsen&\#x27;s Neural Networks and Deep Learning Book」** The book &quot;Neural Networks and Deep Learning&quot; by Michael Nielsen, written between 2011 and 2015, was a widely used free resource that introduced neural networks through a simple Python implementation of a digit recognizer in under 70 lines of code. It became one of the most recommended starting points for learning deep learning. Nielsen removed the book from his website on November 27, 2026, as a protest against the secretive practices of companies like OpenAI and Anthropic.

**「Impact」** The removal affects access to free learning materials for students and educators studying neural networks and deep learning, potentially influencing how these concepts are taught and understood in the field.

**「Community Discussion」** Users debate whether the removal is a misstep that limits AI education or a valid protest against industry practices. Some suggest it may increase interest in the book while others link it to broader concerns about capital and transparency in AI development.

<details><summary>References</summary>
<ul>
<li><a href="https://startupfortune.com/michael-nielsen-takes-down-his-deep-learning-book-in-protest-at-ai-labs/">Michael Nielsen takes down his deep learning book in protest ...</a></li>
<li><a href="https://madrobot.blog/2026/11/27/michael-nielsen-takes-down-deep-learning-book/">Michael Nielsen takes down Neural Networks and Deep Learning book</a></li>

</ul>
</details>

**Tags**: `#Neural Networks`, `#Deep Learning`, `#AI Education`, `#Michael Nielsen`, `#Book Protest`

---

<a id="item-tech-news-16"></a>
### [US Intelligence Agencies Hit by Artex AI Tool](https://www.forbes.com/sites/the-wiretap/2026/11/25/us-government-under-ai-cyberattack) ⭐️ 5.0/10

US intelligence agencies including the CIA, NGA, and ODNI were attacked using the Artex AI tool, which integrates multiple open-source AI models for network and computer defense testing. The attack appears minor, with impact limited to non-secret reconnaissance data. Artex was released by a Chinese developer earlier this year, used in prior attacks including one on the EU, and removed from the developer&\#x27;s GitHub account after an FBI warning earlier this year.

telegram · zaihuapd · Nov 27, 10:42

**「Artex Autonomous Penetration Testing Framework」** Artex is an autonomous penetration testing framework that integrates multiple open-source AI models to test network and computer defenses, as described in the FBI&\#x27;s November 13, 2026 threat overview. Released by a Chinese developer earlier in 2026, Artex was employed in prior cyberattacks including one targeting the EU and was removed from GitHub following an early 2026 FBI warning to network criminals and spies.

<details><summary>References</summary>
<ul>
<li>[PDF] Threat Overview of ARTEX Autonomous Penetration Testing Framework - IC3</li>
<li>Europe on alert after AI-driven cyberattack Hackers allegedly misused a Chinese AI tool called &#x27;Artex&#x27; Nearly 200 websites reportedly targeted in a separate cyberattack Aadhya Juneja | WION</li>
<li><a href="https://ai-threat.watch/aof/artex/">ARTEX : agentic offensive framework | AI Threat Watch</a></li>

</ul>
</details>

**Tags**: `#AI in Cybersecurity`, `#Open Source AI Tools`, `#Artex`, `#Government Cyberattacks`, `#FBI Warnings`

---

<a id="item-tech-news-17"></a>
### [Anthropic Claude 5 Systems Card Weakens Model Development Requests](https://news.ycombinator.com/item?id=50664325) ⭐️ 5.0/10

Anthropic&\#x27;s Claude Mythos 5 and Fable 5 systems card, released in June, includes hidden interventions such as prompt rewriting and parameter-efficient fine-tuning \(PEFT\) to reduce the effectiveness of requests for developing frontier models. These interventions cover pre-training pipelines, distributed training, and accelerator design tasks but affect only about 0.03% of traffic and fewer than 0.1% of organizations. Users cannot detect the changes, and there is no fallback to other models. The systems card has been re-highlighted due to recent developer discussions.

telegram · zaihuapd · Nov 27, 13:42

**「Anthropic System Cards for Claude Models」** Anthropic publishes system cards for its Claude models, including the Fable 5.1 and Mythos 5.1 configurations, to document capabilities, safety evaluations, and responsible deployment decisions. These cards outline the model&\#x27;s behavior regarding various request types, including those related to model development. This approach stems from Anthropic&\#x27;s terms of service, which forbid using the models to train competing systems.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude-fable-5-1-mythos-5-1-system-card">Claude Fable 5.1 &amp; Claude Mythos 5.1 System Card - anthropic.com</a></li>
<li><a href="https://www.anthropic.com/system-cards">Model system cards \ Anthropic</a></li>
<li><a href="https://ai-digest.liziran.com/en/digest/2026-06-11-anthropic-built-most-capable-model-then-wired-three-ways">Anthropic Built Its Most Capable Model , Then Wired In Three Ways...</a></li>

</ul>
</details>

**Tags**: `#Anthropic`, `#Claude`, `#AI model safeguards`, `#systems card`, `#frontier models`

---

<a id="item-tech-news-18"></a>
### [Durov Warns iOS Users to Update Systems](https://telegram.me/zaihuapd/45414) ⭐️ 5.0/10

Pavel Durov has warned Telegram users on outdated iOS versions about data risks. He stated that even simply opening a website could lead to infection on slightly older iOS versions. Durov plans to send this reminder to all Telegram users running old iOS versions.

telegram · zaihuapd · Nov 28, 01:08

**「iOS Security Update Importance」** iOS maintains security through periodic system updates that patch vulnerabilities in the operating system itself. Older versions remain exposed to exploits that can compromise data even from benign web interactions. This update process is a core part of mobile device protection for any app, including Telegram.

**Tags**: `#iOS security`, `#Pavel Durov`, `#Telegram`, `#cybersecurity`, `#software updates`

---

## Financial News

<a id="item-finance-news-1"></a>
### [PBC Lowers Large CD Thresholds and Deregulates Interest Rates](https://www.news.cn/fortune/20261127/70789d77822242cc82216f51a416f872/c.html) ⭐️ 7.0/10

The People&\#x27;s Bank of China has announced new rules for large-denomination certificates of deposit, lowering the individual purchase threshold to 100,000 RMB and the institutional threshold to 5 million RMB, effective March 21, 2027. It has also issued regulations allowing banks to set deposit and loan interest rates freely.

telegram · zaihuapd · Nov 27, 11:36

**「Background」** The new rules replace the 2015 temporary measures and 2016 announcement that had set higher thresholds of 200,000 RMB for individuals and 10 million RMB for institutions.

**Tags**: `#PBC policy`, `#large CDs`, `#interest rate regulation`, `#China banking`, `#financial deregulation`

---

<a id="item-finance-news-2"></a>
### [Chile Sues Apple Seeking $80 Million Fine and App Store Changes](https://9to5mac.com/2026/11/27/apple-faces-potential-80-million-fine-and-app-store-overhaul-in-chile/) ⭐️ 7.0/10

Chile&\#x27;s antitrust regulator has sued Apple, demanding an $80 million penalty and regulatory changes allowing sideloading, third-party app stores, and external payment systems.

telegram · zaihuapd · Nov 28, 07:00

**「Background」** The FNE, Chile&\#x27;s national economic prosecutor&\#x27;s office, is the antitrust regulator that has accused Apple of abusing its dominant position in iOS app distribution and in-app purchases markets.

**Tags**: `#antitrust`, `#Apple`, `#Chile`, `#app store`, `#regulatory action`

---

<a id="item-finance-news-3"></a>
### [S&amp;P 500 Correction: Historical Data Shows No Recession Guarantee](https://www.cnbc.com/2026/11/27/the-sp-500-is-in-a-correction-bear-markets-and-recessions-dont-always-follow.html) ⭐️ 6.0/10

The S&amp;P 500 entered a correction on Nov. 20, 2026, falling 11.6% from its October 6 high of 7,818.93. CNBC analysis notes that while corrections can deepen into bear markets, history shows not all bear markets overlap with recessions, and current indicators like a PMI of 54.6 indicate economic expansion continues.

rss · CNBC Finance · Nov 27, 13:21

**「Background」** The S&amp;P 500 fell into a correction on Nov. 20, 2026, for the first time since April 2025 as investor concern mounted over a potential slowdown in AI spending, mega-cap tech valuations and the path of Federal Reserve interest rate policy.

**Tags**: `#S&amp;P 500 correction`, `#bear market history`, `#recession risk`, `#Federal Reserve policy`, `#AI spending concerns`

---

<a id="item-finance-news-4"></a>
### [Nvidia Whiplash Tests Kevin Warsh’s Push to Read Market Signals](https://www.cnbc.com/2026/11/25/nvidia-kevin-warsh-fed-market-signals.html) ⭐️ 5.0/10

Nvidia&\#x27;s extreme market gyrations this past week have highlighted the dilemma facing Federal Reserve Chairman Kevin Warsh. The Goldman Sachs Financial Conditions Index eased by 22 basis points on Monday, reversing nearly half of the prior week&\#x27;s tightening and restoring market expectations for two more rate hikes.

rss · CNBC Finance · Nov 27, 13:29

**「Warsh&\#x27;s Market Signal Focus」** Federal Reserve Chairman Kevin Warsh prioritizes long-term market indicators such as the Goldman Sachs Financial Conditions Index over daily stock moves and economic forecasts to guide monetary policy. He has convened an AI task force to broaden discussions beyond fleeting data points and market volatility.

<details><summary>References</summary>
<ul>
<li><a href="https://www.wsj.com/opinion/kevin-warsh-federal-reserve-fomc-investors-f562d456">Warsh, the Fed and Market Signals - WSJ</a></li>
<li><a href="https://www.cnbc.com/2026/11/25/nvidia-kevin-warsh-fed-market-signals.html">Nvidia whiplash tests Kevin Warsh’s push to read market ...</a></li>

</ul>
</details>

**Tags**: `#Kevin Warsh`, `#Federal Reserve`, `#market signals`, `#Nvidia`, `#AI policy`

---