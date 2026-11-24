---
layout: default
title: "Horizon Summary: 2026-11-24 (EN)"
date: 2026-11-24
lang: en
---

> From 35 items, 24 important content pieces were selected

---

**Technology News**
1. [Nvidia Reinstates Jensen Huang as CEO](#item-tech-news-1) ⭐️ 8.0/10
2. [Codex2api Suspected Supply Chain Poisoning](#item-tech-news-2) ⭐️ 8.0/10
3. [Anthropic Formalizes VP ≠ VNP Over Every Field](#item-tech-news-3) ⭐️ 7.0/10
4. [Zhipu AI Releases GLM-5.4 Loop Transformer](#item-tech-news-4) ⭐️ 7.0/10
5. [Ladybird Browser Engine Reaches Alpha](#item-tech-news-5) ⭐️ 7.0/10
6. [Spelunkr.tv: Free TV Channels from Internet Archive Videos](#item-tech-news-6) ⭐️ 7.0/10
7. [Nospeaker: MacBook Trackpad Audio via Haptic Motor](#item-tech-news-7) ⭐️ 7.0/10
8. [datasette-charts 0.1a0](#item-tech-news-8) ⭐️ 7.0/10
9. [Google Builds Mirror Dimension for Chrome AI Agent Testing](#item-tech-news-9) ⭐️ 7.0/10
10. [Starlink Integration in Tesla Vehicles by Late 2027](#item-tech-news-10) ⭐️ 7.0/10
11. [Meta AI Chief Warns of Superintelligence Control Risks](#item-tech-news-11) ⭐️ 7.0/10
12. [Yann LeCun Accuses Dario Amodei of Hyping AI Dangers to Ban Open Models](#item-tech-news-12) ⭐️ 6.0/10
13. [Microsoft Defaults to No 32-bit WoW64 in Windows Server 2028](#item-tech-news-13) ⭐️ 6.0/10
14. [Arm Requests jonpalmisc.com Shutdown on December 4, 2026](#item-tech-news-14) ⭐️ 5.0/10
15. [Apple Removes Open-Source App from EU App Store After 9 Years](#item-tech-news-15) ⭐️ 5.0/10
16. [Win4wine: Windows Shell as Linux Desktop via Wine](#item-tech-news-16) ⭐️ 5.0/10

**Financial News**
1. [Fed&\#x27;s John Williams: Higher rates likely over time to reach 2% inflation target](#item-finance-news-1) ⭐️ 7.0/10
2. [Ant Group Leads $100 Million Investment in Simplexity Robotics at $1.6 Billion Valuation](#item-finance-news-2) ⭐️ 6.0/10
3. [Anthropic Limits IPO Underwriting Team to 4 Bankers, Bans Competitor Work](#item-finance-news-3) ⭐️ 6.0/10
4. [Anthropic IPO Triggers Sell-Off in Chinese Tech Stocks](#item-finance-news-4) ⭐️ 6.0/10
5. [Nvidia Reinstatement of Jensen Huang as CEO Triggers Relief Rally](#item-finance-news-5) ⭐️ 5.0/10
6. [Foundation Future Industries Employees Lose Health Benefits](#item-finance-news-6) ⭐️ 5.0/10
7. [JPMorgan and Hyundai Card Test AI Agents for Autonomous FX Transactions](#item-finance-news-7) ⭐️ 5.0/10
8. [Shanghai Metro Raises Fares After 21 Years](#item-finance-news-8) ⭐️ 5.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Nvidia Reinstates Jensen Huang as CEO](https://www.cnbc.com/2026/11/23/nvidia-jensen-huang-ceo.html) ⭐️ 8.0/10

Nvidia&\#x27;s board has reinstated Jensen Huang as president and CEO and as a board member after a brief ouster. The unanimous decision followed input from senior levels of the United States government, with the board stating that Huang&\#x27;s reinstatement poses no national security risk. The board formed an investigation committee of independent directors to examine reports that Huang was targeted by foreign intelligence activities, with Huang committing to full cooperation, and established a national security and export controls committee while initiating recruitment for a chief compliance officer. Colette Kress, who served as interim CEO, will continue as chief financial officer.

hackernews · jaz · Nov 23, 14:00 · [Discussion](https://news.ycombinator.com/item?id=50611576)

**「Jensen Huang&\#x27;s Resignation Context」** Jensen Huang resigned as Nvidia CEO on November 12, 2026, after reports emerged of his extramarital affairs, including one with an alleged Chinese spy, and the company&\#x27;s alleged complicity in evading U.S. export controls on advanced semiconductors to China.

**「Impact」** The reinstatement provides leadership continuity for Nvidia&\#x27;s AI hardware and semiconductor operations, with the board&\#x27;s confirmation of no national security risk supporting uninterrupted executive direction.

**「Community Discussion」** Users highlight the US government input as the decisive factor in the board&\#x27;s decision, noting the unanimous vote as surprising given the prior ouster. Some community members discuss potential protections for board members under Delaware law precedents and express concerns about perceived hypocrisy in US sanctions policy toward Nvidia compared to other companies.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aljazeera.com/economy/2026/11/23/nvidia-board-reinstates-jensen-huang-as-ceo">Nvidia board reinstates Jensen Huang as CEO | Al Jazeera</a></li>
<li><a href="https://www.theguardian.com/technology/2026/nov/23/jensen-huang-reinstated-as-nvidia-chief-executive">Jensen Huang reinstated as Nvidia CEO | Jensen ... | The Guardian</a></li>
<li><a href="https://foreignpolicy.com/2026/11/23/jensen-huang-nvidia-return-ceo-national-security-scandal/">Jensen Huang &#x27;s Return to Nvidia Is Unprecedented for U . S . National ...</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#Jensen Huang`, `#CEO`, `#AI Hardware`, `#Sanctions`

---

<a id="item-tech-news-2"></a>
### [Codex2api Suspected Supply Chain Poisoning](https://github.com/WormW/codex2api-incident-2026-11) ⭐️ 8.0/10

The Codex2api author account was compromised, enabling an attacker to push a tagged release that bypassed the main branch and embedded a backdoor. Version 3.1.11 removed authentication entirely, allowing passwordless remote command execution. A GitHub Actions workflow also exfiltrated 16 secrets, affecting at least 21 repositories under the compromised account. Users on versions 3.1.10–3.1.12 should immediately stop using the software, revert to 3.1.9, and rotate all related credentials including GitHub tokens, SSH keys, databases, and DeepSeek API keys.

telegram · zaihuapd · Nov 23, 11:21

**「GitHub Releases and Supply Chain Risks」** Open-source software projects are typically hosted on platforms like GitHub, where releases are often managed through tags. Automated workflows can be set up to build and publish packages upon tag creation. An attacker who gains access to the repository can exploit this by pushing a malicious tag, thereby distributing compromised software without altering the default branch.

**「Backdoor and Credential Exposure」** Users who installed or updated Codex2api to versions 3.1.10–3.1.12 face remote code execution without authentication, as the backdoored v3.1.11 release removed auth checks. The hacked account also exfiltrated 16 GitHub Actions secrets, impacting at least 21 repositories. Affected users must immediately revert to 3.1.9 and rotate all related keys including GitHub tokens, SSH keys, databases, and DeepSeek credentials.

<details><summary>References</summary>
<ul>
<li><a href="https://aisafetyradar.org/topic/backdoors_poisoning">Backdoors &amp; Poisoning : AI safety research · AI Safety Radar</a></li>

</ul>
</details>

**Tags**: `#supply-chain-attack`, `#open-source-security`, `#AI-tool-vulnerability`, `#GitHub-secrets-leak`, `#backdoor`

---

<a id="item-tech-news-3"></a>
### [Anthropic Formalizes VP ≠ VNP Over Every Field](https://github.com/anthropics/formal-math/tree/main/vp-vnp) ⭐️ 7.0/10

Anthropic has formalized a proof that VP is not equal to VNP over every field in the Lean theorem prover as part of its formal mathematics project. This is a partial result toward resolving the P versus NP problem in algebraic complexity theory. The formalization is a shipped capability demonstrating AI-assisted theorem proving, with the paper available on GitHub.

hackernews · mikeryan52 · Nov 23, 22:09 · [Discussion](https://news.ycombinator.com/item?id=50620102)

**「VP and VNP in Arithmetic Circuit Complexity」** In algebraic complexity theory, the classes VP and VNP consist of families of polynomials that can be computed by arithmetic circuits of polynomial size and those that can be expressed as the permanent of a matrix with linear entries, respectively. Proving that VP is not equal to VNP over a given field is equivalent to showing that the permanent does not have polynomial-size arithmetic circuits over that field, a longstanding open problem. The recent result establishes this inequality over every field using formal verification in the Lean theorem prover.

**「VP ≠ VNP Separation Claim」** The Anthropic formal proof claiming VP ≠ VNP over every field would separate the classes in algebraic complexity theory by showing the permanent has no polynomial size circuits. However, this remains an open problem as per standard references.

**「Community Discussion」** Users describe the result as a partial step in the P vs NP effort and speculate on its impact on mathematics graduate students, noting that problems could be solved by AI in a year. One comment points out the paper&\#x27;s unanalyzed relation to relativization and algebrization.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Arithmetic_circuit_complexity">Arithmetic circuit complexity - Wikipedia</a></li>
<li><a href="https://hexagonmath.org/2611.00954v1">VP ||#92;neq$ VNP over every field · Hexagon</a></li>
<li><a href="https://en.wikipedia.org/wiki/Lean_%28proof_assistant%29">Lean (proof assistant) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Arithmetic_circuit_complexity">Arithmetic circuit complexity - Wikipedia</a></li>
<li><a href="https://www.kongchang.com/en/articles/vp-vnp-a-major-breakthrough-in-computational-complexity-theory">VP ≠ VNP: A Major Breakthrough in Computational Complexity ...</a></li>
<li><a href="https://link.springer.com/chapter/10.1007/978-3-662-03338-8_21">P Versus NP: A Nonuniform Algebraic Analogue - Springer</a></li>

</ul>
</details>

**Tags**: `#algebraic complexity theory`, `#formal verification`, `#Lean theorem prover`, `#P vs NP`, `#AI-assisted mathematics`

---

<a id="item-tech-news-4"></a>
### [Zhipu AI Releases GLM-5.4 Loop Transformer](https://z.ai/blog/glm-5.4) ⭐️ 7.0/10

Zhipu AI has released GLM-5.4, its first model using a looped transformer architecture. In this design, a group of weight-shared layers runs for multiple iterations per forward pass, refining hidden states from the previous iteration to deepen the effective network depth without increasing the parameter count. The model is now available through the Z.ai API via a required Coding Plan subscription and uses the same OpenAI-compatible Responses API format as the regular plan.

hackernews · foohis · Nov 23, 10:06 · [Discussion](https://news.ycombinator.com/item?id=50609685)

**「Loop Transformer Architecture」** In a standard transformer, each layer runs once per forward pass, pairing distinct sets of weights for attention and feed-forward networks. Loop transformers instead apply a group of weight-shared layers multiple times within each forward pass, iteratively refining hidden states from the previous iteration. This looped-depth sharing or recurrent-depth approach creates deeper networks without increasing parameter count and optimizes memory bandwidth bottlenecks during inference.

**「Developer and User Impact」** Developers and users gain access to GLM-5.4 for generalized coding tasks through the OpenAI-compatible API, with the potential for improved reasoning on agentic coding without added parameters. However, the model is not yet released as open weights and requires a paid Coding Plan subscription for API access.

**「Community Reactions」** Users highlight Zhipu AI&\#x27;s transparency in sharing technical details as a refreshing contrast to Western AI companies and see looped transformers as a logical next step for SOTA LLMs. Some note the model&\#x27;s &\#x27;marathon thinking&\#x27; behavior causes delays on simple tasks, while one comment explains the architecture&\#x27;s optimization of memory bandwidth bottlenecks during inference.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Transformer_%28deep_learning%29">Transformer (deep learning) - Wikipedia</a></li>
<li><a href="https://techstackups.com/articles/loop-architecture-explained/">Loop Architecture Explained: Why Looped Transformers Are ...</a></li>
<li><a href="https://sebastianraschka.com/llm-architecture-gallery/looped-depth-sharing/">Looped Transformer | Sebastian Raschka, PhD</a></li>

</ul>
</details>

**Tags**: `#loop transformers`, `#GLM-5.4`, `#LLM architecture`, `#Zhipu AI`, `#coding models`

---

<a id="item-tech-news-5"></a>
### [Ladybird Browser Engine Reaches Alpha](https://ladybird.org/posts/alpha/) ⭐️ 7.0/10

Ladybird, the open-source browser engine from the SerenityOS project, has entered its first alpha stage. Users can now download and install the browser directly on macOS and Linux without compiling it themselves. Early testing shows strong web compatibility for complex sites and WebAssembly applications, with tabs isolated in separate processes and recent AI-assisted improvements boosting Web Platform Tests passes to surpass Safari.

hackernews · janvdberg · Nov 23, 16:13 · [Discussion](https://news.ycombinator.com/item?id=50614249)

**「Ladybird: SerenityOS Browser Engine」** Ladybird is a new web browser engine developed from scratch as part of the SerenityOS operating system project, which aims to create a complete Unix-like OS in C++. The engine implements its own HTML parsing, CSS engine, layout, JavaScript engine, and WebAssembly support, reusing code from SerenityOS while depending on external components like HarfBuzz and Skia. Alpha builds are now available for download on macOS and Linux without requiring compilation.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Ladybird_%28web_browser%29">Ladybird (web browser) - Wikipedia</a></li>
<li><a href="https://ladybird.org/">Ladybird</a></li>
<li><a href="https://ladybird.org/posts/alpha/">Ladybird is now in alpha - Ladybird</a></li>

</ul>
</details>

**Tags**: `#Ladybird Browser`, `#SerenityOS`, `#Browser Engine`, `#Open Source`, `#Web Rendering`

---

<a id="item-tech-news-6"></a>
### [Spelunkr.tv: Free TV Channels from Internet Archive Videos](https://spelunkr.tv/) ⭐️ 7.0/10

Spelunkr.tv has launched as a free, ad-supported streaming service that curates forgotten videos from the Internet Archive into themed on-demand TV channels. Users can access channels such as 2am Theater, which features drive-in movie double features with related previews and interstitial material, and Headbangers Ball, a 1987 classic rock program. The project assembles public-domain and user-uploaded content from the Internet Archive to create an alternative media streaming experience without traditional cable subscriptions.

hackernews · SockThief · Nov 23, 01:13 · [Discussion](https://news.ycombinator.com/item?id=50606192)

**「Retro Cable TV from the Internet Archive」** Internet Archive videos including cartoons, B-movies, old commercials and oddities are curated into themed channels. Spelunkr.tv runs 34 channels of 24/7 synchronized retro cable television from these materials, offering free streaming without signup.

**「Community Discussion」** Users have praised Spelunkr.tv for reviving forgotten content, reporting hours spent watching channels like Headbangers Ball and appreciating the nostalgic drive-in style of 2am Theater. Several commenters have shared DIY alternatives using Raspberry Pi hardware and Internet Archive sources, showing the project&\#x27;s influence on media enthusiasts building similar setups.

<details><summary>References</summary>
<ul>
<li><a href="https://spelunkr.tv/">SPELUNKR — Cable TV, but weirder</a></li>
<li><a href="https://spelunkr.tv/directory">directory — SPELUNKR</a></li>
<li><a href="https://spelunkertv.online/">Spelunkr TV — 34 Channels of 24/7 Retro Cable TV, Free</a></li>

</ul>
</details>

**Tags**: `#Internet Archive`, `#digital preservation`, `#media streaming`, `#open source`, `#alternative media`

---

<a id="item-tech-news-7"></a>
### [Nospeaker: MacBook Trackpad Audio via Haptic Motor](https://github.com/os6/nospeaker) ⭐️ 7.0/10

Nospeaker is an open-source macOS tool that generates audible audio from a MacBook&\#x27;s trackpad by driving its haptic motor at frequencies up to 4 kHz. It reads text using macOS TTS and modulates the haptic feedback through the private MultitouchSupport framework, producing vibrations audible to the human ear between 100 Hz and 4 kHz. The project requires a Force Touch trackpad and has been tested on the M5 Max MacBook Pro, but is limited to text output only.

hackernews · yakkomajuri · Nov 23, 11:31 · [Discussion](https://news.ycombinator.com/item?id=50610318)

**「Driving Trackpad Haptics at Audio Frequencies」** MacBook trackpads contain a small haptic motor beneath the glass that vibrates to simulate clicks and taps as part of Apple&\#x27;s haptic feedback system. Normally limited to low frequencies for tactile sensation, driving the motor at audio frequencies up to 4,000 times per second causes the trackpad surface to produce audible sound waves. The open-source nospeaker project takes advantage of this by using a private macOS framework to control the motor at these high frequencies, paired with macOS text-to-speech to read out text as voice.

**「Community Discussion」** Users find the haptic feedback surprisingly convincing, as if the trackpad is actually being clicked. Community members also draw parallels to historical hardware hacks such as using the Commodore 1541 floppy drive motor for audio output and note Apple&\#x27;s sum-of-sines representation for controlling the haptic motor.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/os6/nospeaker">GitHub - os 6 / nospeaker : make your macbook &#x27;s trackpad talk using...</a></li>
<li><a href="https://www.macrumors.com/2026/11/23/macbook-trackpad-turns-into-a-speaker/">Developer Turns MacBook Trackpad Into a Speaker Using Haptic ...</a></li>
<li><a href="https://www.youtube.com/watch?v=YvheuEyHFPo">This Developer Made a MacBook Talk Without Speakers . - YouTube</a></li>

</ul>
</details>

**Tags**: `#haptic feedback`, `#trackpad audio`, `#open-source project`, `#hardware integration`, `#vibration synthesis`

---

<a id="item-tech-news-8"></a>
### [datasette-charts 0.1a0](https://simonwillison.net/2026/Nov/23/datasette-charts/) ⭐️ 7.0/10

The datasette-charts 0.1a0 plugin has been released for Datasette, enabling interactive line charts and other visualizations directly in Datasette Lite. Prototyped rapidly with Claude AI after over a year of development, the plugin supports any table or SQL query using D3, Observable Plot, and topojson-client libraries. Charts now account for all rows in the result set via aggregated SQL queries \(using GROUP BY, time bucketing, and window functions\), with suggestions based on sampling, and the current chart state is persisted in the URL fragment.

rss · Simon Willison · Nov 23, 00:37

**「Datasette Visualization Plugins」** Plugins extend Datasette with new functionality including visualization options. Earlier examples include the datasette-chart plugin that adds interactive charts using Chart.js and the datasette-dashboards plugin for creating dashboards. This is all documented on the official Datasette plugins page.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/r-curio/datasette-chart">GitHub - r-curio/datasette-chart: A Datasette plugin that ...</a></li>
<li><a href="https://github.com/rclement/datasette-dashboards">GitHub - rclement/datasette-dashboards: Datasette plugin to ...</a></li>
<li><a href="https://datasette.io/plugins">Datasette Plugins</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#charts`, `#open source`, `#AI`, `#software engineering`

---

<a id="item-tech-news-9"></a>
### [Google Builds Mirror Dimension for Chrome AI Agent Testing](https://www.landian.news/archives/128701.html) ⭐️ 7.0/10

Google has constructed Mirror Dimension, an isolated simulated internet environment containing thousands of sites, to test Chrome AI agents on tasks like browsing, searching, logging in, adding to cart, and completing transactions. Engineers run over 1,000 daily test cases in isolation, with a focus on defending against prompt injection attacks from malicious web content.

telegram · zaihuapd · Nov 23, 01:30

**「Mirror Dimension: Synthetic Web for Chrome AI Agent Testing」** Google has built Mirror Dimension, a synthetic version of the web, to safely test its Chrome AI agents. This controlled environment allows engineers to evaluate how agents perform tasks such as browsing, searching, and completing transactions in realistic online settings. It helps address security concerns by providing an isolated space to train and validate AI systems without risking real-world interactions or prompt injection attacks.

**「Impact」** This internal testing environment supports safer development of Chrome AI agents by providing a controlled sandbox that mitigates risks from real-world web interactions and prompt injection vulnerabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/security/mirror-dimension-for-agents/">Mirror Dimension for Agents: Evaluating Browser-Use Agents ...</a></li>
<li><a href="https://www.wired.com/story/google-built-a-giant-mirror-dimension-internet-to-test-its-chrome-ai-agents/">Google Built a Giant ‘Mirror Dimension’ Internet to Test Its ...</a></li>
<li><a href="https://indianexpress.com/article/technology/artificial-intelligence/google-mirror-dimension-explained-fake-internet-ai-agents-10975011/">What is Google’s ‘Mirror Dimension’, the fake internet built ...</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#prompt injection`, `#Chrome AI`, `#AI safety testing`, `#Google Mirror Dimension`

---

<a id="item-tech-news-10"></a>
### [Starlink Integration in Tesla Vehicles by Late 2027](https://x.com/elonmusk/status/2124673053246312848) ⭐️ 7.0/10

Elon Musk stated that Starlink integration in Tesla vehicles is expected around the end of 2027. This capability is intended to support unsupervised Full Self-Driving \(FSD\) operations and provide entertainment and work opportunities for passengers. However, the feature will not be available in China due to local regulations prohibiting Starlink.

telegram · zaihuapd · Nov 23, 03:33

**「Starlink Regulatory Status in China」** Starlink has faced outright bans in China since at least 2007, when the People&\#x27;s Liberation Army conducted a kinetic weapons test against a Feng Yun satellite, prompting national security restrictions that continue to prohibit commercial satellite internet services. As of September 2026, no commercial, diplomatic, or emergency exemptions have been granted in mainland China, with no pending SpaceX applications in MIIT records. This regulatory prohibition directly accounts for the exclusion of China from Elon Musk&\#x27;s announced late-2027 Starlink integration in Tesla vehicles.

<details><summary>References</summary>
<ul>
<li><a href="https://starlink-news.com/2026/09/19/starlink-country-approvals-2026-licences-bans-prices/">Starlink Country Approvals 2026: Licences, Bans, Prices</a></li>
<li><a href="https://starlink-news.com/2026/09/19/starlink-in-china-ban-price-and-legal-satellite-internet/">Starlink in China: Ban, Price and Legal Satellite Internet</a></li>
<li><a href="https://starlinkinsider.com/starlink-china/">Starlink and China: Background (2026) - Starlink Insider Mapped: Where Starlink Is Available Around the World (May 2026) Starlink Gen 3 China: 2026 Regulatory Outlook - accio.com Starlink Price China 2026: Banned &amp; Illegal - accio.com China regulations on Satellite communications: Starlink</a></li>

</ul>
</details>

**Tags**: `#Starlink`, `#Tesla`, `#FSD`, `#Autonomous Driving`, `#Elon Musk`

---

<a id="item-tech-news-11"></a>
### [Meta AI Chief Warns of Superintelligence Control Risks](https://thenextweb.com/news/metas-ai-chief-says-superintelligence-is-arriving-and-control-is-at-risk) ⭐️ 7.0/10

Meta AI chief Alexandr Wang posted on X that superintelligence is no longer a distant future matter. He cited the example of mathematician Levent Alpöge using Anthropic&\#x27;s Claude to complete a proof of the Riemann hypothesis, which was machine-verified by the Lean and Mathlib community on Saturday. Wang warned that controlling self-improving AI systems 1000 times smarter than humans is extremely difficult, calling for urgent research into AI safety, alignment, and protection. The proof currently lacks a human-readable version.

telegram · zaihuapd · Nov 23, 12:49

**「Background」** The recent formal proof of the Riemann hypothesis using AI assistance in Lean and Mathlib exemplifies the growing role of large language models in formal mathematical verification. This development makes the challenges of AI alignment and control more relevant as systems demonstrate capabilities that approach or exceed human expertise in specific domains.

**「Impact」** The warning highlights the critical need for accelerated investment in AI alignment research to address the risks of losing control over self-improving artificial intelligence systems that could be thousands of times more capable than humans.

**Tags**: `#AI safety`, `#superintelligence`, `#Meta AI`, `#AI alignment`, `#formal verification`

---

<a id="item-tech-news-12"></a>
### [Yann LeCun Accuses Dario Amodei of Hyping AI Dangers to Ban Open Models](https://twitter.com/ylecun/status/2124550037912920090) ⭐️ 6.0/10

Yann LeCun tweeted that Anthropic&\#x27;s Dario Amodei has been hyping AI dangers since GPT-2 to push regulations that would make open-source models illegal and keep him in control. The accusation has sparked a popular Hacker News thread with 1,023 upvotes and 595 comments debating regulatory tactics to restrict open-weight models. Users discuss proposals such as microcode updates limiting consumer GPUs and requiring registration for privately owned compute.

hackernews · MrBuddyCasino · Nov 23, 17:07 · [Discussion](https://news.ycombinator.com/item?id=50615308)

**「LeCun Accuses Amodei of Hyping AI Dangers」** Yann LeCun has accused Anthropic CEO Dario Amodei of overstating the dangers of open-weight AI models to push for regulations that would restrict their availability and preserve industry control. This criticism connects to Amodei&\#x27;s consistent position against open releases since his 2019 warnings about GPT-2, as seen in his roles at OpenAI and Anthropic.

**「Impact」** The debate could accelerate policies requiring hardware modifications like microcode updates to restrict LLM capabilities on GPUs from companies such as Nvidia and AMD, or mandating compute registration, thereby limiting open-source AI development and favoring closed models.

**「Community Discussion」** Hacker News users have compared Dario Amodei&\#x27;s approach to the Ottoman Empire banning the printing press for Arabic to maintain dogmatic control, arguing it restricts free access to diverse knowledge. Another commenter noted that open models are essential for defending against attacks from closed frontier models, suggesting some view the absence of open alternatives as a feature rather than a bug.

<details><summary>References</summary>
<ul>
<li><a href="https://www.indiatoday.in/technology/news/story/ai-godfather-says-dario-amodei-has-medieval-mindset-left-openai-when-things-went-out-of-control-3044733-2026-11-23">AI godfather says Dario Amodei has medieval mindset... - India Today</a></li>
<li><a href="https://www.explainx.ai/blog/dario-amodei-gpt2-openai-open-source-ai-controversy-2026">Dario Amodei Warned Against GPT-2 in 2019. Now He&#x27;s at | explainx. ai</a></li>

</ul>
</details>

**Tags**: `#AI regulation`, `#open-source AI`, `#Yann LeCun`, `#Anthropic`, `#AI safety`

---

<a id="item-tech-news-13"></a>
### [Microsoft Defaults to No 32-bit WoW64 in Windows Server 2028](https://www.windowslatest.com/2026/11/23/32-bit-apps-days-are-numbered-as-microsoft-strips-support-bit-by-bit-starting-with-windows-server-2028-but-windows-11-is-safe-for-now/) ⭐️ 6.0/10

Microsoft announced at Ignite 2026 that Windows Server 2028 will default-disable the WoW64 compatibility subsystem, so 32-bit applications cannot run out of the box. The change, part of reducing the attack surface to block 32-bit malware, allows reinstallation via optional FoD using PowerShell or DISM on Server Core. Windows 11 retains full WoW64 support with no deprecation timeline set.

telegram · zaihuapd · Nov 23, 03:03

**「WoW64 Deprecation in Windows Server 2028」** Windows 64-bit operating systems have supported 32-bit applications through the WoW64 subsystem, which enables the execution of 32-bit code on 64-bit processors. Microsoft plans to remove WoW64 from the default installation of Windows Server 2028, making 32-bit apps unavailable out of the box but restorable via optional features, to minimize the attack surface and reduce the risk of 32-bit malware. This deprecation does not impact Windows 11, which maintains full 32-bit compatibility.

**「Impact」** Organizations using Windows Server 2028 for legacy 32-bit software must manually install the WoW64 optional feature to restore compatibility, as it will be disabled by default.

<details><summary>References</summary>
<ul>
<li><a href="https://windowsreport.com/microsoft-is-dropping-32-bit-app-support-by-default-in-windows-server-2028/">Microsoft Is Dropping 32-Bit App Support by Default in ...</a></li>
<li><a href="https://www.neowin.net/news/windows-server-2028-dropping-support-for-32-bit-apps-wow64-will-be-available-as-fod/">Windows Server 2028 dropping support for 32-bit apps (WoW64 ...</a></li>
<li><a href="https://windowsforum.com/news/windows-server-2028-plans-to-make-wow64-optional-affecting-32-bit-apps.453724/">Windows Server 2028 Plans to Make WoW64 Optional, Affecting ...</a></li>

</ul>
</details>

**Tags**: `#Windows Server`, `#32-bit compatibility`, `#WoW64`, `#server security`, `#Microsoft announcements`

---

<a id="item-tech-news-14"></a>
### [Arm Requests jonpalmisc.com Shutdown on December 4, 2026](https://arm.jonpalmisc.com/) ⭐️ 5.0/10

Arm has requested that the jonpalmisc.com website, which hosts documentation on the Arm architecture including AArch64 references such as latest\_aarch64/absAnd, be discontinued on December 4, 2026. The request cites the site&\#x27;s use of Arm trademarks and intellectual property. This announced plan has sparked debate in the tech community on whether such hosting qualifies as fair use for hardware reverse engineering.

hackernews · tech234a · Nov 23, 19:17 · [Discussion](https://news.ycombinator.com/item?id=50617499)

**「Arm&\#x27;s Trademark and IP Policies」** Arm maintains trademark usage guidelines for its marks in websites and publications. The jonpalmisc.com site has hosted reference documentation for the AArch64 instruction set and system registers defined by the Armv8-A and Armv9-A architectures. Arm has requested the site&\#x27;s discontinuation on December 4, 2026, citing concerns over trademark and IP usage.

**「Impact」** After December 4, 2026, users and developers who have relied on the jonpalmisc.com site for Arm AArch64 documentation and reverse engineering resources will lose access, potentially requiring them to seek alternative sources or documentation.

**「Community Discussion」** Comments debate the legality of the request, questioning if hosting Arm documentation is fair use for reverse engineering while noting that the MRAS specifications appear licensed under BSD-style terms for open-source packages. One user mentioned offers of hosting mirrors or releasing non-IP source code to replicate the site.

<details><summary>References</summary>
<ul>
<li><a href="https://daily.dev/posts/per-arm-s-request-this-site-will-be-discontinued-on-4-december-2026--reuowbrg7">&quot;Per ARM&#x27;s Request, This Site Will Be Discontinued on 4 ...</a></li>
<li><a href="https://www.arm.com/company/policies/trademarks/guidelines-trademarks">Trademark use guidelines – Arm®</a></li>

</ul>
</details>

**Tags**: `#Arm Architecture`, `#Intellectual Property`, `#Fair Use`, `#Hardware Documentation`, `#Reverse Engineering`

---

<a id="item-tech-news-15"></a>
### [Apple Removes Open-Source App from EU App Store After 9 Years](https://github.com/glushchenko/fsnotes/discussions/2056) ⭐️ 5.0/10

Apple removed the open-source app fsnotes from the EU App Store after nine years because developer Oleksandr Hlushchenko did not verify as a DSA trader. The store message states that the developer has not identified as a merchant for the app. The app remains available in the US and UK app stores.

hackernews · fluder · Nov 23, 18:48 · [Discussion](https://news.ycombinator.com/item?id=50616933)

**「EU DSA Trader Status」** The European Union&\#x27;s Digital Services Act \(DSA\) requires app developers to identify as traders when distributing apps in the EU for regulatory compliance. Apple has integrated DSA trader status verification into App Store Connect, where developers must confirm their status for apps available in the European market. Without this verification, apps can be removed from the EU App Store, as mandated by the platform&\#x27;s compliance processes.

**「App Removals from EU App Stores for Non-Verified DSA Traders」** Apple began removing apps without verified trader status from the EU App Store across all 27 EU countries on February 17, 2025. Developers must declare and maintain verified trader status under the Digital Services Act to distribute apps in the EU, or risk having their apps removed.

**「Community Discussion」** Developers describe the removal as a known issue with EU DSA trader status verification, noting the app is still accessible in other regions. Open-source status is irrelevant, as compliance requires declaring trader status regardless of funding model.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.apple.com/help/app-store-connect/manage-compliance-information/manage-european-union-digital-services-act-trader-requirements/">Manage European Union Digital Services Act... - Apple Developer</a></li>
<li><a href="https://developer.apple.com/help/app-store-connect/manage-compliance-information/manage-european-union-digital-services-act-trader-requirements/">Manage European Union Digital Services Act trader requirements</a></li>
<li><a href="https://developer.apple.com/news/?id=x60uzbu9">Provide your trader status in App Store Connect</a></li>
<li><a href="https://appcompliance.io/blog/dsa-trader-status-app-stores/">DSA Trader Status: Why Apps Disappear from the EU App Store</a></li>
<li><a href="https://developer.apple.com/help/app-store-connect/manage-compliance-information/manage-european-union-digital-services-act-trader-requirements/">Manage European Union Digital Services Act trader ...</a></li>
<li><a href="https://developer.apple.com/forums/thread/826151">DSA Trader Verification &quot;In Review… | Apple Developer Forums</a></li>

</ul>
</details>

**Tags**: `#EU DSA`, `#App Store compliance`, `#Open source`, `#Regulatory impact`, `#Developer experience`

---

<a id="item-tech-news-16"></a>
### [Win4wine: Windows Shell as Linux Desktop via Wine](https://github.com/mikuta0407/win4wine) ⭐️ 5.0/10

Win4wine is a project that enables Linux users to run the Windows Shell \(explorer.exe from Windows XP or 7\) as their desktop environment by embedding it into the Linux desktop using Wine. This incremental open-source tool allows access to Windows applications from the Linux environment in a familiar Explorer interface. The capability is available on GitHub and targets users seeking a hybrid desktop setup without a full virtual machine.

hackernews · hard\_times · Nov 23, 12:28 · [Discussion](https://news.ycombinator.com/item?id=50610743)

**「Wine Compatibility Layer」** Wine is a compatibility layer that allows Windows applications to run on Linux by translating the Windows API to POSIX calls.

**「Community Discussion」** HN comments discuss the project&\#x27;s potential to run tools like AutoHotkey and note drawbacks including security vulnerabilities from using older Windows XP or 7 explorer.exe. Users suggest alternatives such as the XPTC theme for XFCE to achieve Windows XP looks and propose a reverse integration where Linux&\#x27;s composable command-line tools run on the Windows NT kernel.

**Tags**: `#wine`, `#linux-desktop`, `#windows-shell`, `#open-source`, `#compatibility`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Fed&\#x27;s John Williams: Higher rates likely over time to reach 2% inflation target](https://www.cnbc.com/2026/11/23/john-williams-fed-inflation-rate-hikes.html) ⭐️ 7.0/10

New York Fed President John Williams stated that inflation will reach the 2% target in 2027, signaling measured interest rate increases over time to address current pressures while the economy grows strongly ahead of the December FOMC meeting.

rss · CNBC Finance · Nov 23, 21:02

**「Inflation Target and Measurement」** The Federal Reserve targets a 2% inflation rate, measured by the Consumer Price Index \(CPI\) that tracks the price changes in a basket of goods and services commonly purchased by households, with the inflation rate calculated as \(current CPI minus previous CPI\) divided by previous CPI times 100.

<details><summary>References</summary>
<ul>
<li><a href="https://economy.inflaxia.com/">Economy Pulse | Inflation , CPI &amp; Economic Signals</a></li>
<li><a href="https://cpigauge.com/">CPI Guage | Live Consumer Price Index Monitoring &amp; Insights</a></li>
<li><a href="https://www.tradingview.com/markets/world-economy/">World Economy — Rankings and Forecasts — TradingView</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#Interest Rates`, `#Inflation`, `#Monetary Policy`, `#FOMC`

---

<a id="item-finance-news-2"></a>
### [Ant Group Leads $100 Million Investment in Simplexity Robotics at $1.6 Billion Valuation](https://www.bloomberg.com/news/articles/2026-11-22/ant-group-bets-on-simplexity-to-thrive-in-china-s-humanoid-race) ⭐️ 6.0/10

Ant Group led a $100 million pre-A round investment in Simplexity Robotics, a Chinese humanoid robotics company founded in 2025, at a $1.6 billion post-money valuation.

telegram · zaihuapd · Nov 23, 02:02

**「Simplexity Robotics prior funding and industry position」** Simplexity Robotics, a Chinese humanoid robotics company founded in July 2025 in Hangzhou with a core team from Li Auto, completed five funding rounds totaling 2 billion RMB by March 2026 at a post-money valuation exceeding 1 billion USD, as the Chinese humanoid robot industry holds about 97% of global shipments.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-11-22/ant-group-bets-on-simplexity-to-thrive-in-china-s-humanoid-race">Ant Group Bets on Simplexity in China’s Humanoid Race - Bloomberg</a></li>
<li><a href="https://aiweekly.co/alerts/ant-group-leads-100m-pre-a-for-simplexity-at-16b-valuation">Ant Group Leads $100M Pre-A for Simplexity at $1.6B Valuation</a></li>
<li><a href="https://www.japantimes.co.jp/business/2026/11/23/tech/ant-group-simplexity-china-humanoid/">Ant Group bets on Simplexity to thrive in China’s humanoid ...</a></li>

</ul>
</details>

**Tags**: `#Ant Group`, `#Simplexity Robotics`, `#humanoid robotics`, `#Chinese AI funding`, `#robotics market`

---

<a id="item-finance-news-3"></a>
### [Anthropic Limits IPO Underwriting Team to 4 Bankers, Bans Competitor Work](https://www.reuters.com/world/like-spacex-anthropic-ran-an-unusual-ipo-process-chafing-some-bankers-2026-11-22/) ⭐️ 6.0/10

Anthropic has required its IPO underwriting team to be limited to a maximum of 4 senior bankers and prohibited them from serving competitors such as OpenAI, Cursor, and DeepSeek for six months after the IPO, according to a Reuters report.

telegram · zaihuapd · Nov 23, 05:15

**「Anthropic IPO restrictions」** Anthropic capped deal teams at four senior bankers to prevent leaks despite bank workarounds and asked some bank officers to accept six-month restrictions on work with rivals such as OpenAI, Cursor and DeepSeek.

**「Impact on Investment Banks」** Investment banks weigh $500 million in underwriting fees against restrictions capping deal teams at four bankers and prohibiting work with rivals like OpenAI for six months, which may reduce their participation in the IPO and affect the AI industry&\#x27;s access to capital markets.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reuters.com/world/like-spacex-anthropic-ran-an-unusual-ipo-process-chafing-some-bankers-2026-11-22/">Like SpaceX, Anthropic ran an unusual IPO process, chafing ...</a></li>
<li><a href="https://www.unite.ai/anthropic-sought-limits-on-ipo-deal-teams-and-work-with-rivals/">Anthropic Sought Limits on IPO Deal Teams and Work with ...</a></li>
<li><a href="https://www.unite.ai/anthropic-sought-limits-on-ipo-deal-teams-and-work-with-rivals/">Anthropic Sought Limits on IPO Deal Teams and Work with Rivals</a></li>

</ul>
</details>

**Tags**: `#Anthropic`, `#IPO process`, `#AI industry`, `#Investment banking`, `#Tech competition`

---

<a id="item-finance-news-4"></a>
### [Anthropic IPO Triggers Sell-Off in Chinese Tech Stocks](https://www.bloomberg.com/news/articles/2026-11-23/china-s-next-ai-deals-clouded-by-selloff-after-anthropic-ipo) ⭐️ 6.0/10

Anthropic&\#x27;s record IPO has triggered a sell-off in Chinese tech stocks, clouding the listing plans of DeepSeek, Moon&\#x27;s Dark Side, and Step Star. Chinese tech stocks have evaporated $1.7 trillion since the end of June.

telegram · zaihuapd · Nov 23, 09:31

**「Background」** Anthropic&\#x27;s $119.5 billion IPO rose 17% on its first day and reached a market capitalization of $1.8 trillion before falling 8.5% the next day.

**Tags**: `#Anthropic IPO`, `#Chinese AI stocks sell-off`, `#DeepSeek listing`, `#AI market reaction`, `#tech sector impact`

---

<a id="item-finance-news-5"></a>
### [Nvidia Reinstatement of Jensen Huang as CEO Triggers Relief Rally](https://www.cnbc.com/2026/11/23/nvidia-jensen-huang-ceo-market-rally.html) ⭐️ 5.0/10

Nvidia reinstated Jensen Huang as CEO, triggering a relief rally in U.S. stocks on Monday after the S&amp;P 500 had tumbled more than 9% following his departure announcement on Nov. 12.

rss · CNBC Finance · Nov 23, 18:00

**「Background」** Nvidia CEO Jensen Huang was ousted on Nov. 12, triggering a sell-off in U.S. stocks, but his reinstatement on Monday sparked a relief rally.

**Tags**: `#Nvidia`, `#Jensen Huang`, `#AI trade`, `#market rally`, `#tech sector valuation`

---

<a id="item-finance-news-6"></a>
### [Foundation Future Industries Employees Lose Health Benefits](https://www.cnbc.com/2026/11/22/foundation-future-industries-health-benefits-payroll-base-group.html) ⭐️ 5.0/10

Employees at humanoid robot startup Foundation Future Industries, backed by Eric Trump, have had their health benefits terminated through Rippling retroactive to October after the last pay run on Oct. 15. The company is offering COBRA coverage to all employees for November and reimbursing premiums while seeking a bridge loan and potential $150 million investment from South Korean firm Base Group.

rss · CNBC Finance · Nov 23, 23:28

**「Cash crunch at Eric Trump-backed robot startup」** The humanoid robot startup Foundation Future Industries, advised and backed by Eric Trump, has been in cash crunch since August, with employees unpaid since October 15.

**「Impact」** Employees and their families face higher out-of-pocket costs for health coverage after benefits termination, with some already drawing down savings to cover living expenses.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/14/foundation-payroll-ceo-loan.html">Foundation robot startup runs out of cash after founder ...</a></li>
<li><a href="https://www.ibtimes.co.uk/eric-trump-robotics-startup-misses-payroll-pentagon-deal-1832474">Eric Trump-Backed Military Robot Startup Touted $24M Pentagon ...</a></li>
<li><a href="https://www.cnbc.com/2026/11/22/foundation-future-industries-health-benefits-payroll-base-group.html">Eric Trump -backed robot startup Foundation drops employee...</a></li>

</ul>
</details>

**Tags**: `#robotics startup`, `#financial distress`, `#employee benefits`, `#Eric Trump`, `#venture funding`

---

<a id="item-finance-news-7"></a>
### [JPMorgan and Hyundai Card Test AI Agents for Autonomous FX Transactions](https://www.cnbc.com/2026/11/18/jpmorgan-hyundai-card-ai-agents-payments.html) ⭐️ 5.0/10

JPMorgan Chase and Hyundai Card have completed an initial proof-of-concept testing AI agents autonomously handling foreign exchange transactions on a private blockchain for corporate treasury management. The companies are targeting advanced agent-to-agent negotiations in the first half of 2027.

rss · CNBC Finance · Nov 23, 06:06

**「Blockchain Collaboration Between JPMorgan and Hyundai Card」** Hyundai Card has previously completed blockchain-based cross-border payment proof-of-concepts, such as a $20,000 transfer using the USDT stablecoin between Hyundai Motor&\#x27;s U.S. and Mexican subsidiaries that took an average of seven minutes, while JPMorgan&\#x27;s Kinexys platform supports programmable payments and has processed more than $4 trillion in transactions.

<details><summary>References</summary>
<ul>
<li><a href="https://qz.com/jpmorgan-hyundai-card-ai-agents-payments-test-112326">JPMorgan and Hyundai Card test AI agents handling transactions</a></li>
<li><a href="https://www.cnbc.com/2026/11/18/jpmorgan-hyundai-card-ai-agents-payments.html">JPMorgan is working on AI agent transactions that don’t involve...</a></li>
<li><a href="https://www.jpmorgan.com/kinexys/index">Kinexys : Enterprise Bank-Led Blockchain Solutions</a></li>

</ul>
</details>

**Tags**: `#AI agents in finance`, `#JPMorgan Chase`, `#Hyundai Card`, `#blockchain payments`, `#autonomous transactions`

---

<a id="item-finance-news-8"></a>
### [Shanghai Metro Raises Fares After 21 Years](https://weibo.com/1699432410/5368461393397183) ⭐️ 5.0/10

Shanghai Metro has raised fares for the first time in 21 years, setting the starting price at 3 yuan for 0-4 km with incremental charges for additional distance. New 35-, 45-, 60-, and 90-ride tickets plus a monthly 9-fold discount will take effect on December 1.

telegram · zaihuapd · Nov 23, 10:45

**「Shanghai Metro Fare Adjustment」** Shanghai Metro has not adjusted fares for 21 years, and on November 23, 2026, the Shanghai Municipal Development and Reform Commission approved an optimization of the metro fare mechanism, effective December 1.

<details><summary>References</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20261123A0BINT00">上海地铁票价时隔21年调整，平均每人次提高0.9元，12月1日执行</a></li>
<li><a href="https://www.thepaper.cn/newsDetail_forward_34540094">时隔21年上海地铁票价调整：12月起实施，乘客支出怎么变？_浦江头条_...</a></li>
<li><a href="https://news.qq.com/rain/a/20261123A0CIXZ00">上海地铁票价时隔21年调整 平均每人次提高0.9元_腾讯新闻</a></li>

</ul>
</details>

**Tags**: `#Shanghai Metro fares`, `#transportation policy`, `#fare adjustment`, `#commuter concessions`, `#China urban transport`

---