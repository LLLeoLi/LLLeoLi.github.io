---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

I am a second-year master student at the School of AI, Beihang University (BUAA), supervised by Prof. [Lei Sha](https://shalei120.github.io/.). I was honored to be advised  by [Jing Shao](https://amandajshao.github.io/), JG Yao, and [Junxian He](https://jxhe.github.io/).

My previous research focused on the safety alignment of AI and long-horizon reasoning, and I am now seeking a PhD position for 2027 Fall.


# 🔥 News
- *2026.08*: &nbsp;🎉🎉 SafeSteer is accepted by EMNLP 2026. 
- *2026.04*: &nbsp;🎉🎉 SSP is accepted by ACL 2026 Findings. 
- *2026.02*: &nbsp;🎉🎉 ReVeL is accepted by CVPR 2026. 
- *2025.08*: &nbsp;🎉🎉 Two papers (LARF and DIffusionAttacker) are accepted by EMNLP 2025 and DIffusionAttacker is selected as Oral Presentation. 
- *2025.03*: &nbsp;🎉🎉 Two papers (ActorBreaker and VLSBench) are accepted by ACL 2025 and ActorBreaker is selected as Outstanding Paper.
- *2024.09*: &nbsp;🎉🎉 ASETF is accepted by EMNLP 2024 and selected as Oral Presentation.

# 📝 Publications 

<div class='paper-box'>
  <div class='paper-box-text' markdown="1">

  <div class="badge">EMNLP 2026</div>

  [SafeSteer: Localized On-Policy Distillation for Efficient Safety Alignment](https://arxiv.org/abs/2606.02530)

  **Hao Li**\*, Jingkun An\*, Zijun Song\*, Pengyu Zhu, Rui Li, Hao Wang, Wendi Feng, Yesheng Liu, Lijun Li, Jin-Ge Yao, Lei Sha

  <span class="paper-tldr">**TL;DR:** Restricting the reverse KL penalty to algorithmically identified safety tokens, distilled from an activation-steering safety instructor, aligns LLMs with only 100 harmful samples and no general-purpose data — cutting the alignment tax on general capabilities.</span>

  <!-- [**Code**](#) <strong><span class='show_paper_citations' data='fan-etal-2025-metaflowllm'></span></strong>   -->
  </div>
</div>

<div class='paper-box'>
  <div class='paper-box-text' markdown="1">

  <div class="badge">ACL 2026 Findings</div>

  [Be Your Own Red Teamer: Safety Alignment via Self-Play and Reflective Experience Replay](https://arxiv.org/abs/2601.10589)
  
  Hao Wang, Yanting Wang, **Hao Li**, Rui Li, Lei Sha

  <span class="paper-tldr">**TL;DR:** Safety Self-Play (SSP) lets one model be both attacker and defender in a single RL loop, with UCB-sampled reflective experience replay over low-reward failures, so defenses keep evolving instead of overfitting static adversarial datasets.</span>

  <!-- [**Code**](#) <strong><span class='show_paper_citations' data='fan-etal-2025-metaflowllm'></span></strong>   -->
  </div>
</div>


<div class='paper-box'>
  <div class='paper-box-text' markdown="1">

  <div class="badge">CVPR 2026</div>

  [Beyond Multiple Choice: Verifiable OpenQA for Robust Vision-Language RFT](https://arxiv.org/abs/2511.17405)

  Yesheng Liu, **Hao Li**, Haiyu Xu, Baoqi Pei, Jiahao Wang, Mingxuan Zhao, Jingshu Zheng, Zheqi He, JG Yao, Bowen Qin, Xi Yang, Jiajun Zhang

  <span class="paper-tldr">**TL;DR:** Multiple-choice options leak exploitable signals that inflate scores and reward guessing during RFT; ReVeL rewrites them into open-form yet still verifiable questions, improving OpenQA accuracy by ~6 points and exposing up to 20 points of MCQA score inflation.</span>

  <!-- [**Code**](#) <strong><span class='show_paper_citations' data='fan-etal-2025-metaflowllm'></span></strong>   -->
  </div>
</div>

<div class='paper-box'>
  <div class='paper-box-text' markdown="1">

  <div class="badge">EMNLP 2025</div>

  [Layer-Aware Representation Filtering: Purifying Finetuning Data to Preserve LLM Safety Alignment](https://arxiv.org/abs/2507.18631)

  **Hao Li**\*, Lijun Li*, Zhenghao Lu, Xianyi Wei, Rui Li, Jing Shao, Lei Sha

  <span class="paper-tldr">**TL;DR:** Seemingly benign finetuning data hides safety-degrading features; LARF locates safety-sensitive layers and uses their representations to filter those samples out, mitigating the alignment degradation that downstream finetuning otherwise causes.</span>

  <!-- [**Code**](#) <strong><span class='show_paper_citations' data='fan-etal-2025-metaflowllm'></span></strong>   -->
  </div>
</div>

<div class='paper-box'>
  <div class='paper-box-text' markdown="1">

  <div class="badge">EMNLP 2025 Oral</div>

  [DiffusionAttacker: Diffusion-Driven Prompt Manipulation for LLM Jailbreak](https://arxiv.org/abs/2412.17522)

  Hao Wang, **Hao Li**, Junda Zhu, Xinyuan Wang, Chengwei Pan, Minlie Huang, Lei Sha

  <span class="paper-tldr">**TL;DR:** A seq2seq text diffusion model rewrites harmful prompts end-to-end, steered by an attack loss and Gumbel-Softmax differentiable sampling, which frees the attack from suffix templates and iterative token search while beating prior methods on success rate, fluency, and diversity.</span>

  <!-- [**Code**](#) <strong><span class='show_paper_citations' data='fan-etal-2025-metaflowllm'></span></strong>   -->
  </div>
</div>

<div class='paper-box'>
  <div class='paper-box-text' markdown="1">

  <div class="badge">ACL 2025 Outstanding Paper</div>

  [LLMs know their vulnerabilities: Uncover Safety Gaps through Natural Distribution Shifts](https://arxiv.org/abs/2410.10700v2)

  Qibing Ren\*, **Hao Li**\*, Dongrui Liu, Zhanxu Xie, Xiaoya Lu, Yu Qiao, Lei Sha, Junchi Yan, Lizhuang Ma, Jing Shao

  <span class="paper-tldr">**TL;DR:** Grounded in actor-network theory, ActorBreaker mines actors tied to a toxic goal within the pre-training distribution and builds multi-turn benign-looking prompts that walk models into unsafe content — revealing that safety training covers too narrow a semantic space.</span>

  <!-- [**Code**](#) <strong><span class='show_paper_citations' data='fan-etal-2025-metaflowllm'></span></strong>   -->
  </div>
</div>


<div class='paper-box'>
  <div class='paper-box-text' markdown="1">

  <div class="badge">ACL 2025</div>

  [VLSBench: Unveiling Visual Leakage in Multimodal Safety](https://arxiv.org/abs/2411.19939)

  Xuhao Hu, Dongrui Liu, **Hao Li**, Xuanjing Huang, Jing Shao

  <span class="paper-tldr">**TL;DR:** Existing multimodal safety benchmarks leak the image's risky content into the text query, so models can refuse from text alone; the leakage-free VLSBench (2.2k pairs) restores reliable cross-modal evaluation and challenges LLaVA, Qwen2-VL, and GPT-4o alike.</span>

  <!-- [**Code**](#) <strong><span class='show_paper_citations' data='fan-etal-2025-metaflowllm'></span></strong>   -->
  </div>
</div>

<div class='paper-box'>
  <div class='paper-box-text' markdown="1">

  <div class="badge">EMNLP 2024 Oral</div>

  [ASETF: A Novel Method for Jailbreak Attack on LLMs through Translate Suffix Embeddings](https://arxiv.org/abs/2402.16006)

  Hao Wang\*, **Hao Li**\*, Minlie Huang, Lei Sha

  <span class="paper-tldr">**TL;DR:** Translating continuous adversarial suffix embeddings into coherent natural text replaces costly discrete token search, yielding fluent, perplexity-filter-resistant and transferable jailbreak prompts at a fraction of the compute.</span>

  <!-- [**Code**](#) <strong><span class='show_paper_citations' data='fan-etal-2025-metaflowllm'></span></strong>   -->
  </div>
</div>

# 📝 Reports

- [AISafetyLab: A Comprehensive Framework for AI Safety Evaluation and Improvement](https://arxiv.org/abs/2502.16776), CoAI & Lesca Group

- [SafeWork-R1: Coevolving Safety and Intelligence under the AI-45 Law](https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=iZcvrH8AAAAJ&citation_for_view=iZcvrH8AAAAJ:Y0pCki6q_DkC), Shanghai AI Lab

# 📖 Educations
- *2024.09 - present*, Master, Beihang University, Beijing.
- *2020.09 - 2024.06*, Bachelor, Beihang University, Beijing.


# 🎖 Selected  Honors and Awards
- *2025*, National Scholarship in China.
- *2023*, Special Prize (Top 1) in "Challenge Cup" Competition of Science Achievement in China.

# 🧩 Academic Services
- Conference Review: ACL, EMNLP, NAACL
- Workshop Challenge Organizer: Trustworthy Multi-modal Foundation Models and AI Agents ([TiFA](https://icml-tifa.github.io/)) in ICML 2024.

# 💻 Internships
- *2026.03 - 2026.06*, Agentic RL, TikTok AI Innovation Center
- *2025.08 - 2026.01*, VLM post-training & evaluation, BAAI
- *2024.07 – 2025.07*, LLM and VLM safety, Shanghai AI Lab
