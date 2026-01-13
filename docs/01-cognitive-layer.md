# Cognitive Layer Papers

Papers on agent intelligence, multi-agent coordination, and role-playing evaluation.

## Overview

The cognitive layer evaluates the "brain" of the multi-agent system:
- **Single Agent Capability**: Tool use, memory, reasoning
- **Multi-Agent Coordination**: Collaboration, communication efficiency
- **Role-Playing Fidelity**: Persona consistency, in-character behavior

## Single Agent Capability

| Paper | Venue | Links | Key Metrics | Notes |
|-------|-------|-------|-------------|-------|
| **AgentBench: Evaluating LLMs as Agents** | ICLR 2024 | [![arXiv](https://img.shields.io/badge/arXiv-2308.03688-b31b1b.svg)](https://arxiv.org/abs/2308.03688) [![GitHub](https://img.shields.io/github/stars/THUDM/AgentBench.svg?style=social)](https://github.com/THUDM/AgentBench) | Success Rate, Pass@k | 8 environments: OS, DB, KG, etc. |
| **AgentArch: A Comprehensive Benchmark to Evaluate Agent Architectures** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2509.10769-b31b1b.svg)](https://arxiv.org/abs/2509.10769) | Architecture Score | Enterprise agent architecture evaluation |
| **Evaluation and Benchmarking of LLM Agents: A Survey** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2507.21504-b31b1b.svg)](https://arxiv.org/abs/2507.21504) | Survey | Comprehensive agent evaluation survey |

## Multi-Agent Coordination

| Paper | Venue | Links | Key Metrics | Notes |
|-------|-------|-------|-------------|-------|
| **MultiAgentBench: Evaluating the Collaboration and Competition of LLM agents** | ACL 2025 | [![Paper](https://img.shields.io/badge/ACL-2025-blue.svg)](https://aclanthology.org/2025.acl-long.421.pdf) | Collaboration Score, UPR | MARBLE framework for coordination |
| **GEMMAS: Graph-based Evaluation Metrics for Multi Agent Systems** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2507.13190-b31b1b.svg)](https://arxiv.org/abs/2507.13190) | Information Diversity Score (IDS), Unnecessary Path Ratio | Graph-theory based evaluation |
| **StoryWriter: A Multi-Agent Framework for Long Story Generation** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2506.16445-b31b1b.svg)](https://arxiv.org/abs/2506.16445) | Story Quality, Length | Outline + Planning + Writing agents |
| **CreAgentive: An Agent Workflow Driven Multi-Category Creative Generation Engine** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2509.26461-b31b1b.svg)](https://arxiv.org/abs/2509.26461) | Creativity Score | Multi-category creative generation |

## Role-Playing Evaluation

| Paper | Venue | Links | Key Metrics | Notes |
|-------|-------|-------|-------------|-------|
| **RoleAgent: Building, Interacting, and Benchmarking High-quality Role-Playing Agents from Scripts** | NeurIPS 2024 | [![Paper](https://img.shields.io/badge/NeurIPS-2024-purple.svg)](https://proceedings.neurips.cc/paper_files/paper/2024/file/5875aca1ef70285a35940afbbce0f9fb-Paper-Datasets_and_Benchmarks_Track.pdf) | Role consistency | Building agents from scripts |
| **Role-Playing Evaluation for Large Language Models** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2505.13157-b31b1b.svg)](https://arxiv.org/abs/2505.13157) | ICC, Emotional Understanding, Decision-Making, Moral Alignment | 4-dimension evaluation |
| **PersonaEval: Benchmarking LLMs on Role-Playing Evaluation Tasks** | OpenReview | [![OpenReview](https://img.shields.io/badge/OpenReview-2024-green.svg)](https://openreview.net/forum?id=wZbkQStAXj) | Classification-based | Judge model approach |

## Key Concepts

### Success Rate (SR)
Percentage of tasks completed successfully by the agent.

### Pass@k
Probability of generating at least one correct solution within k attempts.

### Collaboration Score (CS)
Ratio of task completion to communication cost:
```
CS = TaskCompletion / CommunicationCost
```

### In-Character Consistency (ICC)
Measures whether an agent maintains its assigned persona without breaking character.

## Navigation

- [← Back to Overview](00-full-stack-overview.md)
- [→ Next: Narrative Layer](02-narrative-layer.md)

---

# 认知层论文

Agent智能、多Agent协作与角色扮演评估相关论文。

## 概述

认知层评估多Agent系统的"大脑"：
- **单体Agent能力**：工具使用、记忆、推理
- **多Agent协作**：协作效率、沟通质量
- **角色扮演保真度**：人格一致性、角色内行为

## 单体Agent能力

| 论文 | 会议 | 链接 | 核心指标 | 备注 |
|------|------|------|----------|------|
| **AgentBench: Evaluating LLMs as Agents** | ICLR 2024 | [![arXiv](https://img.shields.io/badge/arXiv-2308.03688-b31b1b.svg)](https://arxiv.org/abs/2308.03688) [![GitHub](https://img.shields.io/github/stars/THUDM/AgentBench.svg?style=social)](https://github.com/THUDM/AgentBench) | 成功率, Pass@k | 8种环境：OS、DB、KG等 |
| **AgentArch: A Comprehensive Benchmark to Evaluate Agent Architectures** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2509.10769-b31b1b.svg)](https://arxiv.org/abs/2509.10769) | 架构评分 | 企业级Agent架构评估 |
| **Evaluation and Benchmarking of LLM Agents: A Survey** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2507.21504-b31b1b.svg)](https://arxiv.org/abs/2507.21504) | 综述 | Agent评测综合调研 |

## 多Agent协作

| 论文 | 会议 | 链接 | 核心指标 | 备注 |
|------|------|------|----------|------|
| **MultiAgentBench: Evaluating the Collaboration and Competition of LLM agents** | ACL 2025 | [![Paper](https://img.shields.io/badge/ACL-2025-blue.svg)](https://aclanthology.org/2025.acl-long.421.pdf) | 协作评分, UPR | MARBLE协作框架 |
| **GEMMAS: Graph-based Evaluation Metrics for Multi Agent Systems** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2507.13190-b31b1b.svg)](https://arxiv.org/abs/2507.13190) | 信息多样性得分(IDS), 非必要路径比率 | 基于图论的评估 |
| **StoryWriter: A Multi-Agent Framework for Long Story Generation** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2506.16445-b31b1b.svg)](https://arxiv.org/abs/2506.16445) | 故事质量, 长度 | 大纲+规划+写作多Agent框架 |
| **CreAgentive: An Agent Workflow Driven Multi-Category Creative Generation Engine** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2509.26461-b31b1b.svg)](https://arxiv.org/abs/2509.26461) | 创意评分 | 多类别创意生成引擎 |

## 角色扮演评估

| 论文 | 会议 | 链接 | 核心指标 | 备注 |
|------|------|------|----------|------|
| **RoleAgent: Building, Interacting, and Benchmarking High-quality Role-Playing Agents from Scripts** | NeurIPS 2024 | [![Paper](https://img.shields.io/badge/NeurIPS-2024-purple.svg)](https://proceedings.neurips.cc/paper_files/paper/2024/file/5875aca1ef70285a35940afbbce0f9fb-Paper-Datasets_and_Benchmarks_Track.pdf) | 角色一致性 | 从剧本构建Agent |
| **Role-Playing Evaluation for Large Language Models** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2505.13157-b31b1b.svg)](https://arxiv.org/abs/2505.13157) | ICC, 情感理解, 决策一致性, 道德对齐 | 4维度评估 |
| **PersonaEval: Benchmarking LLMs on Role-Playing Evaluation Tasks** | OpenReview | [![OpenReview](https://img.shields.io/badge/OpenReview-2024-green.svg)](https://openreview.net/forum?id=wZbkQStAXj) | 分类评估 | Judge模型方法 |

## 关键概念

### 成功率（SR）
Agent成功完成任务的百分比。

### Pass@k
在k次尝试内生成至少一个正确解的概率。

### 协作评分（CS）
任务完成度与通信成本的比值：
```
CS = 任务完成度 / 通信成本
```

### 角色内一致性（ICC）
衡量Agent是否在不破坏角色的情况下保持其分配的人格。

## 导航

- [← 返回概述](00-full-stack-overview.md)
- [→ 下一章：叙事层](02-narrative-layer.md)
