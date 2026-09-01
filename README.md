# Awesome Transformer Tracking with stars

This repository is a paper digest of [Transformer](https://arxiv.org/abs/1706.03762)-related approaches in visual tracking tasks. Currently, tasks in this repository include **Unified Tracking (UT)**, **Single Object Tracking (SOT)** and **3D Single Object Tracking (3DSOT)**. Note that some trackers involving a [Non-Local](https://arxiv.org/abs/1711.07971) attention mechanism are also collected. Papers are listed in alphabetical order of the first character.

### :link:Jump to:

* ### \[[Unified Tracking](https://github.com/Little-Podi/Transformer_Tracking#bookmarkunified-tracking-ut) ⭐ 391 | 🐛 0 | 📅 2026-07-26]
* ### \[[Single Object Tracking](https://github.com/Little-Podi/Transformer_Tracking#bookmarksingle-object-tracking-sot) ⭐ 391 | 🐛 0 | 📅 2026-07-26]
* ### \[[3D Single Object Tracking](https://github.com/Little-Podi/Transformer_Tracking#bookmark3d-single-object-tracking-3dsot) ⭐ 391 | 🐛 0 | 📅 2026-07-26]

> \[!NOTE]
> I find it hard to trace all tasks that are related to tracking, including Video Object Segmentation (VOS), Multiple Object Tracking (MOT), Video Instance Segmentation (VIS), Video Object Detection (VOD) and Object Re-Identification (ReID). Hence, I discard all other tracking tasks in a previous update. If you are interested, you can find plenty of collections in [this archived version](https://github.com/Little-Podi/Transformer_Tracking/tree/4cc6050c07dfd4ecbc9f6aa584601a457ed84eb3) ⭐ 391 | 🐛 0 | 📅 2026-07-26. Besides, the most recent trend shows that different tracking tasks are coming to the same avenue.

## :star2:Recommendation

### Game Over???

* **[SAM 2](https://ai.meta.com/SAM2)** \[[paper](https://arxiv.org/abs/2408.00714)] \[[code](https://github.com/facebookresearch/segment-anything-2) ⭐ 19,788 | 🐛 482 | 🌐 Jupyter Notebook | 📅 2026-05-30]
* **[EfficientTAM](https://yformer.github.io/efficient-track-anything)** \[[paper](https://arxiv.org/abs/2411.18933)] \[[code](https://github.com/yformer/EfficientTAM) ⭐ 822 | 🐛 24 | 🌐 Python | 📅 2025-01-06]

### State-of-the-Art Transformer Tracker:two\_hearts::two\_hearts::two\_hearts:

* **AiATrack** (AiATrack: Attention in Attention for Transformer Visual Tracking) \[[paper](https://arxiv.org/abs/2207.09603)] \[[code](https://github.com/Little-Podi/AiATrack) ⭐ 128 | 🐛 1 | 🌐 Python | 📅 2023-12-30] \[[video](https://youtu.be/TqNiOWx9cnI)]
* **GRM** (Generalized Relation Modeling for Transformer Tracking) \[[paper](https://arxiv.org/abs/2303.16580)] \[[code](https://github.com/Little-Podi/GRM) ⭐ 87 | 🐛 1 | 🌐 Python | 📅 2023-12-30] \[[video](https://youtu.be/bQKN3HV-8XI)]

### Up-to-Date Benchmark Results:rocket::rocket::rocket:

![](performance.png)

* Image courtesy: <https://arxiv.org/abs/2302.11867>

### Helpful Learning Resource for Tracking:thumbsup::thumbsup::thumbsup:

* **(Library)** PyTracking: Visual Tracking Library Based on PyTorch \[[code](https://github.com/visionml/pytracking) ⭐ 3,514 | 🐛 82 | 🌐 Python | 📅 2024-08-08]
* **(Survey)** A Deep Dive into Generic Object Tracking: A Survey \[[paper](https://arxiv.org/abs/2507.23251)], Transformers in Single Object Tracking: An Experimental Survey \[[paper](https://arxiv.org/abs/2302.11867)], Visual Object Tracking with Discriminative Filters and Siamese Networks: A Survey and Outlook \[[paper](https://arxiv.org/abs/2112.02838)]
* **(Talk)** Discriminative Appearance-Based Tracking and Segmentation \[[video](https://youtu.be/ILVnBhFq2Ds)], Deep Visual Reasoning with Optimization-Based Network Modules \[[video](https://youtu.be/UR2TlFCrYac)]
* **(People)** Martin Danelljan\@ETH \[[web](https://martin-danelljan.github.io)], Bin Yan\@DLUT \[[web](https://masterbin-iiau.github.io)]

### Recent Trends:fire::fire::fire:

* ### Target Head: Autoregressive Temporal Modeling

  * #### Representative

    * Bounding box as coordinate sequence.
      * **ARTrackV2** \[[CVPR'24](https://github.com/Little-Podi/Transformer_Tracking#cvpr-2024-1) ⭐ 391 | 🐛 0 | 📅 2026-07-26] **ARTrack** \[[CVPR'23](https://github.com/Little-Podi/Transformer_Tracking#cvpr-2023-1) ⭐ 391 | 🐛 0 | 📅 2026-07-26], **SeqTrack** \[[CVPR'23](https://github.com/Little-Podi/Transformer_Tracking#cvpr-2023-1) ⭐ 391 | 🐛 0 | 📅 2026-07-26]

  ![](head.png)

* ### Feature Backbone: Joint Feature Extraction and Interaction

  * #### Advantage

    * Benefit from pre-trained vision Transformer models.
    * Free from randomly initialized correlation modules.
    * More discriminative target-specific feature extraction.
    * Much faster inference and training convergence speed.
    * Simple and generic one-branch tracking framework.

  * #### Roadmap

    * 1st step :feet: feature interaction inside the backbone.
      * **SiamAttn** \[[CVPR'20](https://github.com/Little-Podi/Transformer_Tracking#cvpr-2020) ⭐ 391 | 🐛 0 | 📅 2026-07-26], **SBT** \[[CVPR'22](https://github.com/Little-Podi/Transformer_Tracking#cvpr-2022-1) ⭐ 391 | 🐛 0 | 📅 2026-07-26], **InMo** \[[IJCAI'22](https://github.com/Little-Podi/Transformer_Tracking#ijcai-2022) ⭐ 391 | 🐛 0 | 📅 2026-07-26]
    * 2nd step :feet: concatenation-based feature interaction.
      * **STARK** \[[ICCV'21](https://github.com/Little-Podi/Transformer_Tracking#iccv-2021) ⭐ 391 | 🐛 0 | 📅 2026-07-26], **SwinTrack** \[[NeurIPS'22](https://github.com/Little-Podi/Transformer_Tracking#neurips-2022) ⭐ 391 | 🐛 0 | 📅 2026-07-26]
    * 3rd step :feet: joint feature extraction and interaction.
      * **MixFormer** \[[CVPR'22](https://github.com/Little-Podi/Transformer_Tracking#cvpr-2022-1) ⭐ 391 | 🐛 0 | 📅 2026-07-26], **OSTrack** \[[ECCV'22](https://github.com/Little-Podi/Transformer_Tracking#eccv-2022-1) ⭐ 391 | 🐛 0 | 📅 2026-07-26], **SimTrack** \[[ECCV'22](https://github.com/Little-Podi/Transformer_Tracking#eccv-2022-1) ⭐ 391 | 🐛 0 | 📅 2026-07-26]
    * 4th step :feet: generalized and robust relation modeling.
      * **GRM** \[[CVPR'23](https://github.com/Little-Podi/Transformer_Tracking#cvpr-2023-1) ⭐ 391 | 🐛 0 | 📅 2026-07-26], **ROMTrack** \[[ICCV'23](https://github.com/Little-Podi/Transformer_Tracking#iccv-2023) ⭐ 391 | 🐛 0 | 📅 2026-07-26].
    * 5th step :feet: using SAM foundation models.
      * **SAMURAI**, **SAMITE**

  ![](backbone.png)

## :bookmark:Unified Tracking (UT)

### AAAI 2026

* **SATA** (Tracking and Segmenting Anything in Any Modality) \[[paper](https://arxiv.org/abs/2511.19475)] \[~~code~~]

### Preprint 2025

* **SAM 2++** (SAM 2++: Tracking Anything at Any Granularity) \[[paper](https://arxiv.org/abs/2510.18822)] \[[code](https://github.com/MCG-NJU/SAM2-Plus) ⭐ 71 | 🐛 0 | 🌐 Python | 📅 2025-12-15]

### CVPR 2024

* **GLEE** (General Object Foundation Model for Images and Videos at Scale) \[[paper](https://arxiv.org/abs/2312.09158)] \[[code](https://github.com/FoundationVision/GLEE) ⭐ 1,170 | 🐛 47 | 🌐 Python | 📅 2024-10-21]
* **OmniViD** (OmniVid: A Generative Framework for Universal Video Understanding) \[[paper](https://arxiv.org/abs/2403.17935)] \[[code](https://github.com/wangjk666/OmniVid) ⭐ 58 | 🐛 8 | 🌐 Python | 📅 2024-06-04]

### CVPR 2023

* **UNINEXT** (Universal Instance Perception as Object Discovery and Retrieval) \[[paper](https://arxiv.org/abs/2303.06674)] \[[code](https://github.com/MasterBin-IIAU/UNINEXT) ⭐ 1,279 | 🐛 32 | 🌐 Python | 📅 2023-07-18]
* **OmniTracker** (OmniTracker: Unifying Object Tracking by Tracking-with-Detection) \[[paper](https://arxiv.org/abs/2303.12079)] \[~~code~~]

### ICCV 2023

* **MITS** (Integrating Boxes and Masks: A Multi-Object Framework for Unified Visual Tracking and Segmentation) \[[paper](https://arxiv.org/abs/2308.13266)] \[[code](https://github.com/yoxu515/MITS) ⭐ 22 | 🐛 3 | 🌐 Python | 📅 2024-07-25]

### Preprint 2023

* **TAM** (Track Anything: Segment Anything Meets Videos) \[[paper](https://arxiv.org/abs/2304.11968)] \[[code](https://github.com/gaomingqi/Track-Anything) ⭐ 6,996 | 🐛 114 | 🌐 Python | 📅 2025-12-13]
* **SAM-Track** (Segment and Track Anything) \[[paper](https://arxiv.org/abs/2305.06558)] \[[code](https://github.com/z-x-yang/Segment-and-Track-Anything) ⭐ 3,134 | 🐛 45 | 🌐 Jupyter Notebook | 📅 2026-07-03]
* **HQTrack** (Tracking Anything in High Quality) \[[paper](https://arxiv.org/abs/2307.13974)] \[[code](https://github.com/jiawen-zhu/HQTrack) ⭐ 753 | 🐛 14 | 🌐 Python | 📅 2023-12-01]

### CVPR 2022

* **UTT** (Unified Transformer Tracker for Object Tracking) \[[paper](https://arxiv.org/abs/2203.15175)] \[[code](https://github.com/Flowerfan/Trackron) ⭐ 51 | 🐛 4 | 🌐 Python | 📅 2022-06-20]

### ECCV 2022

* **Unicorn** (Towards Grand Unification of Object Tracking) \[[paper](https://arxiv.org/abs/2207.07078)] \[[code](https://github.com/MasterBin-IIAU/Unicorn) ⭐ 951 | 🐛 23 | 🌐 Python | 📅 2022-10-17]

## :bookmark:Single Object Tracking (SOT)

### CVPR 2026

* **RAGTrack** (RAGTrack: Language-Aware RGBT Tracking with Retrieval-Augmented Generation) \[[paper](https://arxiv.org/abs/2603.03617)] \[[code](https://github.com/IdolLab/RAGTrack) ⭐ 206 | 🐛 3 | 🌐 Python | 📅 2026-08-14]
* **UETrack** (UETrack: A Unified and Efficient Framework for Single Object Tracking) \[[paper](https://arxiv.org/abs/2603.01412)] \[[code](https://github.com/kangben258/UETrack) ⭐ 46 | 🐛 2 | 🌐 Python | 📅 2026-03-20]
* **SpikeTrack** (SpikeTrack: A Spike-Driven Framework for Efficient Visual Tracking) \[[paper](https://arxiv.org/abs/2602.23963)] \[[code](https://github.com/faicaiwawa/SpikeTrack) ⭐ 44 | 🐛 1 | 🌐 Python | 📅 2026-04-08]
* **SEATrack** (SEATrack: Simple, Efficient, and Adaptive Multimodal Tracker) \[[paper](https://arxiv.org/abs/2604.12502)] \[[code](https://github.com/AutoLab-SAI-SJTU/SEATrack) ⭐ 41 | 🐛 3 | 🌐 Python | 📅 2026-05-29]
* **UTPTrack** (UTPTrack: Towards Simple and Unified Token Pruning for Visual Tracking) \[[paper](https://arxiv.org/abs/2602.23734)] \[[code](https://github.com/EIT-NLP/UTPTrack) ⭐ 32 | 🐛 0 | 🌐 Python | 📅 2026-04-05]
* **DTPTrack** (Drift-Resilient Temporal Priors for Visual Tracking) \[[paper](https://arxiv.org/abs/2604.02654)] \[[code](https://github.com/NorahGreen/DTPTrack) ⭐ 14 | 🐛 2 | 🌐 Python | 📅 2026-05-28]

### ICLR 2026

* **GOT-Edit** (GOT-Edit: Geometry-Aware Generic Object Tracking via Online Model Editing) \[[paper\&review](https://openreview.net/forum?id=aVa7etWnwF)] \[[code](https://github.com/chenshihfang/GOT) ⭐ 45 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-07-13]
* **FARTrack** (FARTrack: Fast Autoregressive Visual Tracking with High Performance) \[[paper\&review](https://openreview.net/forum?id=lq7Zfr8kAS)] \[[code](https://github.com/wangguijiepedeval/FARTrack)]

### ICML 2026

* **RELO** (RELO: Reinforcement Learning to Localize for Visual Object Tracking) \[[paper\&review](https://openreview.net/forum?id=IKZcb2jZqM)] \[[code](https://github.com/Multimedia-Analytics-Laboratory/RELO) ⭐ 23 | 🐛 2 | 🌐 Python | 📅 2026-05-16]
* **FATrack** (Foreground-Aware Token Routing Vision Transformer for Real-Time Satellite Video Tracking) \[[paper\&review](https://openreview.net/forum?id=yB0YMDuqqx)] \[~~code~~]
* **OneTrackerV2** (Unified Multimodal Visual Tracking with Dual Mixture-of-Experts) \[[paper\&review](https://openreview.net/forum?id=Eeo0uBd5mt)] \[~~code~~]

### AAAI 2026

* **GOLA** (Group Orthogonal Low-Rank Adaptation for RGB-T Tracking) \[[paper](https://arxiv.org/abs/2512.05359)] \[[code](https://github.com/MelanTech/GOLA) ⭐ 28 | 🐛 3 | 🌐 Python | 📅 2025-12-24]

### ICRA 2026

* **DPTracker** (Dual Prompt-Driven Feature Encoding for Nighttime UAV Tracking) \[[paper](https://arxiv.org/abs/2603.19628)] \[[code](https://github.com/yiheng-wang-duke/DPTracker) ⭐ 4 | 🐛 2 | 🌐 Python | 📅 2026-03-17]

### Preprint 2026

* **SAMOSA** (Segment Anything with Motion, Geometry, and Semantic Adaptation for Complex Nonlinear Visual Object Tracking) \[[paper](https://arxiv.org/abs/2605.22538)] \[[code](https://github.com/DurYi/SAMOSA) ⭐ 11 | 🐛 1 | 🌐 Python | 📅 2026-05-24]
* **APRTrack** (Active Adversarial Perturbation-Driven Associative Memory Retrieval for RGB-Event Visual Object Tracking) \[[paper](https://arxiv.org/abs/2606.26455)] \[[code](https://github.com/Event-AHU/OpenEvTracking) ⭐ 10 | 🐛 1 | 🌐 Python | 📅 2026-07-08]
* **PSMTrack** (Dynamic Pondering Sparsity-Aware Mixture-of-Experts Transformer for Event Stream-Based Visual Object Tracking) \[[paper](https://arxiv.org/abs/2605.06112)] \[[code](https://github.com/Event-AHU/OpenEvTracking) ⭐ 10 | 🐛 1 | 🌐 Python | 📅 2026-07-08]
* **GLAD** (GLAD: Generative Language-Assisted Visual Tracking for Low-Semantic Templates) \[[paper](https://arxiv.org/abs/2602.00570)] \[[code](https://github.com/Confetti-lxy/GLAD) ⭐ 6 | 🐛 0 | 🌐 Python | 📅 2026-03-14]
* **E2EMPT** (End-to-End Unmixing with Material Prompts for Hyperspectral Object Tracking) \[[paper](https://arxiv.org/abs/2605.20569)] \[[code](https://github.com/han030927/E2EMPT) ⭐ 4 | 🐛 1 | 📅 2026-05-21]
* **PATrack** (Learning Progressive Adaptation for Multi-Modal Tracking) \[[paper](https://arxiv.org/abs/2603.21100)] \[[code](https://github.com/ouha1998/Learning-Progressive-Adaptation-for-Multi-Modal-Tracking) ⭐ 3 | 🐛 1 | 🌐 Python | 📅 2025-07-30]
* **VL-UniTrack** (VL-UniTrack: A Unified Framework with Visual-Language Prompts for UAV-Ground Visual Tracking) \[[paper](https://arxiv.org/abs/2605.04574)] \[[code](https://github.com/xuboyue1999/VL-UniTrack) ⭐ 0 | 🐛 1 | 📅 2026-05-06]
* **Diff-Tracking** (Leveraging Text-to-Image Diffusion Models for Unsupervised Visual Object Tracking) \[[paper](https://arxiv.org/abs/2605.26933)] \[~~code~~]
* **SDMoE** (Sparse-Dense Mixture of Experts Adapter for Multi-Modal Tracking) \[[paper](https://arxiv.org/abs/2603.13719)] \[~~code~~]
* **UAV-Track VLA** (UAV-Track VLA: Embodied Aerial Tracking via Vision-Language-Action Models) \[[paper](https://arxiv.org/abs/2604.02241)] \[[code](https://github.com/Hub-Tian/UAVTrack_VLA)]
* **UBATrack** (UBATrack: Spatio-Temporal State Space Model for General Multi-Modal Tracking) \[[paper](https://arxiv.org/abs/2601.14799)] \[~~code~~]
* **Uni-MDTrack** (Uni-MDTrack: Learning Decoupled Memory and Dynamic States for Parameter-Efficient Visual Tracking in All Modality) \[[paper](https://arxiv.org/abs/2603.14452)] \[~~code~~]

### CVPR 2025

* **VL-SAM2** (Underwater Camouflaged Object Tracking Meets Vision-Language SAM2) \[[paper](https://arxiv.org/abs/2409.16902)] \[[code](https://github.com/983632847/Awesome-Multimodal-Object-Tracking) ⭐ 1,057 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-09-01]
* **SAM2.1++** (A Distractor-Aware Memory for Visual Object Tracking with SAM2) \[[paper](https://arxiv.org/abs/2411.17576)] \[[code](https://github.com/jovanavidenovic/DAM4SAM) ⭐ 493 | 🐛 8 | 🌐 Python | 📅 2026-04-07]
* **MITracker** (MITracker: Multi-View Integration for Visual Object Tracking) \[[paper](https://arxiv.org/abs/2502.20111)] \[[code](https://github.com/XuM007/MITracker) ⭐ 138 | 🐛 14 | 🌐 Python | 📅 2025-06-18]
* **SGLATrack** (Similarity-Guided Layer-Adaptive Vision Transformer for UAV Tracking)  \[[paper](https://arxiv.org/abs/2503.06625)] \[[code](https://github.com/GXNU-ZhongLab/SGLATrack) ⭐ 123 | 🐛 9 | 🌐 Python | 📅 2026-08-14]
* **ORTrack** (Learning Occlusion-Robust Vision Transformers for Real-Time UAV Tracking) \[[paper](https://arxiv.org/abs/2504.09228)] \[[code](https://github.com/wuyou3474/ORTrack) ⭐ 122 | 🐛 7 | 🌐 Python | 📅 2025-06-12]
* **UNTrack** (MUST: The First Dataset and Unified Framework for Multispectral UAV Single Object Tracking) \[[paper](https://arxiv.org/abs/2503.17699)] \[[code](https://github.com/q2479036243/MUST-Multispectral-UAV-Single-Object-Tracking) ⭐ 73 | 🐛 8 | 🌐 Python | 📅 2025-05-27]
* **SPMTrack** (SPMTrack: Spatio-Temporal Parameter-Efficient Fine-Tuning with Mixture of Experts for Scalable Visual Tracking) \[[paper](https://arxiv.org/abs/2503.18338)] \[[code](https://github.com/WenRuiCai/SPMTrack) ⭐ 61 | 🐛 8 | 🌐 Python | 📅 2025-10-19]
* **DUTrack** (Dynamic Updates for Language Adaptation in Visual-Language Tracking) \[[paper](https://arxiv.org/abs/2503.06621)] \[[code](https://github.com/GXNU-ZhongLab/DUTrack) ⭐ 44 | 🐛 8 | 🌐 Python | 📅 2025-03-27]
* **ARGTrack** (Autoregressive Sequential Pretraining for Visual Tracking) \[[paper](https://openaccess.thecvf.com/content/CVPR2025/html/Liang_Autoregressive_Sequential_Pretraining_for_Visual_Tracking_CVPR_2025_paper.html)] \[~~code~~]
* **DreamTrack** (DreamTrack: Dreaming the Future for Multimodal Visual Object Tracking) \[[paper](https://openaccess.thecvf.com/content/CVPR2025/html/Guo_DreamTrack_Dreaming_the_Future_for_Multimodal_Visual_Object_Tracking_CVPR_2025_paper.html)] \[~~code~~]

### NeurIPS 2025

* **DSATrack** (Dynamic Semantic-Aware Correlation Modeling for UAV Tracking) \[[paper\&review](https://openreview.net/forum?id=7lLnWh0otf)] \[~~code~~]
* **LoRATv2** (LoRATv2: Enabling Low-Cost Temporal Modeling in One-Stream Trackers) \[[paper\&review](https://openreview.net/forum?id=q06YjUj0FB)] \[~~code~~]

### ICCV 2025

* **ATCTrack** (ATCTrack: Aligning Target-Context Cues with Dynamic Target States for Robust Vision-Language Tracking) \[[paper](https://arxiv.org/abs/2507.19875)] \[[code](https://github.com/XiaokunFeng/ATCTrack) ⭐ 119 | 🐛 4 | 🌐 Python | 📅 2025-08-23]
* **UMDATrack** (UMDATrack: Unified Multi-Domain Adaptive Tracking Under Adverse Weather Conditions) \[[paper](https://arxiv.org/abs/2507.00648)] \[[code](https://github.com/Z-Z188/UMDATrack) ⭐ 44 | 🐛 3 | 🌐 Python | 📅 2026-02-10]
* **XTrack** (XTrack: Multimodal Training Boosts RGB-X Video Object Trackers) \[[paper](https://arxiv.org/abs/2405.17773)] \[[code](https://github.com/supertyd/XTrack) ⭐ 38 | 🐛 0 | 🌐 Python | 📅 2025-07-11]
* **CompressTracker** (General Compression Framework for Efficient Transformer Object Tracking) \[[paper](https://arxiv.org/abs/2409.17564)] \[[code](https://github.com/LingyiHongfd/CompressTracker) ⭐ 25 | 🐛 5 | 🌐 Python | 📅 2025-11-16]
* **FlexTrack** (What You Have is What You Track: Adaptive and Robust Multimodal Tracking) \[[paper](https://arxiv.org/abs/2507.05899)] \[[code](https://github.com/supertyd/FlexTrack) ⭐ 22 | 🐛 3 | 📅 2026-08-27]
* **TUE** (Temporal Unlearnable Examples: Preventing Personal Video Data from Unauthorized Exploitation by Object Tracking) \[[paper](https://arxiv.org/abs/2507.07483)] \[~~code~~]

### ICML 2025

* **CSTrack** (CSTrack: Enhancing RGB-X Tracking via Compact Spatiotemporal Features) \[[paper](https://arxiv.org/abs/2505.19434)] \[[code](https://github.com/XiaokunFeng/CSTrack) ⭐ 112 | 🐛 5 | 🌐 Python | 📅 2025-08-23]
* **MPT** (Efficient Motion Prompt Learning for Robust Visual Tracking) \[[paper](https://arxiv.org/abs/2505.16321)] \[[code](https://github.com/zj5559/Motion-Prompt-Tracking) ⭐ 31 | 🐛 1 | 🌐 Python | 📅 2025-12-17]

### AAAI 2025

* **CADTrack** (CADTrack: Learning Contextual Aggregation with Deformable Alignment for Robust RGBT Tracking) \[[paper](https://arxiv.org/abs/2511.17967)] \[[code](https://github.com/IdolLab/CADTrack) ⭐ 189 | 🐛 0 | 🌐 Python | 📅 2026-06-03]
* **SUTrack** (SUTrack: Towards Simple and Unified Single Object Tracking) \[[paper](https://arxiv.org/abs/2412.19138)] \[[code](https://github.com/chenxin-dlut/SUTrack) ⭐ 168 | 🐛 12 | 🌐 Python | 📅 2025-06-16]
* **MCITrack** (Exploring Enhanced Contextual Information for Video-Level Object Tracking) \[[paper](https://arxiv.org/abs/2412.11023)] \[[code](https://github.com/kangben258/MCITrack) ⭐ 118 | 🐛 9 | 🌐 Python | 📅 2024-12-17]
* **STTrack** (Exploiting Multimodal Spatial-Temporal Patterns for Video Object Tracking) \[[paper](https://arxiv.org/abs/2412.15691)] \[[code](https://github.com/NJU-PCALab/STTrack) ⭐ 118 | 🐛 7 | 🌐 Python | 📅 2025-05-18]
* **AsymTrack** (Two-Stream Beats One-Stream: Asymmetric Siamese Network for Efficient Visual Tracking) \[[paper](https://arxiv.org/abs/2503.00516)] \[[code](https://github.com/jiawen-zhu/AsymTrack) ⭐ 55 | 🐛 9 | 🌐 Python | 📅 2025-03-04]
* **MambaLCT** (MambaLCT: Boosting Tracking via Long-Term Context State Space Model) \[[paper](https://arxiv.org/abs/2412.13615)] \[[code](https://github.com/GXNU-ZhongLab/MambaLCT) ⭐ 24 | 🐛 3 | 🌐 Python | 📅 2024-12-20]
* **TemTrack** (Robust Tracking via Mamba-Vased Context-Aware Token Learning) \[[paper](https://arxiv.org/abs/2412.13611)] \[[code](https://github.com/GXNU-ZhongLab/TemTrack) ⭐ 16 | 🐛 2 | 📅 2025-11-06]
* **LMTrack** (Less is More: Token Context-Aware Learning for Object Tracking) \[[paper](https://arxiv.org/abs/2501.00758)] \[[code](https://github.com/XuChenLong/LMTrack) ⭐ 13 | 🐛 4 | 🌐 Python | 📅 2025-07-09]
* **SpikeFET** (Fully Spiking Neural Networks for Unified Frame-Event Object Tracking) \[[paper](https://arxiv.org/abs/2505.20834)] \[~~code~~]

### IJCAI 2025

* **GDSTrack** (Modality-Guided Dynamic Graph Fusion and Temporal Diffusion for Self-Supervised RGB-T Tracking) \[[paper](https://arxiv.org/abs/2505.03507)] \[[code](https://github.com/LiShenglana/GDSTrack) ⭐ 6 | 🐛 1 | 🌐 Python | 📅 2025-05-29]

### MM 2025

* **RSTrack** (Explicit Context Reasoning with Supervision for Visual Tracking) \[[paper](https://arxiv.org/abs/2507.16191)] \[[code](https://github.com/GXNU-ZhongLab/RSTrack) ⭐ 18 | 🐛 2 | 📅 2025-07-20]
* **MST** (Multi-State Tracker: Enhancing Efficient Object Tracking via Multi-State Specialization and Interaction) \[[paper](https://arxiv.org/abs/2508.11531)] \[[code](https://github.com/wsumel/MST) ⭐ 10 | 🐛 3 | 🌐 Python | 📅 2025-08-20]
* **SymTrack** (Serial Over Parallel: Learning Continual Unification for Multi-Modal Visual Object Tracking and Benchmarking) \[[paper](https://arxiv.org/abs/2508.10655)] \[[code](https://github.com/Zhangyong-Tang/UniBench300) ⭐ 5 | 🐛 1 | 📅 2025-09-22]

### ICRA 2025

* **CGTrack** (CGTrack: Cascade Gating Network with Hierarchical Feature Aggregation for UAV Tracking) \[[paper](https://arxiv.org/abs/2505.05936)] \[[code](https://github.com/Nightwatch-Fox11/CGTrack) ⭐ 2 | 🐛 1 | 📅 2025-02-28]

### ICASSP 2025

* **CTVLT** (Enhancing Vision-Language Tracking by Effectively Converting Textual Cues into Visual Cues) \[[paper](https://arxiv.org/abs/2412.19648)] \[[code](https://github.com/XiaokunFeng/CTVLT) ⭐ 19 | 🐛 4 | 🌐 Jupyter Notebook | 📅 2024-12-31]

### Preprint 2025

* **COST** (COST: Contrastive One-Stage Transformer for Vision-Language Small Object Tracking) \[[paper](https://arxiv.org/abs/2504.01321)] \[[code](https://github.com/983632847/Awesome-Multimodal-Object-Tracking) ⭐ 1,057 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-09-01]
* **UM-ODTrack** (Towards Universal Modal Tracking with Online Dense Temporal Token Learning) \[[paper](https://arxiv.org/abs/2507.20177)] \[[code](https://github.com/GXNU-ZhongLab/ODTrack) ⭐ 192 | 🐛 11 | 🌐 Python | 📅 2024-10-07]
* **HDETrackV2** (Event Stream-Based Visual Object Tracking: HDETrack V2 and A High-Definition Benchmark) \[[paper](https://arxiv.org/abs/2502.05574)] \[[code](https://github.com/Event-AHU/EventVOT_Benchmark) ⭐ 149 | 🐛 4 | 🌐 Python | 📅 2026-03-25]
* **R1-Track** (R1-Track: Direct Application of MLLMs to Visual Object Tracking via Reinforcement Learning) \[[paper](https://arxiv.org/abs/2506.21980)] \[[code](https://github.com/Wangbiao2/R1-Track) ⭐ 66 | 🐛 0 | 🌐 Python | 📅 2025-05-14]
* **DyHiT** (Exploiting Lightweight Hierarchical ViT and Dynamic Framework for Efficient Visual Tracking) \[[paper](https://arxiv.org/abs/2506.20381)] \[[code](https://github.com/kangben258/HiT) ⭐ 60 | 🐛 4 | 🌐 Python | 📅 2025-09-25]
* **FocusTrack** (FocusTrack: A Self-Adaptive Local Sampling Algorithm for Efficient Anti-UAV Tracking) \[[paper](https://arxiv.org/abs/2504.13604)] \[[code](https://github.com/vero1925/FocusTrack) ⭐ 37 | 🐛 5 | 🌐 Python | 📅 2025-04-21]
* **ReasoningTrack** (ReasoningTrack: Chain-of-Thought Reasoning for Long-term Vision-Language Tracking) \[[paper](https://arxiv.org/abs/2508.05221)] \[[code](https://github.com/Event-AHU/Open_VLTrack) ⭐ 36 | 🐛 1 | 🌐 Python | 📅 2026-07-04]
* **UncTrack** (UncTrack: Reliable Visual Object Tracking with Uncertainty-Aware Prototype Memory Network) \[[paper](https://arxiv.org/abs/2503.12888)] \[[code](https://github.com/ManOfStory/UncTrack) ⭐ 17 | 🐛 1 | 🌐 Python | 📅 2025-06-16]
* **SAMITE** (SAMITE: Position Prompted SAM2 with Calibrated Memory for Visual Object Tracking) \[[paper](https://arxiv.org/abs/2507.21732)] \[[code](https://github.com/Sam1224/SAMITE) ⭐ 14 | 🐛 2 | 🌐 Python | 📅 2025-07-29]
* **HotMoE** (HotMoE: Exploring Sparse Mixture-of-Experts for Hyperspectral Object Tracking) \[[paper](https://ieeexplore.ieee.org/document/10855488)] \[[code](https://github.com/supertyd/hotmoe) ⭐ 9 | 🐛 0 | 🌐 Python | 📅 2025-07-09]
* **ISTASTrack** (ISTASTrack: Bridging ANN and SNN via ISTA Adapter for RGB-Event Tracking) \[[paper](https://arxiv.org/abs/2509.09977)] \[[code](https://github.com/lsying009/ISTASTrack) ⭐ 8 | 🐛 1 | 🌐 Python | 📅 2026-05-28]
* **MMTrack** (Visual and Memory Dual Adapter for Multi-Modal Object Tracking) \[[paper](https://arxiv.org/abs/2506.23972)] \[[code](https://github.com/xuboyue1999/mmtrack) ⭐ 8 | 🐛 2 | 🌐 Python | 📅 2026-03-28]
* **SFTrack** (Towards Low-Latency Event Stream-Based Visual Object Tracking: A Slow-Fast Approach) \[[paper](https://arxiv.org/abs/2505.12903)] \[[code](https://github.com/Event-AHU/SlowFast_Event_Track) ⭐ 5 | 🐛 1 | 🌐 Python | 📅 2026-05-14]
* **APTrack** (Adaptive Perception for Unified Visual Multi-Modal Object Tracking) \[[paper](https://arxiv.org/abs/2502.06583)] \[~~code~~]
* **ATSTrack** (ATSTrack: Enhancing Visual-Language Tracking by Aligning Temporal and Spatial Scales) \[[paper](https://arxiv.org/abs/2507.00454)] \[~~code~~]
* **BFTrans** (Target-Aware Bidirectional Fusion Transformer for Aerial Object Tracking) \[[paper](https://arxiv.org/abs/2503.09951)] \[~~code~~]
* **DMTrack** (DMTrack: Spatio-Temporal Multimodal Tracking via Dual-Adapter) \[[paper](https://arxiv.org/abs/2508.01592)] \[~~code~~]
* **DT-Training** (Progressive Scaling Visual Object Tracking) \[[paper](https://arxiv.org/abs/2505.19990)] \[~~code~~]
* **SDTrack** (SDTrack: A Baseline for Event-Based Tracking via Spiking Neural Networks) \[[paper](https://arxiv.org/abs/2503.08703)] \[~~code~~]
* **TRACT** (Attention to Trajectory: Trajectory-Aware Open-Vocabulary Tracking) \[[paper](https://arxiv.org/abs/2503.08145)] \[~~code~~]
* **UASTrack** (UASTrack: A Unified Adaptive Selection Framework with Modality-Customization in Single Object Tracking) \[[paper](https://arxiv.org/abs/2502.18220)] \[[code](https://github.com/wanghe/UASTrack)]
* **UAUTrack** (UAUTrack: Towards Unified Multimodal Anti-UAV Visual Tracking) \[[paper](https://arxiv.org/abs/2512.02668)] \[~~code~~]
* **UniSOT** (UniSOT: A Unified Framework for Multi-Modality Single Object Tracking) \[[paper](https://arxiv.org/abs/2511.01427)] \[~~code~~]
* **VFPTrack** (Robust RGB-T Tracking via Learnable Visual Fourier Prompt Fine-Tuning and Modality Fusion Prompt Generation) \[[paper](https://arxiv.org/abs/2509.19733)] \[~~code~~]

### CVPR 2024

* **ARTrackV2** (ARTrackV2: Prompting Autoregressive Tracker Where to Look and How to Describe) \[[paper](https://arxiv.org/abs/2312.17133)] \[[code](https://github.com/MIV-XJTU/ARTrack) ⭐ 320 | 🐛 9 | 🌐 Python | 📅 2025-10-20]
* **HDETrack** (Event Stream-Based Visual Object Tracking: A High-Resolution Benchmark Dataset and A Novel Baseline) \[[paper](https://arxiv.org/abs/2309.14611)] \[[code](https://github.com/Event-AHU/EventVOT_Benchmark) ⭐ 149 | 🐛 4 | 🌐 Python | 📅 2026-03-25]
* **AQATrack** (Autoregressive Queries for Adaptive Tracking with Spatio-Temporal Transformers) \[[paper](https://arxiv.org/abs/2403.10574)] \[[code](https://github.com/GXNU-ZhongLab/AQATrack) ⭐ 73 | 🐛 4 | 🌐 Python | 📅 2024-08-04]
* **HIPTrack** (HIPTrack: Visual Tracking with Historical Prompts) \[[paper](https://arxiv.org/abs/2311.02072)] \[[code](https://github.com/WenRuiCai/HIPTrack) ⭐ 72 | 🐛 4 | 🌐 Python | 📅 2024-05-04]
* **SDSTrack** (SDSTrack: Self-Distillation Symmetric Adapter Learning for Multi-Modal Visual Object Tracking) \[[paper](https://arxiv.org/abs/2403.16002)] \[[code](https://github.com/hoqolo/SDSTrack) ⭐ 70 | 🐛 6 | 🌐 Python | 📅 2024-06-30]
* **Un-Track** (Single-Model and Any-Modality for Video Object Tracking) \[[paper](https://arxiv.org/abs/2311.15851)] \[[code](https://github.com/Zongwei97/UnTrack) ⭐ 69 | 🐛 2 | 🌐 Python | 📅 2024-10-19]
* **DiffusionTrack** (DiffusionTrack: Point Set Diffusion Model for Visual Object Tracking) \[[paper](https://openaccess.thecvf.com/content/CVPR2024/html/Xie_DiffusionTrack_Point_Set_Diffusion_Model_for_Visual_Object_Tracking_CVPR_2024_paper.html)] \[[code](https://github.com/VISION-SJTU/DiffusionTrack) ⭐ 42 | 🐛 11 | 🌐 Python | 📅 2025-08-20]
* **QueryNLT** (Context-Aware Integration of Language and Visual References for Natural Language Tracking) \[[paper](https://arxiv.org/abs/2403.19975)] \[[code](https://github.com/twotwo2/QueryNLT) ⭐ 6 | 🐛 3 | 📅 2024-03-28]
* **OneTracker** (OneTracker: Unifying Visual Object Tracking with Foundation Models and Efficient Tuning) \[[paper](https://arxiv.org/abs/2403.09634)] \[~~code~~]

### NeurIPS 2024

* **OKTrack** (WebUOT-1M: Advancing Deep Underwater Object Tracking with A Million-Scale Benchmark) \[[paper\&review](https://openreview.net/forum?id=cLS4fLIA5P)] \[[code](https://github.com/983632847/Awesome-Multimodal-Object-Tracking) ⭐ 1,057 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-09-01]
* **MemVLT** (MemVLT: Vision-Language Tracking with Adaptive Memory-Based Prompts) \[[paper\&review](https://openreview.net/forum?id=ZK1CZXKgG5)] \[[code](https://github.com/XiaokunFeng/MemVLT) ⭐ 19 | 🐛 2 | 📅 2024-10-07]
* **CPDTrack** (Beyond Accuracy: Tracking More Like Human via Visual Search) \[[paper\&review](https://openreview.net/forum?id=LezAEImfoc)] \[[code](https://github.com/ZhangDailing8/CPDTrack) ⭐ 18 | 🐛 1 | 🌐 Python | 📅 2026-02-08]
* **ChatTracker** (ChatTracker: Enhancing Visual Tracking Performance via Chatting with Multimodal Large Language Model) \[[paper\&review](https://openreview.net/forum?id=HzANl2unCB)] \[~~code~~]
* **DeTrack** (DeTrack: In-model Latent Denoising Learning for Visual Object Tracking) \[[paper\&review](https://openreview.net/forum?id=ZJjuNF0olj)] \[~~code~~]

### ECCV 2024

* **LoRAT** (Tracking Meets LoRA: Faster Training, Larger Model, Stronger Performance) \[[paper](https://arxiv.org/abs/2403.05231)] \[[code](https://github.com/LitingLin/LoRAT) ⭐ 126 | 🐛 19 | 🌐 Python | 📅 2026-02-06]
* **Diff-Tracker** (Diff-Tracker: Text-to-Image Diffusion Models are Unsupervised Trackers) \[[paper](https://arxiv.org/abs/2407.08394)] \[~~code~~]

### ICML 2024

* **AVTrack** (Learning Adaptive and View-Invariant Vision Transformer for Real-Time UAV Tracking) \[[paper](https://openreview.net/forum?id=eaNLvrP8n1)] \[[code](https://github.com/wuyou3474/AVTrack) ⭐ 114 | 🐛 11 | 🌐 Python | 📅 2025-08-19]

### AAAI 2024

* **ODTrack** (ODTrack: Online Dense Temporal Token Learning for Visual Tracking) \[[paper](https://arxiv.org/abs/2401.01686)] \[[code](https://github.com/GXNU-ZhongLab/ODTrack) ⭐ 192 | 🐛 11 | 🌐 Python | 📅 2024-10-07]
* **BAT** (Bi-Directional Adapter for Multi-Modal Tracking) \[[paper](https://arxiv.org/abs/2312.10611)] \[[code](https://github.com/SparkTempest/BAT) ⭐ 102 | 🐛 11 | 🌐 Python | 📅 2024-03-19]
* **UVLTrack** (Unifying Visual and Vision-Language Tracking via Contrastive Learning) \[[paper](https://arxiv.org/abs/2401.11228)] \[[code](https://github.com/OpenSpaceAI/UVLTrack) ⭐ 51 | 🐛 4 | 🌐 Python | 📅 2024-11-04]
* **EVPTrack** (Explicit Visual Prompts for Visual Object Tracking) \[[paper](https://arxiv.org/abs/2401.03142)] \[[code](https://github.com/GXNU-ZhongLab/EVPTrack) ⭐ 30 | 🐛 2 | 🌐 Python | 📅 2024-04-03]
* **STCFormer** (Sequential Fusion Based Multi-Granularity Consistency for Space-Time Transformer Tracking) \[[paper](https://ojs.aaai.org/index.php/AAAI/article/view/29145)] \[~~code~~]
* **TATrack** (Temporal Adaptive RGBT Tracking with Modality Prompt) \[[paper](https://arxiv.org/abs/2401.01244)] \[~~code~~]

### IJCAI 2024

* **USTrack** (Unified Single-Stage Transformer Network for Efficient RGB-T Tracking) \[[paper](https://arxiv.org/abs/2308.13764)] \[[code](https://github.com/xiajianqiang/USTrack) ⭐ 11 | 🐛 6 | 📅 2024-09-24]
* **DMTrack** (Diffusion Mask-Driven Visual-language Tracking) \[[paper](https://www.ijcai.org/proceedings/2024/183)] \[~~code~~]

### MM 2024

* **CKD** (Breaking Modality Gap in RGBT Tracking: Coupled Knowledge Distillation) \[[paper\&review](https://openreview.net/forum?id=2jzyYyRqX0)] \[[code](https://github.com/Multi-Modality-Tracking/CKD) ⭐ 23 | 🐛 1 | 🌐 Python | 📅 2024-10-16]
* **ATTracker** (Consistencies are All You Need for Semi-Supervised Vision-Language Tracking) \[[paper\&review](https://openreview.net/forum?id=jLJ3htNxVX)] \[~~code~~]

### WACV 2024

* **TaMOs** (Beyond SOT: It's Time to Track Multiple Generic Objects at Once) \[[paper](https://arxiv.org/abs/2212.11920)] \[[code](https://github.com/visionml/pytracking) ⭐ 3,514 | 🐛 82 | 🌐 Python | 📅 2024-08-08]
* **SMAT** (Separable Self and Mixed Attention Transformers for Efficient Object Tracking) \[[paper](https://arxiv.org/abs/2309.03979)] \[[code](https://github.com/goutamyg/SMAT) ⭐ 49 | 🐛 13 | 🌐 Python | 📅 2024-05-02]

### ICRA 2024

* **DCPT** (DCPT: Darkness Clue-Prompted Tracking in Nighttime UAVs) \[[paper](https://arxiv.org/abs/2309.10491)] \[[code](https://github.com/bearyi26/DCPT) ⭐ 31 | 🐛 7 | 🌐 Python | 📅 2024-03-20]

### IROS 2024

* **PRL-Track** (Progressive Representation Learning for Real-Time UAV Tracking) \[[paper](https://arxiv.org/abs/2409.16652)] \[[code](https://github.com/vision4robotics/PRL-Track) ⭐ 53 | 🐛 1 | 🌐 Python | 📅 2024-09-29]
* **LDEnhancer** (Enhancing Nighttime UAV Tracking with Light Distribution Suppression) \[[paper](https://arxiv.org/abs/2409.16631)] \[[code](https://github.com/vision4robotics/LDEnhancer) ⭐ 21 | 🐛 5 | 🌐 Python | 📅 2024-12-02]
* **TDA-Track** (TDA-Track: Prompt-Driven Temporal Domain Adaptation for Nighttime UAV Tracking) \[[paper](https://arxiv.org/abs/2409.18533)] \[[code](https://github.com/vision4robotics/TDA-Track) ⭐ 14 | 🐛 1 | 🌐 Python | 📅 2025-03-26]
* **DaDiff** (DaDiff: Domain-Aware Diffusion Model for Nighttime UAV Tracking) \[[paper](https://arxiv.org/abs/2410.12270)] \[[code](https://github.com/vision4robotics/DaDiff) ⭐ 10 | 🐛 1 | 🌐 Python | 📅 2024-03-25]
* **CGDenoiser** (Conditional Generative Denoiser for Nighttime UAV Tracking) \[[paper](https://arxiv.org/abs/2409.16834)] \[[code](https://github.com/vision4robotics/CGDenoiser) ⭐ 8 | 🐛 1 | 🌐 Python | 📅 2024-08-25]

### Preprint 2024

* **SAMURAI** (SAMURAI: Adapting Segment Anything Model for Zero-Shot Visual Tracking with Motion-Aware Memory) \[[paper](https://arxiv.org/abs/2411.11922)] \[[code](https://github.com/yangchris11/samurai) ⭐ 7,113 | 🐛 11 | 🌐 Python | 📅 2025-03-18]
* **AVTrack-MD** (Learning Adaptive and View-Invariant Vision Transformer with Multi-Teacher Knowledge Distillation for Real-Time UAV Tracking) \[[paper](https://arxiv.org/abs/2412.20002)] \[[code](https://github.com/wuyou3474/AVTrack) ⭐ 114 | 🐛 11 | 🌐 Python | 📅 2025-08-19]
* **SeqTrackv2** (Unified Sequence-to-Sequence Learning for Single- and Multi-Modal Visual Object Tracking) \[[paper](https://arxiv.org/abs/2304.14394)] \[[code](https://github.com/chenxin-dlut/SeqTrackv2) ⭐ 97 | 🐛 4 | 🌐 Python | 📅 2024-03-26]
* **PiVOT** (Improving Visual Object Tracking through Visual Prompting) \[[paper](https://arxiv.org/abs/2409.18901)] \[[code](https://github.com/chenshihfang/GOT) ⭐ 45 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-07-13]
* **AMTTrack** (Long-Term Frame-Event Visual Tracking: Benchmark Dataset and Baseline) \[[paper](https://arxiv.org/abs/2403.05839)] \[[code](https://github.com/Event-AHU/FELT_SOT_Benchmark) ⭐ 40 | 🐛 9 | 🌐 Python | 📅 2026-06-13]
* **CSTNet** (Transformer-Based RGB-T Tracking with Channel and Spatial Feature Fusion) \[[paper](https://arxiv.org/abs/2405.03177)] \[[code](https://github.com/LiYunfengLYF/CSTNet) ⭐ 29 | 🐛 7 | 🌐 Python | 📅 2024-07-24]
* **BofN** (Predicting the Best of N Visual Trackers) \[[paper](https://arxiv.org/abs/2407.15707)] \[[code](https://github.com/BasitAlawode/Best_of_N_Trackers) ⭐ 25 | 🐛 0 | 🌐 Python | 📅 2024-12-23]
* **CRSOT** (CRSOT: Cross-Resolution Object Tracking using Unaligned Frame and Event Cameras) \[[paper](https://arxiv.org/abs/2401.02826)] \[[code](https://github.com/Event-AHU/Cross_Resolution_SOT) ⭐ 22 | 🐛 1 | 📅 2025-01-18]
* **AFter** (AFter: Attention-Based Fusion Router for RGBT Tracking) \[[paper](https://arxiv.org/abs/2405.02717)] \[[code](https://github.com/Alexadlu/AFter) ⭐ 17 | 🐛 7 | 🌐 Python | 📅 2025-07-08]
* **SuperSBT** (Correlation-Embedded Transformer Tracking: A Single-Branch Framework) \[[paper](https://arxiv.org/abs/2401.12743)] \[[code](https://github.com/phiphiphi31/SBT) ⭐ 15 | 🐛 5 | 🌐 Python | 📅 2024-11-23]
* **LoReTrack** (LoReTrack: Efficient and Accurate Low-Resolution Transformer Tracking) \[[paper](https://arxiv.org/abs/2405.17660)] \[[code](https://github.com/ShaohuaDong2021/LoReTrack) ⭐ 10 | 🐛 1 | 🌐 Python | 📅 2025-07-13]
* **SCANet** (RGB-Sonar Tracking Benchmark and Spatial Cross-Attention Transformer Tracker) \[[paper](https://arxiv.org/abs/2406.07189)] \[[code](https://github.com/LiYunfengLYF/SCANet) ⭐ 10 | 🐛 8 | 🌐 Python | 📅 2025-06-07]
* **OIFTrack** (Optimized Information Flow for Transformer Tracking) \[[paper](https://arxiv.org/abs/2402.08195)] \[[code](https://github.com/JananiKugaa/OIFTrack) ⭐ 7 | 🐛 1 | 🌐 Python | 📅 2024-09-15]
* **TENet** (TENet: Targetness Entanglement Incorporating with Multi-Scale Pooling and Mutually-Guided Fusion for RGB-E Object Tracking) \[[paper](https://arxiv.org/abs/2405.05004)] \[[code](https://github.com/SSSpc333/TENet) ⭐ 7 | 🐛 0 | 📅 2024-12-31]
* **HiPTrack-MLS** (Camouflaged Object Tracking: A Benchmark) \[[paper](https://arxiv.org/abs/2408.13877)] \[[code](https://github.com/openat25/HIPTrack-MLS) ⭐ 6 | 🐛 1 | 🌐 Python | 📅 2025-05-27]
* **NLMTrack** (Enhancing Thermal Infrared Tracking with Natural Language Modeling and Coordinate Sequence Generation) \[[paper](https://arxiv.org/abs/2407.08265)] \[[code](https://github.com/ELOESZHANG/NLMTrack) ⭐ 2 | 🐛 1 | 🌐 Python | 📅 2024-07-26]
* **ABTrack** (Adaptively Bypassing Vision Transformer Blocks for Efficient Visual Tracking) \[[paper](https://arxiv.org/abs/2406.08037)] \[[code](https://github.com/1HykhqV3rU/ABTrack)]
* **ACTrack** (ACTrack: Adding Spatio-Temporal Condition for Visual Object Tracking) \[[paper](https://arxiv.org/abs/2403.07914)] \[~~code~~]
* **CAFormer** (Cross-modulated Attention Transformer for RGBT Tracking) \[[paper](https://arxiv.org/abs/2408.02222)] \[~~code~~]
* **CFBT** (Cross Fusion RGB-T Tracking with Bi-Directional Adapter) \[[paper](https://arxiv.org/abs/2408.16979)] \[~~code~~]
* **DT-Training** (Closed-Loop Scaling Up for Visual Object Tracking) \[[paper\&review](https://openreview.net/forum?id=YcUtOIzIXK)] \[~~code~~]
* **DyTrack** (Exploring Dynamic Transformer for Efficient Object Tracking) \[[paper](https://arxiv.org/abs/2403.17651)] \[~~code~~]
* **eMoE-Tracker** (eMoE-Tracker: Environmental MoE-Based Transformer for Robust Event-Guided Object Tracking) \[[paper](https://arxiv.org/abs/2406.20024)] \[~~code~~]
* **ESAT** (Enhanced Semantic Alignment in Transformer Tracking via Position Learning and Force-Directed Attention) \[[paper\&review](https://openreview.net/forum?id=rsJaUHCZIv)] \[~~code~~]
* **HCTrack** (Hybrid Contrastive Transformer for Visual Tracking) \[[paper\&review](https://openreview.net/forum?id=FV5nsugDY1)] \[~~code~~]
* **MAPNet** (Multi-Attention Associate Prediction Network for Visual Tracking) \[[paper](https://arxiv.org/abs/2403.16395)] \[~~code~~]
* **MDETrack** (Enhanced Object Tracking by Self-Supervised Auxiliary Depth Estimation Learning) \[[paper](https://arxiv.org/abs/2405.14195)] \[~~code~~]
* **MMMP** (From Two Stream to One Stream: Efficient RGB-T Tracking via Mutual Prompt Learning and Knowledge Distillation) \[[paper](https://arxiv.org/abs/2403.16834)] \[~~code~~]
* **MST** (Learning Effective Multi-Modal Trackers via Modality-Sensitive Tuning) \[[paper\&review](https://openreview.net/forum?id=dKZCfzRlm3)] \[~~code~~]
* **M3PT** (Middle Fusion and Multi-Stage, Multi-Form Prompts for Robust RGB-T Tracking) \[[paper](https://arxiv.org/abs/2403.18193)] \[~~code~~]
* **PDAT** (Progressive Domain Adaptation for Thermal Infrared Object Tracking) \[[paper](https://arxiv.org/abs/2407.19430)] \[~~code~~]
* **PromptTrack** (Streaming Spatial-Temporal Prompt Learning for RGB-T Tracking) \[[paper\&review](https://openreview.net/forum?id=S1GTzTFKxb)] \[~~code~~]
* **SPDAN** (BihoT: A Large-Scale Dataset and Benchmark for Hyperspectral Camouflaged Object Tracking) \[[paper](https://arxiv.org/abs/2408.12232)] \[~~code~~]
* **STMT** (Transformer RGBT Tracking with Spatio-Temporal Multimodal Tokens) \[[paper](https://arxiv.org/abs/2401.01674)] \[~~code~~]
* **TrackMamba** (TrackMamba: Mamba-Transformer Tracking) \[[paper\&review](https://openreview.net/forum?id=V7QRVEZ0le)] \[~~code~~]

### CVPR 2023

* **SeqTrack** (SeqTrack: Sequence to Sequence Learning for Visual Object Tracking) \[[paper](https://arxiv.org/abs/2304.14394)] \[[code](https://github.com/microsoft/VideoX/tree/master/SeqTrack) ⭐ 1,071 | 🐛 31 | 🌐 Python | 📅 2024-06-03]
* **ViPT** (Visual Prompt Multi-Modal Tracking) \[[paper](https://arxiv.org/abs/2303.10826)] \[[code](https://github.com/jiawen-zhu/ViPT) ⭐ 351 | 🐛 12 | 🌐 Python | 📅 2025-03-04]
* **ARTrack** (Autoregressive Visual Tracking) \[[paper](https://openaccess.thecvf.com/content/CVPR2023/html/Wei_Autoregressive_Visual_Tracking_CVPR_2023_paper.html)] \[[code](https://github.com/MIV-XJTU/ARTrack) ⭐ 320 | 🐛 9 | 🌐 Python | 📅 2025-10-20]
* **SwinV2** (Revealing the Dark Secrets of Masked Image Modeling) \[[paper](https://arxiv.org/abs/2205.13543)] \[[code](https://github.com/SwinTransformer/MIM-Depth-Estimation) ⭐ 176 | 🐛 6 | 🌐 Python | 📅 2023-03-27]
* **GRM** (Generalized Relation Modeling for Transformer Tracking) \[[paper](https://arxiv.org/abs/2303.16580)] \[[code](https://github.com/Little-Podi/GRM) ⭐ 87 | 🐛 1 | 🌐 Python | 📅 2023-12-30]
* **JointNLT** (Joint Visual Grounding and Tracking with Natural Language Specification) \[[paper](https://arxiv.org/abs/2303.12027)] \[[code](https://github.com/lizhou-cs/JointNLT) ⭐ 77 | 🐛 10 | 🌐 Python | 📅 2023-06-03]
* **TBSI** (Bridging Search Region Interaction with Template for RGB-T Tracking) \[[paper](https://openaccess.thecvf.com/content/CVPR2023/html/Hui_Bridging_Search_Region_Interaction_With_Template_for_RGB-T_Tracking_CVPR_2023_paper.html)] \[[code](https://github.com/RyanHTR/TBSI) ⭐ 70 | 🐛 12 | 🌐 Python | 📅 2023-11-10]
* **ART** (ARKitTrack: A New Diverse Dataset for Tracking Using Mobile RGB-D Data) \[[paper](https://arxiv.org/abs/2303.13885)] \[[code](https://github.com/lawrence-cj/ARKitTrack) ⭐ 48 | 🐛 3 | 🌐 Python | 📅 2023-06-15]
* **DropTrack** (DropMAE: Masked Autoencoders with Spatial-Attention Dropout for Tracking Tasks) \[[paper](https://arxiv.org/abs/2304.00571)] \[[code](https://github.com/jimmy-dq/DropTrack) ⭐ 42 | 🐛 0 | 🌐 Python | 📅 2023-07-01]
* **MAT** (Representation Learning for Visual Object Tracking by Masked Appearance Transfer) \[[paper](https://openaccess.thecvf.com/content/CVPR2023/html/Zhao_Representation_Learning_for_Visual_Object_Tracking_by_Masked_Appearance_Transfer_CVPR_2023_paper.html)] \[[code](https://github.com/difhnp/MAT) ⭐ 18 | 🐛 5 | 🌐 Python | 📅 2023-06-10]
* **VideoTrack** (VideoTrack: Learning to Track Objects via Video Transformer) \[[paper](https://openaccess.thecvf.com/content/CVPR2023/html/Xie_VideoTrack_Learning_To_Track_Objects_via_Video_Transformer_CVPR_2023_paper.html)] \[[code](https://github.com/phiphiphi31/VideoTrack) ⭐ 13 | 🐛 5 | 📅 2023-06-26]
* **EMT** (Resource-Efficient RGBD Aerial Tracking) \[[paper](https://openaccess.thecvf.com/content/CVPR2023/html/Yang_Resource-Efficient_RGBD_Aerial_Tracking_CVPR_2023_paper.html)] \[[code](https://github.com/yjybuaa/RGBDAerialTracking) ⭐ 10 | 🐛 1 | 📅 2023-05-23]

### NeurIPS 2023

* **MixFormerV2** (MixFormerV2: Efficient Fully Transformer Tracking) \[[paper\&review](https://openreview.net/forum?id=8WvYAycmDJ)] \[[code](https://github.com/MCG-NJU/MixFormerV2) ⭐ 227 | 🐛 35 | 🌐 Python | 📅 2024-04-20]
* **ZoomTrack** (ZoomTrack: Target-Aware Non-Uniform Resizing for Efficient Visual Tracking) \[[paper\&review](https://openreview.net/forum?id=DQgTewaKzt)] \[[code](https://github.com/Kou-99/ZoomTrack) ⭐ 19 | 🐛 1 | 🌐 Python | 📅 2024-03-04]
* **RFGM** (Reading Relevant Feature from Global Representation Memory for Visual Object Tracking) \[[paper\&review](https://openreview.net/forum?id=On0IDMYKw2)] \[~~code~~]

### ICCV 2023

* **HRTrack** (Cross-Modal Orthogonal High-Rank Augmentation for RGB-Event Transformer-Trackers) \[[paper](https://arxiv.org/abs/2307.04129)] \[[code](https://github.com/ZHU-Zhiyu/High-Rank_RGB-Event_Tracker) ⭐ 150 | 🐛 2 | 🌐 Python | 📅 2024-08-06]
* **HiT** (Exploring Lightweight Hierarchical Vision Transformers for Efficient Visual Tracking) \[[paper](https://arxiv.org/abs/2308.06904)] \[[code](https://github.com/kangben258/HiT) ⭐ 60 | 🐛 4 | 🌐 Python | 📅 2025-09-25]
* **AiATrack-360** (360VOT: A New Benchmark Dataset for Omnidirectional Visual Object Tracking) \[[paper](https://arxiv.org/abs/2307.14630)] \[[code](https://github.com/HuajianUP/360VOT) ⭐ 55 | 🐛 1 | 🌐 Python | 📅 2026-01-16]
* **Aba-ViTrack** (Adaptive and Background-Aware Vision Transformer for Real-Time UAV Tracking) \[[paper](https://openaccess.thecvf.com/content/ICCV2023/html/Li_Adaptive_and_Background-Aware_Vision_Transformer_for_Real-Time_UAV_Tracking_ICCV_2023_paper.html)] \[[code](https://github.com/xyyang317/Aba-ViTrack) ⭐ 51 | 🐛 7 | 🌐 Python | 📅 2025-12-17]
* **CiteTracker** (CiteTracker: Correlating Image and Text for Visual Tracking) \[[paper](https://arxiv.org/abs/2308.11322)] \[[code](https://github.com/NorahGreen/CiteTracker) ⭐ 49 | 🐛 9 | 🌐 Python | 📅 2024-06-20]
* **ROMTrack** (Robust Object Modeling for Visual Tracking) \[[paper](https://arxiv.org/abs/2308.05140)] \[[code](https://github.com/dawnyc/ROMTrack) ⭐ 49 | 🐛 5 | 🌐 Python | 📅 2025-01-05]
* **DecoupleTNL** (Tracking by Natural Language Specification with Long Short-Term Context Decoupling) \[[paper](https://openaccess.thecvf.com/content/ICCV2023/html/Ma_Tracking_by_Natural_Language_Specification_with_Long_Short-term_Context_Decoupling_ICCV_2023_paper.html)] \[~~code~~]
* **F-BDMTrack** (Foreground-Background Distribution Modeling Transformer for Visual Object Tracking) \[[paper](https://openaccess.thecvf.com/content/ICCV2023/html/Yang_Foreground-Background_Distribution_Modeling_Transformer_for_Visual_Object_Tracking_ICCV_2023_paper.html)] \[~~code~~]

### AAAI 2023

* **TATrack** (Target-Aware Tracking with Long-Term Context Attention) \[[paper](https://arxiv.org/abs/2302.13840)] \[[code](https://github.com/hekaijie123/TATrack) ⭐ 52 | 🐛 4 | 🌐 Python | 📅 2023-03-13]
* **CTTrack** (Compact Transformer Tracker with Correlative Masked Modeling) \[[paper](https://arxiv.org/abs/2301.10938)] \[[code](https://github.com/HUSTDML/CTTrack) ⭐ 43 | 🐛 14 | 🌐 Python | 📅 2024-07-23]
* **GdaTFT** (Global Dilated Attention and Target Focusing Network for Robust Tracking) \[[paper](https://ojs.aaai.org/index.php/AAAI/article/view/25241)] \[~~code~~]

### MM 2023

* **All-in-One** (All in One: Exploring Unified Vision-Language Tracking with Multi-Modal Alignment) \[[paper](https://arxiv.org/abs/2307.03373)] \[~~code~~]
* **UTrack** (Unambiguous Object Tracking by Exploiting Target Cues) \[[paper](https://dl.acm.org/doi/10.1145/3581783.3612240)] \[~~code~~]

### MMAsia 2023

* **UPVPT** (Robust Tracking via Unifying Pretrain-Finetuning and Visual Prompt Tuning) \[[paper](https://dl.acm.org/doi/abs/10.1145/3595916.3626410)] \[~~code~~]

### MICCAI 2023

* **ConTrack** (ConTrack: Contextual Transformer for Device Tracking in X-ray) \[[paper](https://arxiv.org/abs/2307.07541)] \[~~code~~]

### WACV 2023

* **E.T.Track** (Efficient Visual Tracking with Exemplar Transformers) \[[paper](https://arxiv.org/abs/2112.09686)] \[[code](https://github.com/pblatter/ettrack) ⭐ 100 | 🐛 9 | 🌐 Python | 📅 2024-03-25]

### BMVC 2023

* **MVT** (Mobile Vision Transformer-Based Visual Object Tracking) \[[paper](https://arxiv.org/abs/2309.05829)] \[[code](https://github.com/goutamyg/MVT) ⭐ 28 | 🐛 7 | 🌐 Python | 📅 2024-04-23]

### ICRA 2023

* **SGDViT** (SGDViT: Saliency-Guided Dynamic vision Transformer for UAV tracking) \[[paper](https://arxiv.org/abs/2303.04378)] \[[code](https://github.com/vision4robotics/SGDViT) ⭐ 18 | 🐛 3 | 🌐 Python | 📅 2023-04-03]
* **ClimRT** (Continuity-Aware Latent Interframe Information Mining for Reliable UAV Tracking) \[[paper](https://arxiv.org/abs/2303.04525)] \[[code](https://github.com/vision4robotics/ClimRT) ⭐ 10 | 🐛 0 | 🌐 Python | 📅 2022-09-20]

### IROS 2023

* **CDT** (Cascaded Denoising Transformer for UAV Nighttime Tracking) \[[paper](https://ieeexplore.ieee.org/document/10093049)] \[[code](https://github.com/vision4robotics/CDT) ⭐ 12 | 🐛 1 | 🌐 Python | 📅 2024-03-24]
* **FDNT** (End-to-End Feature Decontaminated Network for UAV Tracking) \[[paper](https://ieeexplore.ieee.org/document/9981882)] \[[code](https://github.com/vision4robotics/FDNT) ⭐ 11 | 🐛 0 | 🌐 Python | 📅 2022-11-07]
* **TRTrack** (Boosting UAV Tracking With Voxel-Based Trajectory-Aware Pre-Training) \[[paper](https://ieeexplore.ieee.org/document/10015867)] \[[code](https://github.com/vision4robotics/TRTrack) ⭐ 5 | 🐛 1 | 📅 2022-11-15]
* **ScaleAwareDA** (Scale-Aware Domain Adaptation for Robust UAV Tracking) \[[paper](https://ieeexplore.ieee.org/document/10111056)] \[[code](https://github.com/vision4robotics/ScaleAwareDA) ⭐ 4 | 🐛 1 | 🌐 Python | 📅 2022-10-22]
* **TOTEM** (Transparent Object Tracking with Enhanced Fusion Module) \[[paper](https://arxiv.org/abs/2309.06701)] \[[code](https://github.com/kalyan0510/TOTEM) ⭐ 4 | 🐛 0 | 📅 2023-09-11]

### ICASSP 2023

* **ProContEXT** (ProContEXT: Exploring Progressive Context Transformer for Tracking) \[[paper](https://arxiv.org/abs/2210.15511)] \[[code](https://github.com/jp-lan/ProContEXT) ⭐ 17 | 🐛 0 | 🌐 Python | 📅 2023-08-18]
* **MSTL** (Multi-Source Templates Learning for Real-Time Aerial Tracking) \[[paper](https://ieeexplore.ieee.org/document/10094642)] \[[code](https://github.com/vpx-ecnu/MSTL) ⭐ 5 | 🐛 3 | 🌐 Python | 📅 2023-05-30]

### Preprint 2023

* **MixViT** (MixFormer: End-to-End Tracking with Iterative Mixed Attention) \[[paper](https://arxiv.org/abs/2302.02814)] \[[code](https://github.com/MCG-NJU/MixFormer) ⭐ 539 | 🐛 44 | 🌐 Python | 📅 2024-02-28]
* **TCTrack++** (Towards Real-World Visual Tracking with Temporal Contexts) \[[paper](https://arxiv.org/abs/2308.10330)] \[[code](https://github.com/vision4robotics/TCTrack) ⭐ 205 | 🐛 9 | 🌐 Python | 📅 2023-08-29]
* **LiteTrack** (LiteTrack: Layer Pruning with Asynchronous Feature Extraction for Lightweight and Efficient Visual Tracking) \[[paper](https://arxiv.org/abs/2309.09249)] \[[code](https://github.com/TsingWei/LiteTrack) ⭐ 90 | 🐛 22 | 🌐 Python | 📅 2025-01-20]
* **SAM-DA** (SAM-DA: UAV Tracks Anything at Night with SAM-Powered Domain Adaptation) \[[paper](https://arxiv.org/abs/2307.01024)] \[[code](https://github.com/vision4robotics/SAM-DA) ⭐ 62 | 🐛 3 | 🌐 Jupyter Notebook | 📅 2024-09-27]
* **MPLT** (RGB-T Tracking via Multi-Modal Mutual Prompt Learning) \[[paper](https://arxiv.org/abs/2308.16386)] \[[code](https://github.com/HusterYoung/MPLT) ⭐ 29 | 🐛 4 | 🌐 Python | 📅 2023-10-27]
* **MMTrack** (Towards Unified Token Learning for Vision-Language Tracking) \[[paper](https://arxiv.org/abs/2308.14103)] \[[code](https://github.com/Azong-HQU/MMTrack) ⭐ 24 | 🐛 4 | 🌐 Python | 📅 2023-12-13]
* **HyperTrack** (HyperTrack: A Unified Framework for Hyperspectral Object Tracking) \[[paper](https://arxiv.org/abs/2308.07016)] \[[code](https://github.com/supertyd/HyperTrack) ⭐ 12 | 🐛 3 | 🌐 Python | 📅 2025-12-01]
* **AViTMP** (Exploiting Image-Related Inductive Biases in Single-Branch Visual Tracking) \[[paper](https://arxiv.org/abs/2310.19542)] \[~~code~~]
* **DATr** (Leveraging the Power of Data Augmentation for Transformer-Based Tracking) \[[paper](https://arxiv.org/abs/2309.08264)] \[~~code~~]
* **DETRack** (Efficient Training for Visual Tracking with Deformable Transformer) \[[paper](https://arxiv.org/abs/2309.02676)] \[~~code~~]
* **IPL** (Modality-Missing RGBT Tracking via Invertible Prompt Learning and A High-Quality Data Simulation Method) \[[paper](https://arxiv.org/abs/2312.16244)] \[~~code~~]
* **JN** (Towards Efficient Training with Negative Samples in Visual Tracking) \[[paper](https://arxiv.org/abs/2309.02903)] \[~~code~~]
* **MACFT** (RGB-T Tracking Based on Mixed Attention) \[[paper](https://arxiv.org/abs/2304.04264)] \[~~code~~]
* **ProFormer** (RGBT Tracking via Progressive Fusion Transformer with Dynamically Guided Learning) \[[paper](https://arxiv.org/abs/2303.14778)] \[~~code~~]
* **RTrack** (RTrack: Accelerating Convergence for Visual Object Tracking via Pseudo-Boxes Exploration) \[[paper](https://arxiv.org/abs/2309.13257)] \[~~code~~]
* **SATracker** (Beyond Visual Cues: Synchronously Exploring Target-Centric Semantics for Vision-Language Tracking) \[[paper](https://arxiv.org/abs/2311.17085)] \[~~code~~]
* **USTAM** (USTAM: Unified Spatial-Temporal Attention MixFormer for Visual Object Tracking) \[[paper\&review](https://openreview.net/forum?id=MK7TEe7SJ3)] \[~~code~~]

### CVPR 2022

* **ToMP** (Transforming Model Prediction for Tracking) \[[paper](https://arxiv.org/abs/2203.11192)] \[[code](https://github.com/visionml/pytracking) ⭐ 3,514 | 🐛 82 | 🌐 Python | 📅 2024-08-08]
* **MixFormer** (MixFormer: End-to-End Tracking with Iterative Mixed Attention) \[[paper](https://arxiv.org/abs/2203.11082)] \[[code](https://github.com/MCG-NJU/MixFormer) ⭐ 539 | 🐛 44 | 🌐 Python | 📅 2024-02-28]
* **TCTrack** (TCTrack: Temporal Contexts for Aerial Tracking) \[[paper](https://arxiv.org/abs/2203.01885)] \[[code](https://github.com/vision4robotics/TCTrack) ⭐ 205 | 🐛 9 | 🌐 Python | 📅 2023-08-29]
* **UDAT** (Unsupervised Domain Adaptation for Nighttime Aerial Tracking) \[[paper](https://arxiv.org/abs/2203.10541)] \[[code](https://github.com/vision4robotics/UDAT) ⭐ 126 | 🐛 3 | 🌐 Python | 📅 2023-10-23]
* **STNet** (Spiking Transformers for Event-Based Single Object Tracking) \[[paper](https://openaccess.thecvf.com/content/CVPR2022/html/Zhang_Spiking_Transformers_for_Event-Based_Single_Object_Tracking_CVPR_2022_paper.html)] \[[code](https://github.com/Jee-King/CVPR2022_STNet) ⭐ 99 | 🐛 14 | 🌐 Python | 📅 2022-03-21]
* **CSWinTT** (Transformer Tracking with Cyclic Shifting Window Attention) \[[paper](https://arxiv.org/abs/2205.03806)] \[[code](https://github.com/SkyeSong38/CSWinTT) ⭐ 69 | 🐛 7 | 🌐 Python | 📅 2022-05-10]
* **RBO** (Ranking-Based Siamese Visual Tracking) \[[paper](https://arxiv.org/abs/2205.11761)] \[[code](https://github.com/sansanfree/RBO) ⭐ 36 | 🐛 13 | 🌐 Python | 📅 2023-07-13]
* **SBT** (Correlation-Aware Deep Tracking) \[[paper](https://arxiv.org/abs/2203.01666)] \[[code](https://github.com/phiphiphi31/SBT) ⭐ 15 | 🐛 5 | 🌐 Python | 📅 2024-11-23]
* **GTELT** (Global Tracking via Ensemble of Local Trackers) \[[paper](https://arxiv.org/abs/2203.16092)] \[[code](https://github.com/ZikunZhou/GTELT) ⭐ 11 | 🐛 4 | 📅 2022-03-13]
* **CMTR** (Cross-Modal Target Retrieval for Tracking by Natural Language) \[[paper](https://openaccess.thecvf.com/content/CVPR2022W/ODRUM/html/Li_Cross-Modal_Target_Retrieval_for_Tracking_by_Natural_Language_CVPRW_2022_paper.html)] \[~~code~~]

### NeurIPS 2022

* **SwinTrack** (SwinTrack: A Simple and Strong Baseline for Transformer Tracking) \[[paper\&review](https://openreview.net/forum?id=9h3KsOVXhLZ)] \[[code](https://github.com/LitingLin/SwinTrack) ⭐ 260 | 🐛 29 | 🌐 Python | 📅 2022-10-18]

### ECCV 2022

* **OSTrack** (Joint Feature Learning and Relation Modeling for Tracking: A One-Stream Framework) \[[paper](https://arxiv.org/abs/2203.11991)] \[[code](https://github.com/botaoye/OSTrack) ⭐ 682 | 🐛 54 | 🌐 Python | 📅 2023-08-03]
* **AiATrack** (AiATrack: Attention in Attention for Transformer Visual Tracking) \[[paper](https://arxiv.org/abs/2207.09603)] \[[code](https://github.com/Little-Podi/AiATrack) ⭐ 128 | 🐛 1 | 🌐 Python | 📅 2023-12-30]
* **HCAT** (Efficient Visual Tracking via Hierarchical Cross-Attention Transformer) \[[paper](https://arxiv.org/abs/2203.13537)] \[[code](https://github.com/chenxin-dlut/HCAT) ⭐ 59 | 🐛 2 | 🌐 Python | 📅 2023-06-08]
* **SimTrack** (Backbone is All Your Need: A Simplified Architecture for Visual Object Tracking) \[[paper](https://arxiv.org/abs/2203.05328)] \[[code](https://github.com/LPXTT/SimTrack) ⭐ 53 | 🐛 8 | 🌐 Python | 📅 2022-12-23]
* **CIA** (Hierarchical Feature Embedding for Visual Tracking) \[[paper](https://www.ecva.net/papers/eccv_2022/papers_ECCV/html/4400_ECCV_2022_paper.php)] \[[code](https://github.com/zxgravity/CIA) ⭐ 3 | 🐛 3 | 🌐 Python | 📅 2022-07-19]
* **DMTracker** (Learning Dual-Fused Modality-Aware Representations for RGBD Tracking) \[[paper](https://arxiv.org/abs/2211.03055)] \[[code](https://github.com/CV-Tracking/DMTracker) ⭐ 2 | 🐛 0 | 📅 2022-08-19]
* **VOT2022** (The Tenth Visual Object Tracking VOT2022 Challenge Results) \[[paper](https://prints.vicos.si/publications/416/the-tenth-visual-object-tracking-vot2022-challenge-results)] \[[code](https://www.votchallenge.net/vot2022/trackers.html)]

### AAAI 2022

* **APFNet** (Attribute-Based Progressive Fusion Network for RGBT Tracking) \[[paper](https://aaai-2022.virtualchair.net/poster_aaai7747)] \[[code](https://github.com/yangmengmeng1997/APFNet) ⭐ 45 | 🐛 10 | 📅 2022-05-05]

### IJCAI 2022

* **InMo** (Learning Target-Aware Representation for Visual Tracking via Informative Interactions) \[[paper](https://arxiv.org/abs/2201.02526)] \[[code](https://github.com/JudasDie/SOTS) ⭐ 518 | 🐛 38 | 🌐 Python | 📅 2026-04-14]
* **SparseTT** (SparseTT: Visual Tracking with Sparse Transformers) \[[paper](https://arxiv.org/abs/2205.03776)] \[[code](https://github.com/fzh0917/SparseTT) ⭐ 59 | 🐛 9 | 🌐 Python | 📅 2022-05-21]

### MICCAI 2022

* **TLT** (Transformer Lesion Tracker) \[[paper](https://arxiv.org/abs/2206.06252)] \[[code](https://github.com/TangWen920812/TLT) ⭐ 4 | 🐛 3 | 🌐 Python | 📅 2022-09-23]

### WACV 2022

* **SiamTPN** (Siamese Transformer Pyramid Networks for Real-Time UAV Tracking) \[[paper](https://arxiv.org/abs/2110.08822)] \[[code](https://github.com/RISC-NYUAD/SiamTPNTracker) ⭐ 51 | 🐛 4 | 🌐 Python | 📅 2024-02-20]

### ICRA 2022

* **SCT** (Tracker Meets Night: A Transformer Enhancer for UAV Tracking) \[[paper](https://ieeexplore.ieee.org/document/9696362)] \[[code](https://github.com/vision4robotics/SCT) ⭐ 60 | 🐛 4 | 🌐 Python | 📅 2023-06-16]

### ACCV 2022

* **TAT** (Temporal-Aware Siamese Tracker: Integrate Temporal Context for 3D Object Tracking) \[[paper](https://openaccess.thecvf.com/content/ACCV2022/html/Lan_Temporal-aware_Siamese_Tracker_Integrate_Temporal_Context_for_3D_Object_Tracking_ACCV_2022_paper.html)] \[[code](https://github.com/tqsdyy/TAT) ⭐ 1 | 🐛 0 | 📅 2022-11-24]

### IROS 2022

* **SiamSA** (Siamese Object Tracking for Vision-Based UAM Approaching with Pairwise Scale-Channel Attention) \[[paper](https://arxiv.org/abs/2211.14564)] \[[code](https://github.com/vision4robotics/SiamSA) ⭐ 25 | 🐛 1 | 🌐 Python | 📅 2022-12-15]
* **HighlightNet** (HighlightNet: Highlighting Low-Light Potential Features for Real-Time UAV Tracking) \[[paper](https://arxiv.org/abs/2208.06818)] \[[code](https://github.com/vision4robotics/HighlightNet) ⭐ 18 | 🐛 1 | 🌐 Python | 📅 2022-03-14]
* **LPAT** (Local Perception-Aware Transformer for Aerial Tracking) \[[paper](https://arxiv.org/abs/2208.00662)] \[[code](https://github.com/vision4robotics/LPAT) ⭐ 6 | 🐛 1 | 🌐 Python | 📅 2022-08-23]

### Preprint 2022

* **CEUTrack** (Revisiting Color-Event Based Tracking: A Unified Network, Dataset, and Metric) \[[paper](https://arxiv.org/abs/2211.11010)] \[[code](https://github.com/Event-AHU/COESOT/tree/main/CEUTrack) ⭐ 82 | 🐛 7 | 🌐 Python | 📅 2025-11-05]
* **SPT** (RGBD1K: A Large-scale Dataset and Benchmark for RGB-D Object Tracking) \[[paper](https://arxiv.org/abs/2208.09787)] \[[code](https://github.com/xuefeng-zhu5/RGBD1K) ⭐ 21 | 🐛 0 | 📅 2025-12-10]
* **SFTransT** (Learning Spatial-Frequency Transformer for Visual Object Tracking) \[[paper](https://arxiv.org/abs/2208.08829)] \[[code](https://github.com/Tchuanm/SFTransT) ⭐ 20 | 🐛 1 | 🌐 Python | 📅 2023-06-29]
* **FDT** (Feature-Distilled Transformer for UAV Tracking) \[~~paper~~] \[[code](https://github.com/vision4robotics/FDT-tracker) ⭐ 8 | 🐛 1 | 🌐 Python | 📅 2022-03-19]
* **RAMAVT** (On Deep Recurrent Reinforcement Learning for Active Visual Tracking of Space Noncooperative Objects) \[[paper](https://arxiv.org/abs/2212.14304)] \[[code](https://github.com/Dongzhou-1996/RAMAVT) ⭐ 5 | 🐛 0 | 🌐 Python | 📅 2022-11-02]
* **SiamLA** (Learning Localization-Aware Target Confidence for Siamese Visual Tracking) \[[paper](https://arxiv.org/abs/2204.14093)] \[~~code~~]

### CVPR 2021

* **TransT** (Transformer Tracking) \[[paper](https://arxiv.org/abs/2103.15436)] \[[code](https://github.com/chenxin-dlut/TransT) ⭐ 635 | 🐛 60 | 🌐 Python | 📅 2023-07-01]
* **TMT** (Transformer Meets Tracker: Exploiting Temporal Context for Robust Visual Tracking) \[[paper](https://arxiv.org/abs/2103.11681)] \[[code](https://github.com/594422814/TransformerTrack) ⭐ 262 | 🐛 18 | 🌐 Python | 📅 2021-05-24]
* **SiamGAT** (Graph Attention Tracking) \[[paper](https://arxiv.org/abs/2011.11204)] \[[code](https://github.com/ohhhyeahhh/SiamGAT) ⭐ 151 | 🐛 30 | 🌐 Python | 📅 2022-09-04]
* **STMTrack** (STMTrack: Template-Free Visual Tracking with Space-Time Memory Networks) \[[paper](https://arxiv.org/abs/2104.00324)] \[[code](https://github.com/fzh0917/STMTrack) ⭐ 93 | 🐛 10 | 🌐 Python | 📅 2021-06-24]

### ICCV 2021

* **STARK** (Learning Spatio-Temporal Transformer for Visual Tracking) \[[paper](https://arxiv.org/abs/2103.17154)] \[[code](https://github.com/researchmm/Stark) ⭐ 716 | 🐛 70 | 🌐 Python | 📅 2024-04-13]
* **AutoMatch** (Learn to Match: Automatic Matching Network Design for Visual Tracking) \[[paper](https://arxiv.org/abs/2108.00803)] \[[code](https://github.com/JudasDie/SOTS) ⭐ 518 | 🐛 38 | 🌐 Python | 📅 2026-04-14]
* **HiFT** (HiFT: Hierarchical Feature Transformer for Aerial Tracking) \[[paper](https://arxiv.org/abs/2108.00202)] \[[code](https://github.com/vision4robotics/HiFT) ⭐ 85 | 🐛 4 | 🌐 Python | 📅 2022-10-11]
* **TransT-M** (High-Performance Transformer Tracking) \[[paper](https://arxiv.org/abs/2203.13533)] \[[code](https://github.com/chenxin-dlut/TransT-M) ⭐ 28 | 🐛 4 | 🌐 Python | 📅 2023-03-28]
* **DualTFR** (Learning Tracking Representations via Dual-Branch Fully Transformer Networks) \[[paper](https://arxiv.org/abs/2112.02571)] \[[code](https://github.com/phiphiphi31/DualTFR) ⭐ 18 | 🐛 4 | 📅 2023-06-26]
* **SAMN** (Learning Spatio-Appearance Memory Network for High-Performance Visual Tracking) \[[paper](https://arxiv.org/abs/2009.09669)] \[[code](https://github.com/phiphiphi31/DMB) ⭐ 17 | 🐛 0 | 🌐 Python | 📅 2023-06-26]
* **DTT** (High-Performance Discriminative Tracking with Transformers) \[[paper](https://openaccess.thecvf.com/content/ICCV2021/html/Yu_High-Performance_Discriminative_Tracking_With_Transformers_ICCV_2021_paper.html)] \[[code](https://github.com/tominute/DTT) ⭐ 2 | 🐛 1 | 📅 2021-08-18]
* **VOT2021** (The Ninth Visual Object Tracking VOT2021 Challenge Results) \[[paper](https://prints.vicos.si/publications/400/the-ninth-visual-object-tracking-vot2021-challenge-results)] \[[code](https://www.votchallenge.net/vot2021/trackers.html)]

### BMVC 2021

* **TAPL** (TAPL: Dynamic Part-Based Visual Tracking via Attention-Guided Part Localization) \[[paper](https://arxiv.org/abs/2110.13027)] \[~~code~~]

### Preprint 2021

* **TrTr** (TrTr: Visual Tracking with Transformer) \[[paper](https://arxiv.org/abs/2105.03817)] \[[code](https://github.com/tongtybj/TrTr) ⭐ 83 | 🐛 13 | 🌐 Python | 📅 2021-12-19]
* **TREG** (Target Transformed Regression for Accurate Tracking) \[[paper](https://arxiv.org/abs/2104.00403)] \[[code](https://github.com/MCG-NJU/TREG) ⭐ 21 | 🐛 1 | 🌐 Python | 📅 2021-12-05]

### CVPR 2020

* **SiamAttn** (Deformable Siamese Attention Networks for Visual Object Tracking) \[[paper](https://arxiv.org/abs/2004.06711)] \[[code](https://github.com/msight-tech/research-siamattn) ⭐ 48 | 🐛 8 | 🌐 Python | 📅 2021-03-24]

### ICPR 2020

* **VTT** (VTT: Long-Term Visual Tracking with Transformers) \[[paper](https://pure.qub.ac.uk/en/publications/vtt-long-term-visual-tracking-with-transformers)] \[~~code~~]

## :bookmark:3D Single Object Tracking (3DSOT)

### CVPR 2026

* **ChronoTrack** (Temporally Consistent Long-Term Memory for 3D Single Object Tracking) \[[paper](https://arxiv.org/abs/2604.13789)] \[[code](https://github.com/ujaejoon/ChronoTrack) ⭐ 9 | 🐛 1 | 🌐 Python | 📅 2026-04-29]

### CVPR 2025

* **Mono3DVLT** (Mono3DVLT: Monocular-Video-Based 3D Visual Language Tracking) \[[paper](https://openaccess.thecvf.com/content/CVPR2025/html/Wei_Mono3DVLT_Monocular-Video-Based_3D_Visual_Language_Tracking_CVPR_2025_paper.html)] \[~~code~~]

### MM 2025

* **FocusTrack** (FocusTrack: One-Stage Focus-and-Suppress Framework for 3D Point Cloud Object Tracking) \[[paper](https://arxiv.org/abs/2602.24133)] \[~~code~~]

### Preprint 2025

* **SOTFormer** (SOTFormer: A Minimal Transformer for Unified Object Tracking and Trajectory Prediction) \[[paper](https://arxiv.org/abs/2511.11824)] \[[code](https://github.com/zhongpingDong12/SOTFormer) ⭐ 2 | 🐛 2 | 🌐 Python | 📅 2025-11-24]
* **TrajTrack** (Beyond Frame-Wise Tracking: A Trajectory-Based Paradigm for Efficient Point Cloud Tracking) \[[paper](https://arxiv.org/abs/2509.11453)] \[~~code~~]

### ECCV 2024

* **HVTrack** (3D Single-Object Tracking in Point Clouds with High Temporal Variation) \[[paper](https://arxiv.org/abs/2408.02049)] \[~~code~~]

### ICLR 2024

* **CUTrack** (Towards Category Unification of 3D Single Object Tracking on Point Clouds) \[[paper\&review](https://openreview.net/forum?id=QlqdXrzzD1)] \[[code](https://github.com/Haooozi/CUTrack)]

### AAAI 2024

* **M3SOT** (M3SOT: Multi-Frame, Multi-Field, Multi-Space 3D Single Object Tracking) \[[paper](https://arxiv.org/abs/2312.06117)] \[[code](https://github.com/liujia99/M3SOT) ⭐ 16 | 🐛 3 | 🌐 Python | 📅 2024-04-29]
* **SCVTrack** (Robust 3D Tracking with Quality-Aware Shape Completion) \[[paper](https://arxiv.org/abs/2312.10608)] \[[code](https://github.com/zjwhit/SCVTrack) ⭐ 3 | 🐛 2 | 🌐 Python | 📅 2024-04-01]
* **StreamTrack** (Modeling Continuous Motion for 3D Point Cloud Object Tracking) \[[paper](https://ojs.aaai.org/index.php/AAAI/article/view/28196)] \[~~code~~]

### ICRA 2024

* **SeqTrack3D** (SeqTrack3D: Exploring Sequence Information for Robust 3D Point Cloud Tracking) \[[paper](https://arxiv.org/abs/2402.16249)] \[[code](https://github.com/aron-lin/seqtrack3d) ⭐ 29 | 🐛 1 | 🌐 Python | 📅 2024-04-20]

### Preprint 2024

* **PROT3D** (GSOT3D: Towards Generic 3D Single Object Tracking in the Wild) \[[paper](https://arxiv.org/abs/2412.02129)] \[[code](https://github.com/ailovejinx/GSOT3D) ⭐ 33 | 🐛 0 | 🌐 Python | 📅 2025-11-17]
* **PillarTrack** (PillarTrack: Redesigning Pillar-Based Transformer Network for Single Object Tracking on Point Clouds) \[[paper](https://arxiv.org/abs/2404.07495)] \[[code](https://github.com/StiphyJay/PillarTrack) ⭐ 21 | 🐛 1 | 🌐 Python | 📅 2024-08-21]
* **EasyTrack** (EasyTrack: Efficient and Compact One-Stream 3D Point Clouds Tracker) \[[paper](https://arxiv.org/abs/2404.05960)] \[[code](https://github.com/KnightApple427/Easytrack) ⭐ 1 | 🐛 2 | 📅 2023-11-07]
* **SCtrack** (Space-Correlated Transformer: Jointly Explore the Matching and Motion Clues in 3D Single Object Tracking) \[[paper\&review](https://openreview.net/forum?id=Sl1kRAATbw)] \[~~code~~]

### CVPR 2023

* **CXTrack** (CXTrack: Improving 3D Point Cloud Tracking with Contextual Information) \[[paper](https://arxiv.org/abs/2211.08542)] \[[code](https://github.com/slothfulxtx/cxtrack3d) ⭐ 33 | 🐛 1 | 🌐 Python | 📅 2023-03-09]
* **CorpNet** (Correlation Pyramid Network for 3D Single Object Tracking) \[[paper](https://arxiv.org/abs/2305.09195)] \[~~code~~]

### ICCV 2023

* **MBPTrack** (MBPTrack: Improving 3D Point Cloud Tracking with Memory Networks and Box Priors) \[[paper](https://arxiv.org/abs/2303.05071)] \[[code](https://github.com/slothfulxtx/MBPTrack3D) ⭐ 30 | 🐛 13 | 🌐 Python | 📅 2023-09-05]
* **SyncTrack** (Synchronize Feature Extracting and Matching: A Single Branch Framework for 3D Object Tracking) \[[paper](https://arxiv.org/abs/2308.12549)] \[~~code~~]

### AAAI 2023

* **GLT-T** (GLT-T: Global-Local Transformer Voting for 3D Single Object Tracking in Point Clouds) \[[paper](https://arxiv.org/abs/2211.10927)] \[[code](https://github.com/haooozi/GLT-T) ⭐ 39 | 🐛 3 | 🌐 Python | 📅 2023-12-18]

### IJCAI 2023

* **OSP2B** (OSP2B: One-Stage Point-to-Box Network for 3D Siamese Tracking) \[[paper](https://arxiv.org/abs/2304.11584)] \[~~code~~]

### IROS 2023

* **PCET** (Implicit and Efficient Point Cloud Completion for 3D Single Object Tracking) \[[paper](https://arxiv.org/abs/2209.00522)] \[~~code~~]
* **STTracker** (STTracker: Spatio-Temporal Tracker for 3D Single Object Tracking) \[[paper](https://arxiv.org/abs/2306.17440)] \[~~code~~]

### Preprint 2023

* **GLT-T++** (GLT-T++: Global-Local Transformer for 3D Siamese Tracking with Ranking Loss) \[[paper](https://arxiv.org/abs/2304.00242)] \[[code](https://github.com/haooozi/GLT-T) ⭐ 39 | 🐛 3 | 🌐 Python | 📅 2023-12-18]
* **MTM-Tracker** (Motion-to-Matching: A Mixed Paradigm for 3D Single Object Tracking) \[[paper](https://arxiv.org/abs/2308.11875)] \[[code](https://github.com/LeoZhiheng/MTM-Tracker) ⭐ 14 | 🐛 0 | 🌐 Python | 📅 2024-04-01]
* **MMF-Track** (Multi-Modal Multi-Level Fusion for 3D Single Object Tracking) \[[paper](https://arxiv.org/abs/2305.06794)] \[[code](https://github.com/LeoZhiheng/MMF-Tracker) ⭐ 11 | 🐛 1 | 📅 2024-04-01]
* **MCSTN** (Multi-Correlation Siamese Transformer Network with Dense Connection for 3D Single Object Tracking) \[[paper](https://arxiv.org/abs/2312.11051)] \[[code](https://github.com/liangp/MCSTN-3DSOT) ⭐ 4 | 🐛 0 | 🌐 Python | 📅 2023-12-05]
* **StreamTrack** (Modeling Continuous Motion for 3D Point Cloud Object Tracking) \[[paper](https://arxiv.org/abs/2303.07605)] \[~~code~~]

### CVPR 2022

* **PTTR** (PTTR: Relational 3D Point Cloud Object Tracking with Transformer) \[[paper](https://arxiv.org/abs/2112.02857)] \[[code](https://github.com/Jasonkks/PTTR) ⭐ 139 | 🐛 14 | 🌐 Python | 📅 2022-12-02]

### ECCV 2022

* **STNet** (3D Siamese Transformer Network for Single Object Tracking on Point Clouds) \[[paper](https://arxiv.org/abs/2207.11995)] \[[code](https://github.com/fpthink/STNet) ⭐ 40 | 🐛 3 | 🌐 Python | 📅 2022-11-27]
* **CMT** (CMT: Context-Matching-Guided Transformer for 3D Tracking in Point Clouds) \[[paper](https://www.ecva.net/papers/eccv_2022/papers_ECCV/html/1253_ECCV_2022_paper.php)] \[[code](https://github.com/jasongzy/CMT) ⚠️ Archived]
* **SpOT** (SpOT: Spatiotemporal Modeling for 3D Object Tracking) \[[paper](https://arxiv.org/abs/2207.05856)] \[~~code~~]

### Preprint 2022

* **PTTR++** (Exploring Point-BEV Fusion for 3D Point Cloud Object Tracking with Transformer) \[[paper](https://arxiv.org/abs/2208.05216)] \[[code](https://github.com/Jasonkks/PTTR) ⭐ 139 | 🐛 14 | 🌐 Python | 📅 2022-12-02]
* **OST** (OST: Efficient One-stream Network for 3D Single Object Tracking in Point Clouds) \[[paper](https://arxiv.org/abs/2210.08518)] \[~~code~~]
* **RDT** (Point Cloud Registration-Driven Robust Feature Matching for 3D Siamese Object Tracking) \[[paper](https://arxiv.org/abs/2209.06395)] \[~~code~~]

### BMVC 2021

* **LTTR** (3D Object Tracking with Transformer) \[[paper](https://arxiv.org/abs/2110.14921)] \[[code](https://github.com/3bobo/lttr) ⭐ 22 | 🐛 0 | 🌐 Python | 📅 2022-08-27]

### IROS 2021

* **PTT** (PTT: Point-Track-Transformer Module for 3D Single Object Tracking in Point Clouds) \[[paper](https://arxiv.org/abs/2108.06455)] \[[code](https://github.com/shanjiayao/PTT) ⭐ 91 | 🐛 2 | 🌐 Python | 📅 2022-06-29]

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-09-01._
