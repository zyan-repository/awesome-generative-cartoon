# Benchmarks Summary

Quick reference table of all evaluation benchmarks and metrics.

## Overview by Layer

| Layer | Focus Area | Key Benchmarks |
|-------|------------|----------------|
| Cognitive | Agent Intelligence | AgentBench, MultiAgentBench, RolePlayEval |
| Narrative | Story & Script | SCORE, DOME, StoryBench |
| Visual | Image & Video | ViStoryBench, CharaConsist, JEDi |
| Audio | TTS & Music | EmergentTTS-Eval, MusicEval, LSE-D |
| System | Toolkits | DeepEval, t2v_metrics |

## Complete Metrics Reference

### Cognitive Layer Metrics

| Metric | Full Name | Description | Range |
|--------|-----------|-------------|-------|
| SR | Success Rate | Task completion percentage | 0-100% |
| Pass@k | Pass at K | Correct solution within k attempts | 0-1 |
| CS | Collaboration Score | Task completion / Communication cost | Higher = Better |
| ICC | In-Character Consistency | Persona maintenance score | 0-1 |
| IDS | Information Diversity Score | Semantic increment in communication | Higher = Better |
| UPR | Unnecessary Path Ratio | Wasted reasoning nodes | Lower = Better |

### Narrative Layer Metrics

| Metric | Full Name | Description | Range |
|--------|-----------|-------------|-------|
| Logic Score | Logic Consistency | State conflict detection | 0-1 |
| OAS | Outline Adherence Score | Keyword semantic coverage | 0-1 |
| EAC | Emotional Arc Consistency | Sentiment curve matching | 0-1 |
| Viz Score | Visualizability Score | Action description clarity | 0-1 |
| FCR | Format Compliance Rate | Screenplay format adherence | 0-100% |

### Visual Layer Metrics

| Metric | Full Name | Description | Range |
|--------|-----------|-------------|-------|
| CIDS | Character ID Similarity | Cosine similarity with reference | 0-1 (>0.7 = same) |
| OCCM | Onstage Character Count Matching | Character count accuracy | 0-1 |
| CSD | Consistent Style Distance | Style embedding variance | Lower = Better |
| VQAScore | VQA-based Score | QA correctness ratio | 0-1 |
| FVD | Fréchet Video Distance | Video distribution distance | Lower = Better |
| JEDi | JEPA Embedding Distance | Motion-aware video quality | Lower = Better |

### Audio Layer Metrics

| Metric | Full Name | Description | Range |
|--------|-----------|-------------|-------|
| PA | Paralinguistic Accuracy | Non-verbal sound rendering | 0-1 |
| EA | Emotional Appropriateness | Emotion label matching | 0-1 |
| CLAP | Contrastive Language-Audio | Audio-text alignment | Higher = Better |
| LSE-D | Lip-Sync Error Distance | Audio-visual sync distance | Lower = Better |
| LipFD | Lip Forgery Detection | Artifact detection score | Lower = Better |

## Recommended Composite Score

```
SystemScore = 0.30 × Narrative + 0.40 × Visual + 0.20 × Audio + 0.10 × AgentCoordination
```

## Priority Implementation Order

Based on the survey recommendations:

1. **High Priority** (Core pain points)
   - CIDS (Character Consistency)
   - Logic Score (Story Coherence)

2. **Medium Priority**
   - VQAScore (Text-Image Alignment)
   - JEDi (Video Quality)
   - LSE-D (Lip Sync)

3. **Lower Priority** (Optimization)
   - CS (Collaboration Score)
   - CSD (Style Consistency)

## Navigation

- [← Previous: System Layer](05-system-layer.md)
- [← Back to Overview](00-full-stack-overview.md)

---

# 基准汇总

所有评估基准和指标的快速参考表。

## 按层级概述

| 层级 | 重点领域 | 关键基准 |
|------|----------|----------|
| 认知层 | Agent智能 | AgentBench, MultiAgentBench, RolePlayEval |
| 叙事层 | 故事与剧本 | SCORE, DOME, StoryBench |
| 视觉层 | 图像与视频 | ViStoryBench, CharaConsist, JEDi |
| 听觉层 | TTS与音乐 | EmergentTTS-Eval, MusicEval, LSE-D |
| 系统层 | 工具包 | DeepEval, t2v_metrics |

## 完整指标参考

### 认知层指标

| 指标 | 全称 | 描述 | 范围 |
|------|------|------|------|
| SR | 成功率 | 任务完成百分比 | 0-100% |
| Pass@k | K次通过 | k次尝试内正确解决 | 0-1 |
| CS | 协作评分 | 任务完成度/通信成本 | 越高越好 |
| ICC | 角色内一致性 | 人格保持分数 | 0-1 |
| IDS | 信息多样性得分 | 通信中的语义增量 | 越高越好 |
| UPR | 非必要路径比率 | 浪费的推理节点 | 越低越好 |

### 叙事层指标

| 指标 | 全称 | 描述 | 范围 |
|------|------|------|------|
| Logic Score | 逻辑一致性 | 状态冲突检测 | 0-1 |
| OAS | 大纲依从度 | 关键词语义覆盖 | 0-1 |
| EAC | 情感弧一致性 | 情感曲线匹配 | 0-1 |
| Viz Score | 可视化分数 | 动作描写清晰度 | 0-1 |
| FCR | 格式合规率 | 剧本格式遵循度 | 0-100% |

### 视觉层指标

| 指标 | 全称 | 描述 | 范围 |
|------|------|------|------|
| CIDS | 角色识别相似度 | 与参考的余弦相似度 | 0-1 (>0.7=同一人) |
| OCCM | 在场角色数量匹配 | 角色数量准确度 | 0-1 |
| CSD | 一致风格距离 | 风格嵌入方差 | 越低越好 |
| VQAScore | 基于VQA的分数 | QA正确率 | 0-1 |
| FVD | Fréchet视频距离 | 视频分布距离 | 越低越好 |
| JEDi | JEPA嵌入距离 | 运动感知视频质量 | 越低越好 |

### 听觉层指标

| 指标 | 全称 | 描述 | 范围 |
|------|------|------|------|
| PA | 副语言准确性 | 非语言声音渲染 | 0-1 |
| EA | 情感适宜度 | 情感标签匹配 | 0-1 |
| CLAP | 对比语言-音频 | 音频-文本对齐 | 越高越好 |
| LSE-D | 口型同步误差距离 | 视听同步距离 | 越低越好 |
| LipFD | 口型伪造检测 | 伪影检测分数 | 越低越好 |

## 推荐综合评分

```
系统评分 = 0.30 × 叙事层 + 0.40 × 视觉层 + 0.20 × 听觉层 + 0.10 × Agent协作
```

## 优先实施顺序

根据调研报告建议：

1. **高优先级**（核心痛点）
   - CIDS（角色一致性）
   - Logic Score（故事连贯性）

2. **中优先级**
   - VQAScore（图文对齐）
   - JEDi（视频质量）
   - LSE-D（口型同步）

3. **较低优先级**（优化）
   - CS（协作评分）
   - CSD（风格一致性）

## 导航

- [← 上一章：系统层](05-system-layer.md)
- [← 返回概述](00-full-stack-overview.md)
