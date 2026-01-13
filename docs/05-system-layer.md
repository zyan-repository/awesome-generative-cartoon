# System Layer Papers

Evaluation toolkits, frameworks, and integration tools.

## Overview

The system layer provides tools for:
- **Evaluation Frameworks**: Automated testing and scoring
- **Metrics Libraries**: Pre-built evaluation metrics
- **Integration Tools**: End-to-end pipelines

## Evaluation Frameworks

| Tool | Type | Links | Description |
|------|------|-------|-------------|
| **DeepEval** | Framework | [![GitHub](https://img.shields.io/github/stars/confident-ai/deepeval.svg?style=social)](https://github.com/confident-ai/deepeval) | LLM evaluation framework with custom test cases |
| **t2v_metrics** | Library | [![GitHub](https://img.shields.io/github/stars/linzhiqiu/t2v_metrics.svg?style=social)](https://github.com/linzhiqiu/t2v_metrics) | Text-to-video/image evaluation metrics |

## Surveys & Comprehensive Reviews

| Paper | Venue | Links | Focus |
|-------|-------|-------|-------|
| **A Survey of Automatic Evaluation Methods on Text, Visual and Speech Generations** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2506.10019-b31b1b.svg)](https://arxiv.org/abs/2506.10019) | Comprehensive multimodal evaluation |
| **Evaluation and Benchmarking of LLM Agents: A Survey** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2507.21504-b31b1b.svg)](https://arxiv.org/abs/2507.21504) | Agent evaluation comprehensive survey |

## Commercial Tools

| Tool | Type | Links | Description |
|------|------|-------|-------------|
| **Prescene** | Commercial | [![Website](https://img.shields.io/badge/Website-prescene.ai-blue.svg)](https://www.prescene.ai/) | AI for screenplay analysis and coverage |

## LLM-as-a-Judge Paradigm

Given the high cost of human evaluation, the mainstream approach is using LLM-as-Judge:

### Implementation with DeepEval

```python
from deepeval import evaluate
from deepeval.metrics import GEval

# Create a Judge Agent (e.g., GPT-4o) as "Senior Manga Editor"
judge_metric = GEval(
    name="manga_quality",
    criteria="Evaluate the generated manga panel for character consistency and narrative coherence",
    evaluation_params=["actual_output", "expected_output"]
)

# Run evaluation
evaluate(test_cases, [judge_metric])
```

### Meta-Evaluation
To ensure Judge reliability:
1. Compare LLM evaluation results with human expert ratings
2. Compute Pearson/Spearman correlation
3. Research shows well-designed CoT prompts can improve alignment by 34%+

## Navigation

- [← Previous: Audio Layer](04-audio-layer.md)
- [→ Next: Benchmarks Summary](06-benchmarks-summary.md)

---

# 系统层论文

评测工具包、框架与集成工具。

## 概述

系统层提供以下工具：
- **评测框架**：自动化测试与评分
- **指标库**：预构建的评估指标
- **集成工具**：端到端流水线

## 评测框架

| 工具 | 类型 | 链接 | 描述 |
|------|------|------|------|
| **DeepEval** | 框架 | [![GitHub](https://img.shields.io/github/stars/confident-ai/deepeval.svg?style=social)](https://github.com/confident-ai/deepeval) | 支持自定义测试用例的LLM评测框架 |
| **t2v_metrics** | 库 | [![GitHub](https://img.shields.io/github/stars/linzhiqiu/t2v_metrics.svg?style=social)](https://github.com/linzhiqiu/t2v_metrics) | 文本到视频/图像评估指标 |

## 综述与全面回顾

| 论文 | 会议 | 链接 | 重点 |
|------|------|------|------|
| **A Survey of Automatic Evaluation Methods on Text, Visual and Speech Generations** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2506.10019-b31b1b.svg)](https://arxiv.org/abs/2506.10019) | 多模态评估综合调研 |
| **Evaluation and Benchmarking of LLM Agents: A Survey** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2507.21504-b31b1b.svg)](https://arxiv.org/abs/2507.21504) | Agent评测综合调研 |

## 商业工具

| 工具 | 类型 | 链接 | 描述 |
|------|------|------|------|
| **Prescene** | 商业 | [![Website](https://img.shields.io/badge/Website-prescene.ai-blue.svg)](https://www.prescene.ai/) | AI剧本分析与覆盖工具 |

## LLM-as-a-Judge范式

鉴于人工评估的高昂成本，主流方法是使用LLM作为评判者：

### 使用DeepEval实现

```python
from deepeval import evaluate
from deepeval.metrics import GEval

# 创建Judge Agent（如GPT-4o）作为"资深漫画主编"
judge_metric = GEval(
    name="manga_quality",
    criteria="评估生成的漫画面板的角色一致性和叙事连贯性",
    evaluation_params=["actual_output", "expected_output"]
)

# 运行评估
evaluate(test_cases, [judge_metric])
```

### 元评估
为确保Judge的可靠性：
1. 对比LLM评测结果与人类专家评分
2. 计算Pearson/Spearman相关性
3. 研究表明，设计精良的CoT提示可将对齐度提升34%以上

## 导航

- [← 上一章：听觉层](04-audio-layer.md)
- [→ 下一章：基准汇总](06-benchmarks-summary.md)
