# Audio Layer Papers

Papers on TTS expressiveness, music generation, and lip-sync quality.

## Overview

The audio layer evaluates the quality of generated audio content:
- **TTS Expressiveness**: Paralinguistic features, emotional appropriateness
- **Music Generation**: Style matching, structural integrity
- **Lip-Sync Quality**: Audio-visual synchronization

## TTS Expressiveness

| Paper | Venue | Links | Key Metrics | Notes |
|-------|-------|-------|-------------|-------|
| **EmergentTTS-Eval: Evaluating TTS Models on Complex Prosodic, Expressiveness, and Linguistic Challenges** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2505.23009-b31b1b.svg)](https://arxiv.org/abs/2505.23009) | Paralinguistic Accuracy, Emotional Appropriateness | Model-as-Judge approach |
| **EmoSSLSphere: Multilingual Emotional Speech Synthesis with Spherical Vectors** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2508.11273-b31b1b.svg)](https://arxiv.org/abs/2508.11273) | Emotion Control Score | Spherical vectors + discrete tokens |

## Music Generation

| Paper | Venue | Links | Key Metrics | Notes |
|-------|-------|-------|-------------|-------|
| **MusicEval: A Generative Music Dataset with Expert Ratings for Automatic Text-to-Music Evaluation** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2501.10811-b31b1b.svg)](https://arxiv.org/abs/2501.10811) | Expert ratings | Text-to-music evaluation |
| **SongEval: A Benchmark Dataset for Song Aesthetics Evaluation** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2505.10793-b31b1b.svg)](https://arxiv.org/abs/2505.10793) | Aesthetics scores | Song quality evaluation |
| **Benchmarking Music Generation Models and Metrics via Human Preference Studies** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2506.19085-b31b1b.svg)](https://arxiv.org/abs/2506.19085) | CLAP Score | Human preference alignment |
| **A Survey on Evaluation Metrics for Music Generation** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2509.00051-b31b1b.svg)](https://arxiv.org/abs/2509.00051) | Survey | Comprehensive metrics review |

## Lip-Sync & Audio-Visual Synchronization

| Paper | Venue | Links | Key Metrics | Notes |
|-------|-------|-------|-------------|-------|
| **Audio-Visual Speech Representation Expert for Enhanced Talking Face Video Generation and Evaluation** | arXiv 2024 | [![arXiv](https://img.shields.io/badge/arXiv-2405.04327-b31b1b.svg)](https://arxiv.org/abs/2405.04327) | LSE-D (Lip-Sync Error Distance) | SyncNet-based evaluation |
| **Lips Are Lying: Spotting the Temporal Inconsistency between Audio and Visual in Lip-Syncing DeepFakes (LipFD)** | NeurIPS 2024 | [![Paper](https://img.shields.io/badge/NeurIPS-2024-purple.svg)](https://proceedings.neurips.cc/paper_files/paper/2024/file/a5a5b0ff87c59172a13342d428b1e033-Paper-Conference.pdf) | Lip Forgery Detection | Quality control for lip-sync |
| **OmniSync: Towards Universal Lip Synchronization via Diffusion Transformers** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2505.21448-b31b1b.svg)](https://arxiv.org/abs/2505.21448) | AIGC-LipSync Benchmark | Universal lip-sync for AIGC |
| **SyncAnyone: Implicit Disentanglement via Progressive Self-Correction** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2512.21736-b31b1b.svg)](https://arxiv.org/abs/2512.21736) | Identity Preservation | In-the-wild lip-syncing |
| **SayAnything: Audio-Driven Lip Synchronization with Conditional Video Diffusion** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2502.11515-b31b1b.svg)](https://arxiv.org/abs/2502.11515) | Lip Motion Quality | Conditional video diffusion |
| **LatentSync: Taming Audio-Conditioned Latent Diffusion Models for Lip Sync** | arXiv 2024 | [![arXiv](https://img.shields.io/badge/arXiv-2412.09262-b31b1b.svg)](https://arxiv.org/abs/2412.09262) | StableSyncNet Accuracy | Temporal alignment mechanism |
| **Wav2Lip** | ACMMM 2020 | [![Topic](https://img.shields.io/badge/Topic-Wav2Lip-green.svg)](https://www.emergentmind.com/topics/wav2lip) | - | Audio-driven lip sync |

## Key Concepts

### Paralinguistic Accuracy
Evaluates whether TTS correctly renders non-verbal sounds:
- [sigh], [laugh], [hesitation]
- Detected using audio classification models

### Emotional Appropriateness
Uses Speech Emotion Recognition (SER) to:
1. Analyze emotional polarity of generated audio
2. Compare with script's emotion labels
3. Compute matching score

### CLAP Score
Contrastive Language-Audio Pretraining:
- Similar to CLIP for images
- Measures semantic alignment between audio and text description
- Example: "sad piano piece" → audio

### LSE-D (Lip-Sync Error Distance)
Industry-standard metric using SyncNet:
1. Extract audio features
2. Extract lip region video features
3. Compute distance between feature sequences
4. Lower distance = better synchronization

### LipFD (Lip Forgery Detection)
Detects lip-sync artifacts:
- Blurriness in lip region
- Temporal inconsistencies
- Used as quality control filter

## Navigation

- [← Previous: Visual Layer](03-visual-layer.md)
- [→ Next: System Layer](05-system-layer.md)

---

# 听觉层论文

TTS表现力、音乐生成与口型同步质量相关论文。

## 概述

听觉层评估生成音频内容的质量：
- **TTS表现力**：副语言特征、情感适宜性
- **音乐生成**：风格匹配、结构完整性
- **口型同步质量**：视听同步

## TTS表现力

| 论文 | 会议 | 链接 | 核心指标 | 备注 |
|------|------|------|----------|------|
| **EmergentTTS-Eval: Evaluating TTS Models on Complex Prosodic, Expressiveness, and Linguistic Challenges** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2505.23009-b31b1b.svg)](https://arxiv.org/abs/2505.23009) | 副语言准确性, 情感适宜度 | Model-as-Judge方法 |
| **EmoSSLSphere: Multilingual Emotional Speech Synthesis with Spherical Vectors** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2508.11273-b31b1b.svg)](https://arxiv.org/abs/2508.11273) | 情感控制评分 | 球面向量+离散token |

## 音乐生成

| 论文 | 会议 | 链接 | 核心指标 | 备注 |
|------|------|------|----------|------|
| **MusicEval: A Generative Music Dataset with Expert Ratings for Automatic Text-to-Music Evaluation** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2501.10811-b31b1b.svg)](https://arxiv.org/abs/2501.10811) | 专家评分 | 文本到音乐评估 |
| **SongEval: A Benchmark Dataset for Song Aesthetics Evaluation** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2505.10793-b31b1b.svg)](https://arxiv.org/abs/2505.10793) | 美学分数 | 歌曲质量评估 |
| **Benchmarking Music Generation Models and Metrics via Human Preference Studies** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2506.19085-b31b1b.svg)](https://arxiv.org/abs/2506.19085) | CLAP分数 | 人类偏好对齐 |
| **A Survey on Evaluation Metrics for Music Generation** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2509.00051-b31b1b.svg)](https://arxiv.org/abs/2509.00051) | 综述 | 全面指标回顾 |

## 口型同步与视听同步

| 论文 | 会议 | 链接 | 核心指标 | 备注 |
|------|------|------|----------|------|
| **Audio-Visual Speech Representation Expert for Enhanced Talking Face Video Generation and Evaluation** | arXiv 2024 | [![arXiv](https://img.shields.io/badge/arXiv-2405.04327-b31b1b.svg)](https://arxiv.org/abs/2405.04327) | LSE-D (口型同步误差距离) | 基于SyncNet的评估 |
| **Lips Are Lying: Spotting the Temporal Inconsistency between Audio and Visual in Lip-Syncing DeepFakes (LipFD)** | NeurIPS 2024 | [![Paper](https://img.shields.io/badge/NeurIPS-2024-purple.svg)](https://proceedings.neurips.cc/paper_files/paper/2024/file/a5a5b0ff87c59172a13342d428b1e033-Paper-Conference.pdf) | 口型伪造检测 | 口型同步质量控制 |
| **OmniSync: Towards Universal Lip Synchronization via Diffusion Transformers** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2505.21448-b31b1b.svg)](https://arxiv.org/abs/2505.21448) | AIGC口型同步基准 | AIGC通用口型同步 |
| **SyncAnyone: Implicit Disentanglement via Progressive Self-Correction** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2512.21736-b31b1b.svg)](https://arxiv.org/abs/2512.21736) | 身份保持 | 野外场景口型同步 |
| **SayAnything: Audio-Driven Lip Synchronization with Conditional Video Diffusion** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2502.11515-b31b1b.svg)](https://arxiv.org/abs/2502.11515) | 唇动质量 | 条件视频扩散 |
| **LatentSync: Taming Audio-Conditioned Latent Diffusion Models for Lip Sync** | arXiv 2024 | [![arXiv](https://img.shields.io/badge/arXiv-2412.09262-b31b1b.svg)](https://arxiv.org/abs/2412.09262) | StableSyncNet准确率 | 时序对齐机制 |
| **Wav2Lip** | ACMMM 2020 | [![Topic](https://img.shields.io/badge/Topic-Wav2Lip-green.svg)](https://www.emergentmind.com/topics/wav2lip) | - | 音频驱动口型同步 |

## 关键概念

### 副语言准确性
评估TTS是否正确渲染非语言声音：
- [叹气]、[大笑]、[犹豫]
- 使用音频分类模型检测

### 情感适宜度
使用语音情感识别（SER）：
1. 分析生成音频的情感极性
2. 与剧本的情感标签对比
3. 计算匹配分数

### CLAP分数
对比语言-音频预训练：
- 类似于图像的CLIP
- 衡量音频与文本描述的语义对齐
- 示例："悲伤的钢琴曲" → 音频

### LSE-D（口型同步误差距离）
使用SyncNet的工业标准指标：
1. 提取音频特征
2. 提取唇部区域视频特征
3. 计算特征序列之间的距离
4. 距离越小 = 同步越好

### LipFD（口型伪造检测）
检测口型同步伪影：
- 唇部区域模糊
- 时间不一致
- 用作质量控制过滤器

## 导航

- [← 上一章：视觉层](03-visual-layer.md)
- [→ 下一章：系统层](05-system-layer.md)
