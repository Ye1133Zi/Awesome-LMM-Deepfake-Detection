# Awesome-LMM-Deepfake-Detection ![Awesome](https://awesome.re/badge.svg)
> **Defending against AIGC: Tracking the latest papers and datasets on Deepfake Detection using Large Multimodal Models (LMMs).**  
> 大模型时代的视觉-语言多模态伪造检测、定位与可解释性推理学术汇总。
---

> 🚧 **WIP & Disclaimer (建设中说明)**  
> Ironically, while this repository is dedicated to *Defending against AIGC*, I have utilized AI tools to assist in accelerating the initial framework building and summary generation! 🤖 **Manual content verification is actively ongoing.** At this early stage, please be aware that some paper descriptions or links may not perfectly align. Thank you for your patience!  
> *(免责声明：虽然本仓库致力于“防范 AIGC”，但在初期的框架搭建与摘要整理阶段，为了提高效率，我借助了 AI 工具辅助生成。**后续我将持续进行严格的人工核查。** 当前阶段，部分论文的描述文字与链接可能暂未完全对齐，敬请谅解！)*
> 
---



This repository is maintained based on the survey paper:  
📖 "[Deepfake detection in the era of large models (大模型时代的伪造检测综述)](http://scis.scichina.com/cn/2026/SSI-2025-0289.pdf)" by Peng et al.

---



## 🔥 News / Updates
* **[2026.03]** Repository initialized! First batch of papers and datasets added based on our survey. Welcome to contribute!

---


## 📑 Table of Contents

- [1. Multimodal Detection (多模态伪造检测)](#1-multimodal-detection)
- [2. Explainable Reasoning (可解释推理与问答)](#2-explainable-reasoning)
- [3. Model-Specific Detection (特定生成模型检测)](#3-model-specific-detection)
- [4. Datasets & Benchmarks (数据集与基准)](#4-datasets--benchmarks)
- [5. Emerging Trends (前沿探索与其它)](#5-emerging-trends)
- [6. Surveys & Related Resources (综述与Awesome列表)](#6-surveys--related-resources)


描述内容和链接不保证完全对应
## 1. Multimodal Detection (多模态伪造检测)
> While examining the information of each modality individually, cross-modal analysis and semantic detection are also performed. It mainly involves many scenarios such as news detection, social media detection, and meeting audio and video detection.

<details open>
  <summary>2026</summary>
  
  *(Waiting for new breakthroughs...)*
</details>

<details open>
  <summary>2025</summary>

* [AAAI 2025] Each Fake News is Fake in Its Own Way: An Attribution Multi-Granularity Benchmark for Multimodal Fake News Detection [Paper](https://arxiv.org/abs/2501.00000) [Code](https://github.com/mazihan880/AMG-An-Attributing-Multi-modal-Fake-News-Dataset)
  > 提出了一个归因多粒度基准，涵盖五种伪造类型的细粒度归因标签，强调图文之间的跨模态一致性与时序关系.

</details>

<details open>
  <summary>2024</summary>

* [ACM MM 2024] FKA-Owl: Advancing Multimodal Fake News Detection through Knowledge-Augmented LVLMs [Paper](https://arxiv.org/abs/2400.00000)
  > 通过将伪造特定知识注入视觉语言大模型(LVLM)，增强了跨模态语义检测的鲁棒性.

* [CVPR 2024] SNIFFER: Multimodal Large Language Model for Explainable Out-of-Context Misinformation Detection [Paper](https://arxiv.org/abs/2400.00000)
  > 专为检测脱离上下文(OOC)虚假信息设计的多模态大语言模型，结合内外部验证机制同时输出判断结果和可解释理由.

</details>

<details open>
  <summary>2023</summary>

* [CVPR 2023] Detecting and Grounding Multi-Modal Media Manipulation [Paper](https://arxiv.org/abs/2304.02556) [Code](https://github.com/rshaojimmy/MultiModal-DeepFake)
  > 结合ViT和BERT，通过浅层对齐和深层跨注意力机制，旨在检测和定位多模态媒体的操控.

</details>

---

## 2. Explainable Reasoning (可解释推理与问答)
> Leveraging LLMs/LMMs to generate visual question answering (VQA), causal chains, and fine-grained natural language descriptions of forgery artifacts.

<details open>
  <summary>2026</summary>
</details>

<details open>
  <summary>2025</summary>

* [CVPR 2025] Rethinking Vision-Language Model in Face Forensics: Multi-modal Interpretable Forged Face Detector [Paper](https://arxiv.org/abs/2501.00000) [Code](https://github.com/CHELSEA234/M2F2_Det)
  > 引入通用伪造提示和层级伪造标记，利用LLaVA（lora微调）+CLIP+deepfake model的方式，提升伪造检测的准确性和解释能力.
</details>

<details open>
  <summary>2024</summary>

* [ECCV 2024] Common Sense Reasoning for Deepfake Detection [Paper](https://arxiv.org/abs/2407.01633) [Code](https://github.com/Reality-Defender/Research-DD-VQA.git)
  > 将问题文本转化为上下文表示并与视觉词元进行跨模态对齐，同时提供真假判断与基于常识的解释.

* [NeurIPS 2024] A Hitchhiker's Guide to Fine-Grained Face Forgery Detection using Common Sense Reasoning [Paper](https://arxiv.org/abs/2410.00000) [Code](https://github.com/NickyFot/Hitchhikers_Guide)
  > 将人脸伪造检测任务转换为视觉问答(VQA)任务，并在细粒度多标签识别与自然语言解释层面进行全面评估.

* [ArXiv 2024] FakeShield: Explainable Image Forgery Detection and Localization via Multi-modal Large Language Models [Paper](https://arxiv.org/abs/2410.02761)
  > 结合多模态大语言模型的可解释框架，通过分析篡改图像及掩码精确定位篡改区域并生成文本描述.

* [ArXiv 2024] ForgeryGPT: Multimodal Large Language Model for Explainable Image Forgery Detection and Localization [Paper](https://arxiv.org/abs/2410.10238)
  > 构建视觉词汇表与掩码感知机制，将伪造区域掩码转化为提示，引导GPT-4生成高一致性的解释性文本.

</details>

---

## 3. Model-Specific Detection (特定生成模型检测)
> Detection methods specifically targeting architectures like Diffusion Models (Stable Diffusion, Sora) or GANs.

<details open>
  <summary>2026</summary>
</details>

<details open>
  <summary>2024</summary>

* [ACM CCS 2024] ZeroFake: Zero-shot detection of fake images generated and edited by text-to-image generation models [Paper](https://arxiv.org/abs/2400.00000)
  > 针对SD等生成图像，利用BLIP自动生成图像描述提示词，并构造对抗性提示进行零样本伪造检测.

* [NeurIPS 2024] On Learning Multi-Modal Forgery Representation for Diffusion Generated Video Detection [Paper](https://arxiv.org/abs/2410.23623) [Code](https://github.com/SparkleXFantasy/MM-Det)
  > 结合CLIP图像编码器与多模态大模型，检测扩散模型生成的视频内容伪造，强调时序不一致性建模.

* [ArXiv 2024] MFCLIP: Multi-modal Fine-grained CLIP for Generalizable Diffusion Face Forgery Detection [Paper](https://arxiv.org/abs/2400.00000)
  > 在CLIP基础上引入图像与噪声模态的细粒度特征提取机制，提升了模型对扩散图像伪造辨识的泛化性.

</details>

---

## 4. Datasets & Benchmarks (数据集与基准)
> Including multi-modal forgery benchmarks, VQA datasets, and prompt-guided generation datasets, sorted by release year.

<details open>
  <summary>2026</summary>
</details>

<details open>
  <summary>2025</summary>

* **Forensics-Bench** (2025) [Dataset](https://github.com/Forensics-Bench)
  > 专门面向LVLMs检测评估的数据集，包含63,292个样本，覆盖21类复杂伪造操作与多项选择推理.

* **FakeClue** (2025)
  > 包含超10万张图像，采用多模型联合标注，为每张图生成细粒度自然语言描述并标注纹理等伪造线索.

* **VLForgery** (2025)
  > 面向扩散模型人脸伪造检测，包含54万+张图像，提供包含检测、归因与EkCot推理链条描述的结构化文本.

* **MMFakeBench** (2025) [Dataset](https://github.com/liuxuannan/MMFakeBench)
  > 混合来源的大型图文虚假信息检测基准，包含11,000个图文对，涵盖真实数据伪造、AI合成及语义错配等.

</details>

<details open>
  <summary>2024</summary>

* **SID-Set** (2024)
  > 包含30万张真实、生成与篡改图像，涵盖复杂伪造形式，并配有GPT-4O注释信息与3000条解释.

* **FakeBench** (2024)
  > 面向多维度伪造解释任务，包含6000张图像与5.4万个QA对，支持检测判断、因果解释等四类任务.

* **AMG** (2024) [Dataset](https://github.com/mazihan880/AMG-An-Attributing-Multi-modal-Fake-News-Dataset)
  > 大规模多模态假新闻归因数据集，包含5022个图文对，引入实体、事件与时间不一致等五类伪造归因标签.

* **DD-VQA** (2024) [Dataset](https://github.com/Reality-Defender/Research-DD-VQA.git)
  > 图像伪造问答数据集，包含2968张图像与14782个图文问答对，提供真假判断与基于常识的解释文本.

</details>

<details open>
  <summary>2023</summary>

* **DGM4** (2023)
  > 聚焦人物新闻的伪造数据集，包含23万图像-文本对，设计了人脸替换、文本情感篡改等四种篡改类型.

* **COCOFake** (2023)
  > 大规模文本图像伪造检测数据集，包含11万真实图像与120万通过Stable Diffusion生成的伪造图像.

</details>

---

## 5. Emerging Trends (前沿探索与其它)
> Hallucination mitigation, model capability evaluations, zero-shot generalization, and fairness in LMM forensics.

<details open>
  <summary>2026</summary>
</details>

<details open>
  <summary>2025</summary>

* [AAAI 2025] C2P-CLIP: Injecting Category Common Prompt in CLIP to Enhance Generalization in Deepfake Detection [Paper](https://arxiv.org/abs/2501.00000) [Code](https://github.com/chuangchuangtan/C2P-CLIP-Deepfake_Detection)
  > 向文本提示中注入“类别通用提示”，形成新的训练语义，增强CLIP编码器对真假图像的泛化判别能力.

</details>

<details open>
  <summary>2024</summary>

* [CVPR 2024] LION: Empowering Multimodal Large Language Model with Dual-Level Visual Knowledge [Paper](https://arxiv.org/abs/2400.00000)
  > 引入图像级与区域级视觉知识嵌入机制，通过软标签提示引导推理过程，显著降低大模型的幻觉率.

* [CVPR 2024] Can ChatGPT Detect DeepFakes? A Study of Using Multimodal Large Language Models for Media Forensics [Paper](https://arxiv.org/abs/2404.00000) [Code](https://github.com/shanface33/GPT4MF_UB)
  > 系统评估GPT-4V等主流大模型在伪造识别中的性能，揭示其在真实性判断、推理构建与鲁棒性等方面的局限.

</details>

---

## 6. Surveys & Resources (综述与开源资源)
> A collection of comprehensive survey papers and other high-quality repositories in the field.

<details open>
  <summary>2025</summary>

* 📖 **[Sci Sin Inform 2025]** A Survey on Deepfake Detection in the Era of Large Models (大模型时代的伪造检测综述)
  > *Peng et al.* - 本仓库的核心支撑综述，首次系统性聚焦于多模态大模型背景发展下的伪造检测技术.

</details>

<details open>
  <summary>2024</summary>

* 📖 **[ArXiv 2024]** Deepfake media generation and detection in the generative ai era: A survey and outlook
  > *Croitoru et al.*

</details>

<details open>
  <summary>2023</summary>

* 📖 **[IEEE Access 2023]** A survey on the detection and impacts of deepfakes in visual, audio, and textual formats
  > *Mubarak et al.*

</details>
