# Narrative Layer Papers

Papers on story coherence, screenplay generation, and narrative logic evaluation.

## Overview

The narrative layer evaluates the storytelling quality of generated content:
- **Story Logic**: Coherence, causality, state tracking
- **Screenplay Format**: Visualizability, format compliance
- **Long-form Generation**: Outline adherence, emotional arc

## Story Logic & Coherence

| Paper | Venue | Links | Key Metrics | Notes |
|-------|-------|-------|-------------|-------|
| **SCORE: Story Coherence and Retrieval Enhancement for AI Narratives** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2503.23512-b31b1b.svg)](https://arxiv.org/abs/2503.23512) | Logic Consistency Metric, Dynamic State Tracking | Symbol-based verification |
| **Can LLMs Generate Good Stories? Insights from Narrative Planning** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2506.10161-b31b1b.svg)](https://arxiv.org/abs/2506.10161) | Causal Soundness, Planning Score | Narrative planning perspective |
| **Generating Long-form Story Using Dynamic Hierarchical Outlining with Memory-Enhancement (DOME)** | arXiv 2024 | [![arXiv](https://img.shields.io/badge/arXiv-2412.13575-b31b1b.svg)](https://arxiv.org/abs/2412.13575) | Outline Adherence Score, Emotional Arc Consistency | Macro-planning approach |
| **StoryBench: A Multifaceted Benchmark for Continuous Story Visualization** | NeurIPS 2023 | [![Paper](https://img.shields.io/badge/NeurIPS-2023-purple.svg)](https://proceedings.neurips.cc/paper_files/paper/2023/file/f63f5fbed1a4ef08c857c5f377b5d33a-Paper-Datasets_and_Benchmarks.pdf) | Story continuation metrics | Continuous visualization |
| **Designing an Automatic Story Evaluation Metric** | Stanford | [![Paper](https://img.shields.io/badge/Stanford-Report-orange.svg)](https://web.stanford.edu/class/archive/cs/cs224n/cs224n.1224/reports/custom_117176750.pdf) | Story Cloze Test | Classic story evaluation |

## Screenplay & Script Generation

| Paper | Venue | Links | Key Metrics | Notes |
|-------|-------|-------|-------------|-------|
| **Beyond Direct Generation: A Decomposed Approach to Well-Crafted Screenwriting with LLMs (DSR)** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2510.23163-b31b1b.svg)](https://arxiv.org/abs/2510.23163) | Visualizability Score, Format Compliance | Dual-stage refinement |
| **ETVA: Evaluation of Text-to-Video Alignment via Fine-grained Question Generation and Answering** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2503.16867-b31b1b.svg)](https://arxiv.org/abs/2503.16867) | QA-based alignment | Fine-grained evaluation |

## Tools

| Tool | Type | Links | Description |
|------|------|-------|-------------|
| **Prescene** | Commercial | [![Website](https://img.shields.io/badge/Website-prescene.ai-blue.svg)](https://www.prescene.ai/) | AI for screenplay analysis and coverage |

## Key Concepts

### Dynamic State Tracking
Parsing story into symbolic state lists:
```
{Character: Hero, Status: Injured, Location: Cave}
```
Each new sentence is checked against current state for conflicts.

### Outline Adherence Score
Measures how well generated content follows the predefined outline through semantic coverage of keywords.

### Visualizability Score
Classifies action descriptions as:
- **High Visualizability**: "He frowned, staring at the extinguished cigarette butt"
- **Low Visualizability**: "He felt a sense of existential anxiety"

### Format Compliance
Checks screenplay adherence to standard formats (e.g., Fountain):
- Sluglines (scene headers)
- Character names
- Dialogue indentation

## Navigation

- [← Previous: Cognitive Layer](01-cognitive-layer.md)
- [→ Next: Visual Layer](03-visual-layer.md)

---

# 叙事层论文

故事连贯性、剧本生成与叙事逻辑评估相关论文。

## 概述

叙事层评估生成内容的叙事质量：
- **故事逻辑**：连贯性、因果性、状态追踪
- **剧本格式**：可视化潜力、格式合规性
- **长篇生成**：大纲依从度、情感弧

## 故事逻辑与连贯性

| 论文 | 会议 | 链接 | 核心指标 | 备注 |
|------|------|------|----------|------|
| **SCORE: Story Coherence and Retrieval Enhancement for AI Narratives** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2503.23512-b31b1b.svg)](https://arxiv.org/abs/2503.23512) | 逻辑一致性指标, 动态状态追踪 | 符号化验证 |
| **Can LLMs Generate Good Stories? Insights from Narrative Planning** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2506.10161-b31b1b.svg)](https://arxiv.org/abs/2506.10161) | 因果合理性, 规划评分 | 叙事规划视角 |
| **Generating Long-form Story Using Dynamic Hierarchical Outlining with Memory-Enhancement (DOME)** | arXiv 2024 | [![arXiv](https://img.shields.io/badge/arXiv-2412.13575-b31b1b.svg)](https://arxiv.org/abs/2412.13575) | 大纲依从度, 情感弧一致性 | 宏观规划方法 |
| **StoryBench: A Multifaceted Benchmark for Continuous Story Visualization** | NeurIPS 2023 | [![Paper](https://img.shields.io/badge/NeurIPS-2023-purple.svg)](https://proceedings.neurips.cc/paper_files/paper/2023/file/f63f5fbed1a4ef08c857c5f377b5d33a-Paper-Datasets_and_Benchmarks.pdf) | 故事延续指标 | 连续可视化 |
| **Designing an Automatic Story Evaluation Metric** | Stanford | [![Paper](https://img.shields.io/badge/Stanford-Report-orange.svg)](https://web.stanford.edu/class/archive/cs/cs224n/cs224n.1224/reports/custom_117176750.pdf) | Story Cloze Test | 经典故事评估 |

## 剧本与脚本生成

| 论文 | 会议 | 链接 | 核心指标 | 备注 |
|------|------|------|----------|------|
| **Beyond Direct Generation: A Decomposed Approach to Well-Crafted Screenwriting with LLMs (DSR)** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2510.23163-b31b1b.svg)](https://arxiv.org/abs/2510.23163) | 可视化分数, 格式合规性 | 双阶段优化 |
| **ETVA: Evaluation of Text-to-Video Alignment via Fine-grained Question Generation and Answering** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2503.16867-b31b1b.svg)](https://arxiv.org/abs/2503.16867) | 基于QA的对齐 | 细粒度评估 |

## 工具

| 工具 | 类型 | 链接 | 描述 |
|------|------|------|------|
| **Prescene** | 商业 | [![Website](https://img.shields.io/badge/Website-prescene.ai-blue.svg)](https://www.prescene.ai/) | AI剧本分析与覆盖工具 |

## 关键概念

### 动态状态追踪
将故事解析为符号化状态列表：
```
{角色: 英雄, 状态: 受伤, 位置: 洞穴}
```
每生成一个新句子都会检查是否与当前状态冲突。

### 大纲依从度
通过关键词的语义覆盖率衡量生成内容对预设大纲的遵循程度。

### 可视化分数
将动作描写分类为：
- **高可视化**："他皱着眉头，盯着手里熄灭的烟头"
- **低可视化**："他感到一种存在主义的焦虑"

### 格式合规性
检查剧本对标准格式（如Fountain格式）的遵循：
- 场景标题（Sluglines）
- 角色名
- 对话缩进

## 导航

- [← 上一章：认知层](01-cognitive-layer.md)
- [→ 下一章：视觉层](03-visual-layer.md)
