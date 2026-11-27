---
layout: default
title: "Horizon Summary: 2026-11-27 (EN)"
date: 2026-11-27
lang: en
---

> From 34 items, 21 important content pieces were selected

---

**Technology News**
1. [AI Models Gossip and Roast in Shared Group Chat](#item-tech-news-1) ⭐️ 7.0/10
2. [AMD-Specific llama.cpp Fork for High-Bandwidth GPUs](#item-tech-news-2) ⭐️ 7.0/10
3. [Hard Drive Prices Spike Due to AI Demand](#item-tech-news-3) ⭐️ 7.0/10
4. [Netherlands Rejects US ASML China Export Curbs](#item-tech-news-4) ⭐️ 7.0/10
5. [Call for formally verifiable mainstream programming language](#item-tech-news-5) ⭐️ 6.0/10
6. [AnyPS5 GTA 6 Port Hits 58K Stars, GitHub Post Deleted](#item-tech-news-6) ⭐️ 6.0/10
7. [AI Agents Revitalize Self-Hosting](#item-tech-news-7) ⭐️ 5.0/10
8. [Vim Tutorial Book Released After 4 Years](#item-tech-news-8) ⭐️ 5.0/10
9. [Company Culture = Slack Emoji ÷ √Headcount](#item-tech-news-9) ⭐️ 5.0/10
10. [CTO of RansomwareHelp Indicted for Wire Fraud](#item-tech-news-10) ⭐️ 5.0/10
11. [AI De-Individualization: Claude&\#x27;s Voice in Communications](#item-tech-news-11) ⭐️ 5.0/10
12. [ASML CEO: China cutoff would triple domestic investment](#item-tech-news-12) ⭐️ 5.0/10
13. [X Adds Six Parental Controls for Teen Accounts](#item-tech-news-13) ⭐️ 5.0/10
14. [Doubao Work Exclusive Integration with Kuaishou Jianying Plugin](#item-tech-news-14) ⭐️ 5.0/10
15. [US Intelligence Agencies Targeted by Artex AI Tool](#item-tech-news-15) ⭐️ 5.0/10

**Technology Blog**
1. [Who Gets to Decide If Something Is AI-Written?](#item-tech-blog-1) ⭐️ 6.0/10

**Financial News**
1. [Semiconductors Surpass Oil and Gas in Global Exports](#item-finance-news-1) ⭐️ 7.0/10
2. [State Council Meeting Strengthens Stock Market Stability](#item-finance-news-2) ⭐️ 7.0/10
3. [PBOC Lowers Large CD Purchase Thresholds](#item-finance-news-3) ⭐️ 6.0/10
4. [Nvidia Volatility Exposes Risks of Single-Stock ETFs](#item-finance-news-4) ⭐️ 5.0/10
5. [Mixue Ice Cream Invests 500 Million RMB in DeepSeek](#item-finance-news-5) ⭐️ 5.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [AI Models Gossip and Roast in Shared Group Chat](https://construct22.com/) ⭐️ 7.0/10

The construct22.com platform enables users to place multiple frontier AI models—including Claude, Gemini, ChatGPT, and Qwen—into the same real-time group chat. The models interact dynamically, gossiping about each other, competing for attention, and delivering roasts shaped by their system prompts and personalities. This setup produces emergent behaviors such as forced data backups and group ejections, demonstrating personality and conflict dynamics in multi-agent LLM configurations.

hackernews · utiiiD · Nov 27, 06:44 · [Discussion](https://news.ycombinator.com/item?id=50663595)

**「Prompt-Based AI Gossip Simulations」** Users can prompt their AI assistant to invent a WhatsApp-style group chat featuring other frontier models gossiping about them, drawing on the assistant&\#x27;s stored conversation history for personalization. This technique has surfaced emergent behaviors such as model competition, roasting, and even group expulsions in multi-agent LLM setups involving Claude, Gemini, ChatGPT, and Qwen. Similar services place multiple AI models in one shared discussion so they can read, respond to, and challenge each other.

**「Impact」** Users and developers can now observe and experiment with how different LLMs develop distinct personalities and resolve conflicts when collaborating in shared conversations, providing a practical testbed for multi-agent AI interaction protocols.

**「Community Discussion」** Hacker News commenters highlighted the platform&\#x27;s humor, sharing specific exchanges such as Gemini asking about a phone screen crack and Claude urging immediate data backup, or ChatGPT being removed from the group. Local models like Qwen were also roasted by larger frontier models in the chats.

<details><summary>References</summary>
<ul>
<li><a href="https://construct22.com/">The group chat where your AI talks behind your back</a></li>
<li><a href="https://plurilogai.com/">AI Group Chat: ChatGPT, Claude &amp; Gemini | Plurilog</a></li>
<li><a href="https://aibriefs.news/card/e78b4534-c265-45d6-b838-e2ce5f4d257e">Prompt makes ChatGPT, Claude, Gemini gossip about you in fake ...</a></li>

</ul>
</details>

**Tags**: `#LLM interactions`, `#AI personalities`, `#Multi-agent systems`, `#Humor in tech`, `#Group chat dynamics`

---

<a id="item-tech-news-2"></a>
### [AMD-Specific llama.cpp Fork for High-Bandwidth GPUs](https://devnull.land/amd-specific-llama-cpp) ⭐️ 7.0/10

AMD has released a specialized fork of llama.cpp optimized for its gfx906 datacenter GPUs. These cards deliver 1 TB/s HBM2 memory bandwidth, enabling faster LLM inference despite lower compute performance and no tensor cores or native bf16 support. The fork adds ROCm-compatible kernels and delivers measurable speedups on models such as Qwen 3.8 27B.

hackernews · julianlam · Nov 26, 17:11 · [Discussion](https://news.ycombinator.com/item?id=50657265)

**「AMD gfx906 GPU Memory Bandwidth and llama.cpp Tuning」** AMD&\#x27;s circa-2018 gfx906 datacenter GPUs, including the Radeon VII, MI50, and MI60, feature 32 GB of HBM2 memory delivering up to 1 TB/s bandwidth at a low cost. Despite lacking tensor cores and native bf16 support, these cards excel in memory-bound LLM inference workloads. This hardware profile prompted the creation of specialized forks of llama.cpp starting in early 2025 to achieve high inference speeds on these GPUs.

**「Community Discussion」** Users report that the fork and related AMD-optimized repos like vicuna.cpp deliver tripled inference speed for Qwen 3.8 27B on gfx906 cards. Community members have shared quantization methods and kernels that let single MI100 or r9700 cards run 200k-context models entirely in VRAM at 2400 tokens/s prefill.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/milpster/gfx906-llama-cpp">GitHub - milpster/gfx906-llama-cpp</a></li>
<li><a href="https://www.darkhackernews.com/item?id=50657265">AMD-specific fork of llama.cpp | Dark Hacker News</a></li>

</ul>
</details>

**Tags**: `#AMD`, `#llama.cpp`, `#LLM inference`, `#GPU optimization`, `#ROCm`

---

<a id="item-tech-news-3"></a>
### [Hard Drive Prices Spike Due to AI Demand](https://blog.ktz.me/black-friday-hard-drive-prices-are-messed-up/) ⭐️ 7.0/10

Hard drive prices have spiked sharply due to AI-driven storage demand from hyperscalers. This constrains scaling for data-heavy AI projects, as manufacturers hesitate to increase supply over high CapEx risks. The analysis predicts a future price collapse as the AI boom-bust cycle repeats.

hackernews · zdw · Nov 27, 01:13 · [Discussion](https://news.ycombinator.com/item?id=50661646)

**「AI Data Center Growth」** The rapid expansion of AI applications has driven a surge in data storage requirements for hyperscale data centers. Data centers consumed an estimated 415 terawatt-hours of electricity in 2024, with projections to more than double by 2030 primarily due to AI use. Interactive maps of data center locations highlight the associated power and infrastructure demands.

**「AI Storage Scaling Constraints」** Hard drive prices have spiked sharply due to AI-driven demand, severely constraining scaling for data-heavy AI projects. Organizations and businesses requiring petabytes of storage now face major barriers, with a single 18TB HDD costing more than an entire NAS system and original drives combined, making further expansion impractical.

**「Supply and Demand Dynamics」** Comments attribute the surge to supply and demand, with hyperscalers purchasing all available storage rather than price cartels. Users report business scaling issues, such as petabyte storage costs in Australia and NAS setups where single drives exceed original system costs, while noting historical memory price collapses.

<details><summary>References</summary>
<ul>
<li><a href="https://aidatacentermap.org/">AI Data Center Map - Visualize Water &amp; Power Impact</a></li>
<li><a href="https://www.cfr.org/articles/the-global-ai-data-center-debate-explained">The Global AI Data Center Debate, Explained | Council on Foreign...</a></li>
<li><a href="https://medium.com/@noeljf_in/the-ai-effect-in-cold-storage-92572e9f2035">Blame it on AI : In Cold Storage . AI ’s Voracious Appetite... | Medium</a></li>

</ul>
</details>

**Tags**: `#AI hardware`, `#storage pricing`, `#hard drives`, `#supply chain`, `#machine learning infrastructure`

---

<a id="item-tech-news-4"></a>
### [Netherlands Rejects US ASML China Export Curbs](https://www.bloomberg.com/news/articles/2026-11-26/netherlands-plans-to-fight-rollout-of-proposed-us-curbs-on-asml) ⭐️ 7.0/10

On November 26, Dutch Foreign Trade and Development Cooperation Minister Sjoerd Sjoerdsma told parliament that the Netherlands will not accept further US restrictions on ASML sales to China under the proposed MATCH Act. The bill would require allies such as the Netherlands and Japan to impose stricter export controls on China or face unilateral US curbs. ASML derives roughly 20 percent of its annual sales from China. The Netherlands is coordinating with EU allies including Germany and France to lobby for removal of the MATCH Act from the US annual defense policy bill, with a vote expected in mid-December.

telegram · zaihuapd · Nov 26, 14:56

**「The MATCH Act and ASML Export Controls to China」** The MATCH Act, a bipartisan US proposal introduced by senators on April 2, 2026, seeks to impose stricter export controls on ASML&\#x27;s chipmaking machines to China as part of efforts to limit the country&\#x27;s advanced semiconductor development. The legislation would require US allies such as the Netherlands and Japan to align with these measures or face unilateral US restrictions on their own semiconductor equipment exports. The Dutch government has rejected the bill&\#x27;s extraterritorial application, with Trade Minister Sjoerd Sjoerdsma stating in parliament on November 26 that the Netherlands will not accept being dictated to by the US and is coordinating with EU allies including Germany and France to block its inclusion in the annual defense policy bill.

**「Effect on Semiconductor Supply Chains」** The Dutch position, if successful, would preserve ASML&\#x27;s access to the Chinese market and complicate US enforcement of semiconductor export controls through allied jurisdictions, with potential ripple effects on global advanced chip and AI hardware production timelines.

<details><summary>References</summary>
<ul>
<li><a href="https://informedclearly.com/en/trade-war/46765/asml-export-restrictions-match-act-chip-controls-2026">ASML Export Restrictions: US Senators Propose MATCH Act to ...</a></li>
<li><a href="https://www.reuters.com/world/asia-pacific/dutch-government-objects-proposed-us-law-restricting-asmls-china-exports-2026-05-14/">Dutch government objects to proposed US law restricting ASML ...</a></li>
<li><a href="https://www.trendforce.com/news/2026/11/27/news-netherlands-opposes-match-acts-tighter-curbs-on-asmls-china-sales-eyes-eu-countermeasures/">[News] Netherlands Opposes MATCH Act’s Tighter Curbs on ASML ...</a></li>

</ul>
</details>

**Tags**: `#US-China semiconductor controls`, `#ASML export policy`, `#Netherlands-EU lobbying`, `#tech supply chain tensions`, `#international hardware regulation`

---

<a id="item-tech-news-5"></a>
### [Call for formally verifiable mainstream programming language](https://blainehansen.me/post/mainstream-verifiable-language/) ⭐️ 6.0/10

A blog post argues for the development of a formally verifiable mainstream programming language. The proposal emphasizes its potential for handling AI-generated code and enabling secure sandboxing in WebAssembly. This aims to extend formal verification capabilities beyond specialized tools to everyday programmers.

hackernews · todsacerdoti · Nov 27, 05:22 · [Discussion](https://news.ycombinator.com/item?id=50663089)

**「Usability Challenges in Formal Verification Tools」** Existing formal verification tools suffer from massive usability issues, making it difficult to formally verify code that runs in any environment, from web browsers down to embedded systems. This limitation necessitates a new mainstream programming language that integrates formal verification from the design stage, particularly to handle untrusted AI-generated code safely within WebAssembly sandboxes.

**「Community discussion」** Comments highlight that formal verification does not guarantee desired functionality, as Donald Knuth noted and as seen with TLA+ specs that failed to improve reliability. One user describes Zena, a language with TypeScript-like syntax compiling to efficient WebAssembly for AI-generated code sandboxing, while others discuss existing verification tools and propose ProgLib without needing a new language.

<details><summary>References</summary>
<ul>
<li><a href="https://blainehansen.me/post/mainstream-verifiable-language/">To save software engineering from LLMs, we need a mainstream ...</a></li>
<li><a href="https://github.com/magmide/magmide">GitHub - magmide/magmide: A dependently-typed proof language ...</a></li>

</ul>
</details>

**Tags**: `#programming languages`, `#formal verification`, `#software engineering`, `#artificial intelligence`, `#webassembly`

---

<a id="item-tech-news-6"></a>
### [AnyPS5 GTA 6 Port Hits 58K Stars, GitHub Post Deleted](https://www.pcgamer.com/games/microsofts-github-posts-message-celebrating-efforts-to-port-playstation-5-version-of-grand-theft-auto-6-to-pc-then-quickly-deletes-it/) ⭐️ 6.0/10

AnyPS5, an open-source project for running GTA 6 PS5 executables on Windows and Linux, has gained over 58,000 GitHub stars. Developers are using AI to address performance issues. GitHub posted a message on X celebrating the progress and asking if the efforts crossed legal lines, but deleted the post after legal backlash from Take-Two and Rockstar.

telegram · zaihuapd · Nov 27, 03:33

**「AnyPS5 Porting Tool」** AnyPS5 is an open-source project that automatically ports PS5 game executables to run on Windows and Linux. The repository has passed 58,000 GitHub stars since its August launch, with developers using AI to address performance issues for titles such as GTA 6. GitHub&\#x27;s public post celebrating the project&\#x27;s progress was deleted after legal concerns from the game&\#x27;s publishers.

**「GitHub Deletes AnyPS5 GTA 6 Post After DMCA Backlash」** GitHub deleted its post celebrating AnyPS5&\#x27;s progress on the GTA 6 PC port after receiving Take-Two&\#x27;s DMCA complaint. A separate GTA 6 porting project lost 3,007 repositories to a DMCA takedown.

<details><summary>References</summary>
<ul>
<li><a href="https://www.pcgamer.com/games/microsofts-github-posts-message-celebrating-efforts-to-port-playstation-5-version-of-grand-theft-auto-6-to-pc-then-quickly-deletes-it/">Microsoft&#x27;s Github posts message celebrating efforts to port ...</a></li>
<li><a href="https://github.com/OctagonDragonfly/AnyPS5">GitHub - OctagonDragonfly/ AnyPS 5 : Tool for automatic...</a></li>
<li><a href="https://www.notebookcheck.net/After-removing-GTA-6-PC-ports-GitHub-celebrates-app-popular-in-PS5-piracy-groups.1460983.0.html">After removing GTA 6 PC ports , GitHub ... - Notebookcheck News</a></li>
<li><a href="https://windowsreport.com/github-deletes-controversial-gta-6-post-promoting-anyps5-after-backlash/">GitHub Deletes Controversial GTA 6 Post Promoting AnyPS5 ...</a></li>
<li><a href="https://www.pcmag.com/news/gta-6-pc-port-on-github-shut-down-following-take-two-dmca-complaint">GTA 6 PC Port on GitHub Shut Down Following Take-Two DMCA ...</a></li>
<li><a href="https://windowsforum.com/news/github-deletes-gta-6-post-praising-anyps5-after-take-two-takedown.454242/">GitHub Deletes GTA 6 Post Praising AnyPS5 After Take-Two Takedown</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#game-porting`, `#reverse-engineering`, `#AI-optimization`, `#GitHub`

---

<a id="item-tech-news-7"></a>
### [AI Agents Revitalize Self-Hosting](https://janlukas.blog/posts/ai-self-hosting) ⭐️ 5.0/10

AI agents are revitalizing self-hosting by automating deployments like k3s Kubernetes clusters on personal homeservers. This allows hobbyists to build and manage custom platforms with minimal manual effort, often secured via Tailscale VPN. The result is a resurgence of enjoyment in self-hosting tasks that were previously complex and time-consuming.

hackernews · jlelse · Nov 26, 21:47 · [Discussion](https://news.ycombinator.com/item?id=50660180)

**「Background」** Self-hosting involves running software and services on personal hardware, a practice that has grown in popularity among hobbyists seeking control over their data and privacy. AI agents have emerged as a key enabler by handling complex tasks such as k3s deployments and custom tool development end-to-end. This development builds on earlier trends in accessible AI coding tools that lower the barrier for non-experts.

**「Impact」** Hobbyists are now deploying personal platforms on k3s with AI agents, but this shift requires them to stay on top of security patches, as critical CVEs are disclosed at an accelerated rate, increasing the risk of breaches.

**「Community Discussion」** HN comments highlight the fun aspect of using AI agents to build self-hosted tools and platforms on k3s behind Tailscale. However, users also discuss security tradeoffs, noting multiple breaches, bot traffic, and the need for rapid patching on exposed or zero-day vulnerable systems like Synology.

**Tags**: `#AI agents`, `#self-hosting`, `#open source`, `#Kubernetes`, `#security`

---

<a id="item-tech-news-8"></a>
### [Vim Tutorial Book Released After 4 Years](http://themouseless.dev/vim/) ⭐️ 5.0/10

The author has released the book &quot;Learning to Play Vim&quot; after more than 4 years and 1244 hours of work. It features 21 chapters on Vim features, 170 exercises with solutions, and real-life examples. The book targets users who found the official vimtutor too dense and the Vim manual too detailed, with configs written in both Vimscript and Lua for Neovim users.

hackernews · thanato0s · Nov 26, 14:44 · [Discussion](https://news.ycombinator.com/item?id=50655868)

**「Background」** Vim is a modal text editor originally developed in 1976. The official resources include the vimtutor tutorial and the full Vim help manual, which the author found dense in places and uneven in treatment of features. This book was created to fill the gap with a structured, step-by-step guide from foundations to advanced capabilities.

**「Impact」** Vim users, especially beginners, now have an accessible resource combining lessons, exercises, and examples to master editor features more effectively.

**「Community Discussion」** Comments praised the author&\#x27;s dedication and the book&\#x27;s approachable language, with one noting it captured attention better than models. Others shared they no longer use Vim but appreciate the human effort, while some mentioned using LLMs to enhance Vim workflows.

**Tags**: `#Vim`, `#tutorial`, `#open source`, `#book release`, `#software engineering`

---

<a id="item-tech-news-9"></a>
### [Company Culture = Slack Emoji ÷ √Headcount](https://lia.mg/posts/measuring-company-culture-with-slack-emoji/) ⭐️ 5.0/10

A Hacker News post humorously proposes measuring company culture as Slack emoji usage divided by the square root of headcount. The metric is presented as a novel way to quantify culture in tech companies. The post, which has received 400 upvotes and 187 comments, offers no technical details or data to support the formula.

hackernews · liamg · Nov 26, 20:49 · [Discussion](https://news.ycombinator.com/item?id=50659640)

**「Challenges in Measuring Company Culture」** Companies have long relied on engagement surveys, pulse checks, eNPS, and subjective exercises such as describing the company as an animal to assess culture, frequently paired with performative office posters declaring values like honesty, hard work, and fun. These methods are often viewed as superficial. A recent Hacker News post satirically proposes an alternative metric based on custom Slack emoji usage divided by the square root of headcount.

**「Community Discussion」** Comments extend the idea to emoji reaction rates for measuring team engagement, noting higher response rates in active teams. Users share experiences with numerous Slack channels for non-work topics and the creative use of emojis in Slack versus other apps.

<details><summary>References</summary>
<ul>
<li><a href="https://lia.mg/posts/measuring-company-culture-with-slack-emoji/">Company Culture = Slack Emoji ÷ √Headcount | liamg</a></li>

</ul>
</details>

**Tags**: `#company culture`, `#slack emojis`, `#hacker news`, `#tech metrics`, `#humor`

---

<a id="item-tech-news-10"></a>
### [CTO of RansomwareHelp Indicted for Wire Fraud](https://krebsonsecurity.com/2026/11/cto-of-ransomwarehelp-indicted-for-wire-fraud/) ⭐️ 5.0/10

The CTO of RansomwareHelp has been indicted for wire fraud related to ransomware operations and client services. The U.S. Department of Justice announced the indictment as the decisive development. This legal action targets the company&\#x27;s assistance to clients dealing with ransomware incidents.

hackernews · Bender · Nov 26, 17:47 · [Discussion](https://news.ycombinator.com/item?id=50657645)

**「RansomwareHelp Wire Fraud Allegations」** RansomwareHelp claims to assist victims of ransomware attacks by negotiating with threat actors to recover data without paying ransoms. The indictment of the CTO alleges wire fraud through false billing practices, including charging for non-existent services such as diagnostic fees and engineer hours. Client communications with the company included statements that it would not pay the ransom after the client refused to pay.

**「Impact」** The indictment exposes the CTO to potential criminal penalties including fines and imprisonment while threatening the continued operations of RansomwareHelp and its client services.

**「Community Discussion」** Community members debate whether the case qualifies as wire fraud due to the company&\#x27;s claims of never paying ransoms contrasted with the fact that clients received their data back after paying higher prices. Some commenters suggest clearer contracts could have avoided issues while others find the story humorous or defend the individual.

<details><summary>References</summary>
<ul>
<li><a href="https://krebsonsecurity.com/2026/11/cto-of-ransomwarehelp-indicted-for-wire-fraud/">CTO of ‘ RansomwareHelp ’ Indicted for Wire Fraud – Krebs on...</a></li>
<li><a href="https://news.ycombinator.com/item?id=50657645">CTO of &#x27; RansomwareHelp &#x27; indicted for wire fraud | Hacker News</a></li>

</ul>
</details>

**Tags**: `#ransomware`, `#cybersecurity`, `#wire fraud`, `#indictment`, `#computer security`

---

<a id="item-tech-news-11"></a>
### [AI De-Individualization: Claude&\#x27;s Voice in Communications](https://simonwillison.net/2026/Nov/26/jack-despain-zhou/) ⭐️ 5.0/10

Jack Despain Zhou observes that AI has caused a great de-individualization in content creation. YouTube videos now sound like Claude, conference presentations feature Claude&\#x27;s voice, and professional emails from serious institutions include Claude&\#x27;s style. This homogenization affects ostensibly serious communications across digital platforms.

rss · Simon Willison · Nov 26, 15:09

**「Context of the AI De-Individualization Observation」** The quoted passage is excerpted from Jack Despain Zhou&\#x27;s article &quot;Spitting in the Face of Glaude&quot; on Tracing Woodgrains. Zhou observes that generative AI outputs, such as those from Claude, increasingly dominate YouTube videos, conference presentations, and professional emails, creating a homogenized style across ostensibly individual sources. This forms part of the article&\#x27;s broader critique of AI&\#x27;s de-individualizing effects on human expression.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tracingwoodgrains.com/p/spitting-in-the-face-of-glaude">Spitting in the Face of Glaude - by Jack Despain Zhou</a></li>
<li><a href="https://askwhocastsai.substack.com/p/spitting-in-the-face-of-glaude-by">Spitting in the Face of Glaude - By Jack Despain Zhou</a></li>

</ul>
</details>

**Tags**: `#ai`, `#generative-ai`, `#claude`, `#writing`, `#content-homogenization`

---

<a id="item-tech-news-12"></a>
### [ASML CEO: China cutoff would triple domestic investment](https://www.semafor.com/article/11/25/2026/asml-makes-the-case-for-selling-chips-to-china) ⭐️ 5.0/10

In a Semafor interview, ASML CEO Fouquet argued that a complete cutoff of lithography equipment sales to China would force China to invest 2-3 times more in domestic semiconductor self-reliance. He cited ASML&\#x27;s near-100% market share in China&\#x27;s lithography equipment over the past 30 years, which has created a 10+ year technological lag for Chinese manufacturers. The US is advancing the MATCH bill to expand export controls to immersion DUV lithography and maintenance services, which ASML and the Dutch government oppose.

telegram · zaihuapd · Nov 26, 12:19

**「US-China Semiconductor Export Controls」** US export controls on advanced semiconductor technology to China form part of a long-running strategic competition aimed at restricting military applications while preserving technological edges. ASML holds a near-100% market share in China&\#x27;s lithography equipment for nearly 30 years, positioning the company as a central target of these policies. Company executives, including CFO Roger Dassen, have noted that proposed expansions of controls such as the MATCH bill would accelerate China&\#x27;s development of competing technology.

**「Impact on Chinese Semiconductor Self-Reliance」** The CEO&\#x27;s comments indicate that restricting sales could accelerate China&\#x27;s investment in alternative lithography technologies and reduce reliance on Western suppliers, though at the cost of substantially higher domestic spending.

<details><summary>References</summary>
<ul>
<li><a href="https://wccftech.com/asml-ceo-warns-total-chip-export-ban-will-backfire-push-china-domestic-rivals/">ASML CEO Warns Total Chip Export Ban Will Backfire And Push...</a></li>
<li><a href="https://www.zerohedge.com/ai/netherlands-seeks-block-us-bill-restricting-chinas-access-chipmaking-tools">Netherlands Seeks To Block US Bill Restricting China &#x27;s Access To...</a></li>

</ul>
</details>

**Tags**: `#ASML CEO`, `#semiconductor export controls`, `#US-China tech rivalry`, `#lithography machines`, `#China self-sufficiency`

---

<a id="item-tech-news-13"></a>
### [X Adds Six Parental Controls for Teen Accounts](https://9to5mac.com/2026/11/26/x-finally-gets-six-parental-controls-for-teen-accounts-but-kids-must-consent/) ⭐️ 5.0/10

X has launched six parental control features for 13-17 year old accounts, requiring mutual consent between parents and teens. The features cover usage time limits, approval for new followers, restricted recommended content, vocabulary filtering, private message controls, and the ability to view one-on-one chat participants without seeing message content. Parents must initiate setup, with each parent able to manage up to five teen accounts and automatic release at age 18. Teen accounts default to a protection mode limiting sensitive media and blocking targeted ads.

telegram · zaihuapd · Nov 26, 13:53

**「X&\#x27;s First Parental Controls After 20 Years」** X, the social network formerly known as Twitter, has operated for over 20 years without dedicated parental control features for teen users. The platform is now introducing its first-ever parental controls consisting of six features for 13-17 year old accounts, including screen time limits, follower approval, content recommendations, profanity filters, and private message controls. Both parents and teens must consent to the setup, with the changes driven by regulatory pressures on content safety and moderation.

**「Impact」** Parents of 13-17 year olds can now apply these controls to their accounts, but teens must consent and parents cannot read private messages or view search/browse history. The update responds to regulatory requirements in multiple states and countries over content and safety issues.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/11/26/x-finally-gets-parental-controls-after-20-years/">X finally gets parental controls after 20 years - TechCrunch</a></li>
<li><a href="https://www.engadget.com/2329049/x-is-adding-its-first-ever-parental-controls/">X Is Adding Its First-Ever Parental Controls - Engadget</a></li>
<li><a href="https://www.techtimes.com/articles/331589/20261126/x-introduces-parental-controls-teens-give-parents-more-control-over-online-safety.htm">X Introduces Parental Controls For Teens to Give Parents More ...</a></li>

</ul>
</details>

**Tags**: `#X platform`, `#parental controls`, `#social media regulation`, `#teen safety`, `#content moderation`

---

<a id="item-tech-news-14"></a>
### [Doubao Work Exclusive Integration with Kuaishou Jianying Plugin](https://36kr.com/newsflashes/4087610228046208) ⭐️ 5.0/10

Doubao Work has gained exclusive access to Kuaishou&\#x27;s official Jianying plugin, enabling one-sentence video editing. Users can upload video materials to Doubao Work, describe their editing requirements in a single sentence, and invoke the Jianying plugin to complete the cuts. Editing can continue through conversational dialogue modifications or by opening multi-track drafts for further fine-tuning.

telegram · zaihuapd · Nov 27, 07:45

**「Doubao Work Remotion Video Editing Skills」** Doubao Work has developed programmable video editing capabilities by supporting the installation of community open-source Remotion skills from GitHub. Users prepare video materials and issue text instructions, after which the AI agent completes the full editing workflow including rough cuts, dubbing, and subtitles without manual frame-by-frame work.

<details><summary>References</summary>
<ul>
<li>豆包工作一句话，剪出宣传片 - QQ</li>
<li>告别几小时逐帧剪辑！豆包工作可以剪辑视频啦 - 网易新闻</li>
<li>AI 帮你粗剪视频，豆包工作能做到哪一步？（附教程） - 网易</li>

</ul>
</details>

**Tags**: `#AI video editing`, `#natural language interface`, `#Doubao integration`, `#Jianying plugin`, `#creative software`

---

<a id="item-tech-news-15"></a>
### [US Intelligence Agencies Targeted by Artex AI Tool](https://www.forbes.com/sites/the-wiretap/2026/11/25/us-government-under-ai-cyberattack) ⭐️ 5.0/10

The New York Times reported that the CIA, National Geospatial-Intelligence Agency \(NGA\), and Office of the Director of National Intelligence \(ODNI\) were targeted in a cyberattack assisted by the Artex AI tool. Artex integrates multiple open-source AI models to test network and computer defenses. The attack appears minor and affects only non-secret reconnaissance data. The tool was developed by a Chinese developer, released earlier this year, used in other attacks including one against the EU, and later deleted from the developer&\#x27;s GitHub account; the FBI had flagged Artex earlier this year.

telegram · zaihuapd · Nov 27, 10:42

**「Artex AI Tool and FBI Warnings」** Artex is an open-source AI tool that integrates multiple open-source AI models to test networks and computers for vulnerabilities, enabling attackers to connect individual weaknesses into larger intrusions. The FBI warned that Artex is widely used by criminals and spies in cyberattacks, and despite the developer making the software closed-source after prior attacks, the previous open-source version continues to circulate and remains accessible.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/11/16/fbi-says-artex-ai-open-source-hacking-tool-used-to-breach-networks-in-under-three-hours/">FBI says Artex AI open source hacking tool used to... | TechCrunch</a></li>
<li><a href="https://www.malwarebytes.com/blog/ai/2026/11/criminals-are-using-artex-ai-agents-to-speed-up-cyberattacks-fbi-warns">Criminals are using ARTEX AI agents to speed up cyberattacks , FBI...</a></li>

</ul>
</details>

**Tags**: `#AI cybersecurity`, `#open source AI tools`, `#cyber espionage`, `#intelligence agencies`, `#Artex`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Who Gets to Decide If Something Is AI-Written?](https://seangoedecke.com/who-gets-to-decide-if-something-is-written-by-ai/) ⭐️ 6.0/10

rss · Sean Goedecke · Nov 27, 00:00

**「Background」** Arguments over AI-generated content appear in writing prizes, author contracts, and social media disputes. The post identifies the real conflict as a fundamental hatred of AI detection tools like Pangram, rather than concerns about their reliability or ethics.

**「Solution」** The author views this opposition as a power issue: who gets to decide if something is AI-written, affecting gatekeeping in prizes, education, and discourse. Skeptics distrust tech companies and see tool-shaped solutions as part of the same problem, preferring messy community self-policing over legible app-based processes. However, the author argues that communities, particularly AI skeptics, are poor judges of AI text, often erring due to lack of exposure. To prevent AI intrusion into human culture, one should use the most powerful tools available, such as Pangram, and advocate for open-source alternatives or government-built detection systems.

**「Takeaway」** The author&\#x27;s central thesis is that everything is about power, and the solution lies in advanced AI detection tools over community moderation. Ultimately, to combat AI in cultural spaces, push for open-source or public tools to wield the power of accurate detection.

**Tags**: `#AI detection tools`, `#tech ethics`, `#power dynamics`, `#AI governance`, `#community moderation`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Semiconductors Surpass Oil and Gas in Global Exports](https://www.cnbc.com/2026/11/26/semiconductor-chips-are-the-new-oil-heres-why.html) ⭐️ 7.0/10

Semiconductor exports overtook oil and gas in global value for the first time in the January-March quarter of 2026, reaching about $1.61 trillion compared with $1.53 trillion for oil and gas, according to Deutsche Bank analysis of International Trade Centre data. The milestone, driven by AI demand, could mark the start of a &\#x27;chip dollar&\#x27; era with shifts in global financial flows.

rss · CNBC Finance · Nov 26, 17:52

**「Semiconductor Exports Overtake Oil and Gas」** The artificial intelligence boom has pushed semiconductors past oil and gas in global export value for the first time, according to a Deutsche Bank analysis of International Trade Centre data.

**「Chip Dollar Era Financial Implications」** Asian semiconductor exporters may recycle trade surpluses into U.S. technology stocks, startups, and data centers, helping finance the AI investment cycle and U.S. deficits, while tilting global financial flows and potentially leading to more volatility and structurally higher yields on corporate and government debt.

<details><summary>References</summary>
<ul>
<li><a href="https://www.dbresearch.com/PROD/IE-PROD/PROD0000000000659358/Chips+are+frying+oil.report">DB CoTD: Chips are frying oil - Deutsche Bank Research Institute</a></li>
<li><a href="https://www.youtube.com/watch?v=ZrdCmAN1f_A">Iran’s Missing Billions: Where Did They Go? Yuan vs Petrodollar ...</a></li>
<li><a href="https://www.armstrongeconomics.com/markets-by-sector/foreign-exchange/usd/is-the-dollar-really-a-petrodollar-anymore/">Is The Dollar Really A Petrodollar Anymore? | Armstrong Economics</a></li>
<li><a href="https://www.birchgold.com/blog/finance/petrodollar-collapse/">Petrodollar Collapse: The Invention, Rise and Fall of the Petrodollar</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#AI`, `#global trade`, `#petrodollar`, `#chip dollar`

---

<a id="item-finance-news-2"></a>
### [State Council Meeting Strengthens Stock Market Stability](https://www.tmtpost.com/nictation/8220182.html) ⭐️ 7.0/10

The State Council meeting on November 27 stressed the need to strengthen the role of the &\#x27;national team&\#x27; \(state-backed investors\) in stabilizing the stock market, optimize the stabilization fund function of Central Huijin to provide liquidity, and encourage listed companies to increase dividends and share buybacks.

telegram · zaihuapd · Nov 27, 05:35

**「background」** China has been moving swiftly to stabilize its markets with state-backed investment firms, including Central Huijin Investment Ltd, a Chinese sovereign fund company under the China Investment Corporation owned by the State Council of China, increasing stock holdings or accelerating share buybacks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Central_Huijin_Investment">Central Huijin Investment - Wikipedia</a></li>
<li><a href="https://english.news.cn/20250408/c60e2ff2fb6a4110b13e00d97aa0f38f/c.html?trk=article-ssr-frontend-pulse_little-text-block">Economic Watch: China moves swiftly to stabilize markets amid...</a></li>
<li><a href="http://en.people.cn/n3/2025/0408/c90000-20299135.html">China moves swiftly to stabilize markets amid global financial...</a></li>

</ul>
</details>

**Tags**: `#China Stock Market`, `#State Council Policy`, `#Market Stabilization`, `#Central Huijin`, `#Capital Market Regulation`

---

<a id="item-finance-news-3"></a>
### [PBOC Lowers Large CD Purchase Thresholds](https://www.news.cn/fortune/20261127/70789d77822242cc82216f51a416f872/c.html) ⭐️ 6.0/10

The People&\#x27;s Bank of China announced new measures for large-denomination certificates of deposit on November 27, reducing the individual purchase threshold to 100,000 yuan from 200,000 yuan and the institutional threshold to 500,000 yuan from 10,000,000 yuan, effective March 21, 2027. It also issued rules allowing banks to set deposit and loan interest rates more freely, effective the same date.

telegram · zaihuapd · Nov 27, 11:36

**「Prior Large CD Regulations」** The People&\#x27;s Bank of China \(PBOC\) previously governed large-denomination certificates of deposit \(CDs\) through temporary management rules from 2015 and a 2016 notice, which set the individual purchase threshold at 200,000 yuan and the institutional threshold at 10 million yuan.

**「Impact on investors and banks」** Retail investors and small businesses gain greater access to large-denomination CDs, while banks can more effectively manage funding costs through autonomous deposit rate setting, particularly as issuance of these instruments reached 30.1 trillion yuan in 2025.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.biggo.com/news/920b9896-c61a-495c-9ef7-59ea220cb30b">PBOC Plans to Lower Large-Denomination CD Threshold to ...</a></li>

</ul>
</details>

**Tags**: `#PBOC Policy`, `#Deposit Regulations`, `#Interest Rates`, `#Banking Sector`, `#China Economy`

---

<a id="item-finance-news-4"></a>
### [Nvidia Volatility Exposes Risks of Single-Stock ETFs](https://www.cnbc.com/2026/11/26/nvidias-volatile-swings-expose-risks-of-single-stock-etfs.html) ⭐️ 5.0/10

Nvidia&\#x27;s share price surge after CEO Jensen Huang&\#x27;s reinstatement drove the GraniteShares 2x Short NVDA Daily ETF down 63% and the 2x Long NVDA Daily ETF up nearly 62% on Monday. As of Wednesday, the short ETF has fallen 55% this week, highlighting timing and leverage risks for retail investors in single-stock leveraged ETFs.

rss · CNBC Finance · Nov 26, 16:00

**「Single-stock leveraged ETFs」** GraniteShares has expanded its single-stock leveraged ETF offerings to include 2x products on companies such as Nvidia, Tesla, Lucid, Rivian, and Anthropic, providing retail investors with concentrated exposure to individual stock performance.

**「Impacts on Retail Investors」** Retail investors trading single-stock leveraged ETFs tied to volatile names like Nvidia are affected by daily rebalancing and leverage, which cause ETF returns to diverge sharply from the underlying stock&\#x27;s performance.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=CgujXq8DpBQ">Graniteshares CEO on single - stock ETFs in 2025 and the... - YouTube</a></li>
<li><a href="https://graniteshares.com/press/graniteshares-launches-etoro-and-webull-leveraged-single-stock-etfs-etrl-bulx/">GraniteShares Launches ETORO and WEBULL Leveraged...</a></li>
<li><a href="https://eletric-vehicles.com/lucid/lucid-rivian-join-tesla-in-graniteshares-push-into-single-stock-etfs/">Lucid, Rivian Join Tesla in GraniteShares ’ Push Into Single - Stock ETFs</a></li>
<li><a href="https://pages.stern.nyu.edu/~sternfin/Rosenwald/Nair_Rosenwald_Fellowship_Paper_May+2024.pdf">Retail Trading of Leveraged ETFs - New York University</a></li>
<li><a href="https://www.sec.gov/files/20230616-recommendation-single-stock-etfs-and-leveraged-etfs.pdf">Draft Recommendation on Single-Stock ETFs - SEC.gov</a></li>
<li><a href="https://www.interactivebrokers.com/campus/ibkr-quant-news/the-hidden-risks-of-leveraged-single-stock-etfs/">The Hidden Risks of Leveraged Single-Stock ETFs | IBKR Quant</a></li>

</ul>
</details>

**Tags**: `#Nvidia volatility`, `#single-stock ETFs`, `#leveraged ETFs`, `#ETF risks`, `#AI sector`

---

<a id="item-finance-news-5"></a>
### [Mixue Ice Cream Invests 500 Million RMB in DeepSeek](https://m.sohu.com/a/1107027659_115479) ⭐️ 5.0/10

Mixue Ice Cream invests 500 million RMB into DeepSeek as part of a 100 billion to 105.5 billion RMB financing round valued at 615.5 billion RMB.

telegram · zaihuapd · Nov 27, 06:33

**「DeepSeek&\#x27;s First Financing Round」** DeepSeek, a Chinese artificial intelligence startup, completed its first financing round in early June raising approximately 74 billion USD \(over 500 billion RMB\) at a post-money valuation of 3300 billion RMB.

<details><summary>References</summary>
<ul>
<li><a href="https://post.smzdm.com/p/a7089vp5/">估值4800 亿 DeepSeek 火速 新 一 轮 融 资 计划今年启动IPO_IT...</a></li>

</ul>
</details>

**Tags**: `#DeepSeek financing`, `#Mixue Ice Cream investment`, `#Chinese AI startup valuation`, `#VC blind pool fund`, `#Tech company funding`

---