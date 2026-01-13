# Visual Layer Papers

Papers on character consistency, text-image alignment, and video generation quality.

## Overview

The visual layer evaluates the quality of generated images and videos:
- **Character Consistency**: Identity preservation across frames
- **Text-Image Alignment**: Prompt faithfulness, attribute binding
- **Video Quality**: Temporal coherence, motion smoothness
- **Style Consistency**: Artistic style uniformity

## Story Visualization & Character Consistency

| Paper | Venue | Links | Key Metrics | Notes |
|-------|-------|-------|-------------|-------|
| **ViStoryBench: Comprehensive Benchmark Suite for Story Visualization** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2505.24862-b31b1b.svg)](https://arxiv.org/abs/2505.24862) | CIDS, OCCM, CSD | Comprehensive story viz benchmark |
| **CharaConsist: Fine-Grained Consistent Character Generation** | ICCV 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2507.11533-b31b1b.svg)](https://arxiv.org/abs/2507.11533) | Foreground/Background consistency | SAM-based segmentation |
| **TheaterGen: Character Management with LLM for Consistent Multi-turn Image Generation** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2404.18919-b31b1b.svg)](https://arxiv.org/abs/2404.18919) | CMIGBench | 8000 multi-turn instructions |
| **Face Consistency Benchmark for GenAI Video** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2505.11425-b31b1b.svg)](https://arxiv.org/abs/2505.11425) | FCB Score | AIGC video face consistency |
| **MangaVQA: A Benchmark for Multimodal Manga Understanding** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2505.20298-b31b1b.svg)](https://arxiv.org/abs/2505.20298) | MangaOCR, MangaVQA | Manga comprehension + specialized LMM |
| **CoMix: A Comprehensive Benchmark for Multi-Task Comic Understanding** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2407.03550-b31b1b.svg)](https://arxiv.org/abs/2407.03550) | Detection, Re-ID, Reading Order | 3.8k images, 130k annotations |
| **MangaDiffusion: Manga Generation via Layout-controllable Diffusion** | arXiv 2024 | [![arXiv](https://img.shields.io/badge/arXiv-2412.19303-b31b1b.svg)](https://arxiv.org/abs/2412.19303) | Layout Control Score | Manga109Story dataset |

## Text-Image Alignment

| Paper | Venue | Links | Key Metrics | Notes |
|-------|-------|-------|-------------|-------|
| **VQAScore** | GitHub | [![GitHub](https://img.shields.io/github/stars/linzhiqiu/t2v_metrics.svg?style=social)](https://github.com/linzhiqiu/t2v_metrics) | VQAScore | VQA-based alignment |
| **What makes a good metric? Evaluating automatic metrics for text-to-image consistency (DSG)** | arXiv 2024 | [![arXiv](https://img.shields.io/badge/arXiv-2412.13989-b31b1b.svg)](https://arxiv.org/abs/2412.13989) | DSG Score | Dynamic scene graphs |
| **A Survey on Quality Metrics for Text-to-Image Generation** | arXiv 2024 | [![arXiv](https://img.shields.io/badge/arXiv-2403.11821-b31b1b.svg)](https://arxiv.org/abs/2403.11821) | Survey | CLIPScore and beyond |

## Video Generation Quality

| Paper | Venue | Links | Key Metrics | Notes |
|-------|-------|-------|-------------|-------|
| **Beyond FVD: Enhanced Evaluation Metrics for Video Generation Quality (JEDi)** | ICLR 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2410.05203-b31b1b.svg)](https://arxiv.org/abs/2410.05203) | JEDi (JEPA Embedding Distance) | 34% better correlation than FVD |
| **T2VBench: Benchmarking Temporal Dynamics for Text-to-Video Generation** | CVPR 2024 | [![Paper](https://img.shields.io/badge/CVPR-2024-blue.svg)](https://openaccess.thecvf.com/content/CVPR2024W/EvGenFM/papers/Ji_T2VBench_Benchmarking_Temporal_Dynamics_for_Text-to-Video_Generation_CVPRW_2024_paper.pdf) | Motion Smoothness, Subject Persistence | 16 temporal dimensions |
| **T2VWorldBench: A Benchmark for Evaluating World Knowledge in Text-to-Video Generation** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2507.18107-b31b1b.svg)](https://arxiv.org/abs/2507.18107) | Physics Compliance Score | World knowledge evaluation |
| **T2V-CompBench: A Comprehensive Benchmark for Compositional Text-to-Video Generation** | CVPR 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2407.14505-b31b1b.svg)](https://arxiv.org/abs/2407.14505) | Compositional Score | 1400 prompts, 7 composition types |
| **T2VTextBench: A Human Evaluation Benchmark for Textual Control in Video Generation** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2505.04946-b31b1b.svg)](https://arxiv.org/abs/2505.04946) | Text Fidelity Score | On-screen text evaluation |
| **VBench-2.0: Comprehensive Video Generation Benchmark** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2503.21755-b31b1b.svg)](https://arxiv.org/abs/2503.21755) | Physics Realism, Creative Composition | Intrinsic faithfulness evaluation |
| **VidCapBench: A Comprehensive Benchmark for Video Captioning** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2502.12782-b31b1b.svg)](https://arxiv.org/abs/2502.12782) | Caption Quality Score | Controllable T2V caption evaluation |

## Key Concepts

### Character Identification Similarity (CIDS)
1. Use Grounding DINO to detect and crop character regions
2. Extract features with ArcFace/AdaFace or CLIP-ViT
3. Compute cosine similarity with reference character sheet
4. Threshold: Cosine Similarity > 0.7 typically indicates same person

### Onstage Character Count Matching (OCCM)
Compares number of detected characters against prompt entities:
- Detects "character loss" (missing characters)
- Detects "character hallucination" (extra characters)

### VQAScore
1. Decompose prompt into questions: "Is there a knight?" "Is it raining?"
2. Use VQA model to answer questions about generated image
3. Score = proportion of correctly answered questions

### JEDi (JEPA Embedding Distance)
Based on Joint Embedding Predictive Architecture:
- Better correlation with human perception of video quality
- More sensitive to temporal/motion quality than FVD

### Consistent Style Distance (CSD)
Measures style uniformity across image sequence:
- Train style-sensitive CLIP variant
- Extract style embeddings for all frames
- Lower variance = more consistent style

## Navigation

- [← Previous: Narrative Layer](02-narrative-layer.md)
- [→ Next: Audio Layer](04-audio-layer.md)

---

# 视觉层论文

角色一致性、图文对齐与视频生成质量相关论文。

## 概述

视觉层评估生成图像和视频的质量：
- **角色一致性**：跨帧身份保持
- **图文对齐**：提示词忠实度、属性绑定
- **视频质量**：时间连贯性、运动平滑度
- **风格一致性**：艺术风格统一性

## 故事可视化与角色一致性

| 论文 | 会议 | 链接 | 核心指标 | 备注 |
|------|------|------|----------|------|
| **ViStoryBench: Comprehensive Benchmark Suite for Story Visualization** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2505.24862-b31b1b.svg)](https://arxiv.org/abs/2505.24862) | CIDS, OCCM, CSD | 综合故事可视化基准 |
| **CharaConsist: Fine-Grained Consistent Character Generation** | ICCV 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2507.11533-b31b1b.svg)](https://arxiv.org/abs/2507.11533) | 前景/背景一致性 | 基于SAM的分割 |
| **TheaterGen: Character Management with LLM for Consistent Multi-turn Image Generation** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2404.18919-b31b1b.svg)](https://arxiv.org/abs/2404.18919) | CMIGBench | 8000多轮指令 |
| **Face Consistency Benchmark for GenAI Video** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2505.11425-b31b1b.svg)](https://arxiv.org/abs/2505.11425) | FCB评分 | AIGC视频人脸一致性 |
| **MangaVQA: A Benchmark for Multimodal Manga Understanding** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2505.20298-b31b1b.svg)](https://arxiv.org/abs/2505.20298) | MangaOCR, MangaVQA | 漫画理解+专用LMM |
| **CoMix: A Comprehensive Benchmark for Multi-Task Comic Understanding** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2407.03550-b31b1b.svg)](https://arxiv.org/abs/2407.03550) | 检测, 重识别, 阅读顺序 | 3.8k图像, 130k标注 |
| **MangaDiffusion: Manga Generation via Layout-controllable Diffusion** | arXiv 2024 | [![arXiv](https://img.shields.io/badge/arXiv-2412.19303-b31b1b.svg)](https://arxiv.org/abs/2412.19303) | 布局控制评分 | Manga109Story数据集 |

## 图文对齐

| 论文 | 会议 | 链接 | 核心指标 | 备注 |
|------|------|------|----------|------|
| **VQAScore** | GitHub | [![GitHub](https://img.shields.io/github/stars/linzhiqiu/t2v_metrics.svg?style=social)](https://github.com/linzhiqiu/t2v_metrics) | VQAScore | 基于VQA的对齐 |
| **What makes a good metric? Evaluating automatic metrics for text-to-image consistency (DSG)** | arXiv 2024 | [![arXiv](https://img.shields.io/badge/arXiv-2412.13989-b31b1b.svg)](https://arxiv.org/abs/2412.13989) | DSG分数 | 动态场景图 |
| **A Survey on Quality Metrics for Text-to-Image Generation** | arXiv 2024 | [![arXiv](https://img.shields.io/badge/arXiv-2403.11821-b31b1b.svg)](https://arxiv.org/abs/2403.11821) | 综述 | CLIPScore及其扩展 |

## 视频生成质量

| 论文 | 会议 | 链接 | 核心指标 | 备注 |
|------|------|------|----------|------|
| **Beyond FVD: Enhanced Evaluation Metrics for Video Generation Quality (JEDi)** | ICLR 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2410.05203-b31b1b.svg)](https://arxiv.org/abs/2410.05203) | JEDi (JEPA嵌入距离) | 比FVD相关性高34% |
| **T2VBench: Benchmarking Temporal Dynamics for Text-to-Video Generation** | CVPR 2024 | [![Paper](https://img.shields.io/badge/CVPR-2024-blue.svg)](https://openaccess.thecvf.com/content/CVPR2024W/EvGenFM/papers/Ji_T2VBench_Benchmarking_Temporal_Dynamics_for_Text-to-Video_Generation_CVPRW_2024_paper.pdf) | 运动平滑度, 主体持久性 | 16个时间维度 |
| **T2VWorldBench: A Benchmark for Evaluating World Knowledge in Text-to-Video Generation** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2507.18107-b31b1b.svg)](https://arxiv.org/abs/2507.18107) | 物理合规性分数 | 世界知识评估 |
| **T2V-CompBench: A Comprehensive Benchmark for Compositional Text-to-Video Generation** | CVPR 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2407.14505-b31b1b.svg)](https://arxiv.org/abs/2407.14505) | 组合评分 | 1400提示词, 7种组合类型 |
| **T2VTextBench: A Human Evaluation Benchmark for Textual Control in Video Generation** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2505.04946-b31b1b.svg)](https://arxiv.org/abs/2505.04946) | 文字保真度 | 视频内文字评估 |
| **VBench-2.0: Comprehensive Video Generation Benchmark** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2503.21755-b31b1b.svg)](https://arxiv.org/abs/2503.21755) | 物理真实性, 创意组合 | 内在忠实度评估 |
| **VidCapBench: A Comprehensive Benchmark for Video Captioning** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2502.12782-b31b1b.svg)](https://arxiv.org/abs/2502.12782) | 字幕质量评分 | 可控T2V字幕评估 |

## 关键概念

### 角色识别相似度（CIDS）
1. 使用Grounding DINO检测并裁剪角色区域
2. 用ArcFace/AdaFace或CLIP-ViT提取特征
3. 与参考角色设定图计算余弦相似度
4. 阈值：余弦相似度 > 0.7 通常表示同一人

### 在场角色数量匹配（OCCM）
将检测到的角色数量与提示词中的实体进行比对：
- 检测"角色丢失"（缺失角色）
- 检测"角色幻觉"（多余角色）

### VQAScore
1. 将提示词分解为问题："有骑士吗？""在下雨吗？"
2. 使用VQA模型回答关于生成图像的问题
3. 分数 = 正确回答问题的比例

### JEDi（JEPA嵌入距离）
基于联合嵌入预测架构：
- 与人类对视频质量的感知相关性更好
- 对时间/运动质量比FVD更敏感

### 一致风格距离（CSD）
衡量图像序列的风格统一性：
- 训练对风格敏感的CLIP变体
- 提取所有帧的风格嵌入
- 方差越低 = 风格越统一

## 导航

- [← 上一章：叙事层](02-narrative-layer.md)
- [→ 下一章：听觉层](04-audio-layer.md)
