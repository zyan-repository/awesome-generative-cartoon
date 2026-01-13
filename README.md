# Awesome Generative Cartoon [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of papers, benchmarks, and tools for multi-agent comic/animation generation systems.

[![中文版](https://img.shields.io/badge/中文-README-blue.svg)](README_CN.md)
[![Last Updated](https://img.shields.io/badge/Last%20Updated-2025--01-green.svg)]()
[![Papers](https://img.shields.io/badge/Papers-57+-orange.svg)]()
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

## Overview

This repository organizes research on **multi-agent systems for comic and animation generation**, following the **Full-Stack Evaluation Model** framework. The model divides evaluation into four hierarchical layers:

```
┌─────────────────────────────────────────────────────────────┐
│                     System Layer                            │
│              Evaluation Toolkits & Integration              │
├─────────────────────────────────────────────────────────────┤
│                   Presentation Layer                        │
│    ┌────────────────────┬────────────────────┐              │
│    │    Visual          │      Audio         │              │
│    │  • Story Viz       │  • TTS/Voice       │              │
│    │  • Character ID    │  • Music/BGM       │              │
│    │  • Video Quality   │  • Lip Sync        │              │
│    └────────────────────┴────────────────────┘              │
├─────────────────────────────────────────────────────────────┤
│                    Narrative Layer                          │
│           Story Logic • Screenplay • Dialogue               │
├─────────────────────────────────────────────────────────────┤
│                    Cognitive Layer                          │
│        Agent Intelligence • Multi-Agent Coordination        │
└─────────────────────────────────────────────────────────────┘
```

## Table of Contents

- [Cognitive Layer](#cognitive-layer) - Agent intelligence and coordination
- [Narrative Layer](#narrative-layer) - Story logic and screenplay
- [Visual Layer](#visual-layer) - Character consistency and video generation
- [Audio Layer](#audio-layer) - TTS, music, and lip-sync
- [System Layer](#system-layer) - Evaluation toolkits and integration
- [Documentation](#documentation)
- [Contributing](#contributing)

## Cognitive Layer

Benchmarks and papers for evaluating agent capabilities, role-playing fidelity, and multi-agent coordination.

> **Note:** Only papers from 2025-2026 are shown. Papers from 2024 and earlier are in the [archive](docs/archived-papers.md).

| Paper | Venue | Links | Key Contribution |
|-------|-------|-------|------------------|
| **MultiAgentBench** | ACL 2025 | [![Paper](https://img.shields.io/badge/ACL-2025-blue.svg)](https://aclanthology.org/2025.acl-long.421.pdf) | Collaboration Score, multi-agent coordination |
| **StoryWriter** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2506.16445-b31b1b.svg)](https://arxiv.org/abs/2506.16445) | Multi-agent long story generation framework |
| **RolePlayEval** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2505.13157-b31b1b.svg)](https://arxiv.org/abs/2505.13157) | In-Character Consistency (ICC) metric |
| **GEMMAS** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2507.13190-b31b1b.svg)](https://arxiv.org/abs/2507.13190) | Graph-based multi-agent evaluation |

📚 [Full list →](docs/01-cognitive-layer.md) | 📦 [Archived papers →](docs/archived-papers.md)

## Narrative Layer

Benchmarks for story coherence, screenplay format, and plot logic evaluation.

> **Note:** Only papers from 2025-2026 are shown. Papers from 2024 and earlier are in the [archive](docs/archived-papers.md).

| Paper | Venue | Links | Key Contribution |
|-------|-------|-------|------------------|
| **SCORE** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2503.23512-b31b1b.svg)](https://arxiv.org/abs/2503.23512) | Dynamic state tracking, logic consistency |
| **Narrative Planning** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2506.10161-b31b1b.svg)](https://arxiv.org/abs/2506.10161) | LLM story generation via planning |
| **DSR** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2510.23163-b31b1b.svg)](https://arxiv.org/abs/2510.23163) | Decomposed screenwriting approach |
| **ETVA** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2503.16867-b31b1b.svg)](https://arxiv.org/abs/2503.16867) | Fine-grained QA-based alignment |

📚 [Full list →](docs/02-narrative-layer.md) | 📦 [Archived papers →](docs/archived-papers.md)

## Visual Layer

Benchmarks for character consistency, text-image alignment, and video quality.

> **Note:** Only papers from 2025-2026 are shown. Papers from 2024 and earlier are in the [archive](docs/archived-papers.md).

| Paper | Venue | Links | Key Contribution |
|-------|-------|-------|------------------|
| **ViStoryBench** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2505.24862-b31b1b.svg)](https://arxiv.org/abs/2505.24862) | CIDS, OCCM metrics for story visualization |
| **CharaConsist** | ICCV 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2507.11533-b31b1b.svg)](https://arxiv.org/abs/2507.11533) | Fine-grained character consistency |
| **VBench-2.0** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2503.21755-b31b1b.svg)](https://arxiv.org/abs/2503.21755) | Physics realism, creative composition |
| **T2V-CompBench** | CVPR 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2407.14505-b31b1b.svg)](https://arxiv.org/abs/2407.14505) | Compositional T2V, 1400 prompts |
| **JEDi** | ICLR 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2410.05203-b31b1b.svg)](https://arxiv.org/abs/2410.05203) | JEPA embedding distance for video |

📚 [Full list →](docs/03-visual-layer.md) | 📦 [Archived papers →](docs/archived-papers.md)

## Audio Layer

Benchmarks for TTS expressiveness, music generation, and lip-sync quality.

> **Note:** Only papers from 2025-2026 are shown. Papers from 2024 and earlier are in the [archive](docs/archived-papers.md).

| Paper | Venue | Links | Key Contribution |
|-------|-------|-------|------------------|
| **EmergentTTS-Eval** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2505.23009-b31b1b.svg)](https://arxiv.org/abs/2505.23009) | Paralinguistic accuracy, emotional TTS |
| **EmoSSLSphere** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2508.11273-b31b1b.svg)](https://arxiv.org/abs/2508.11273) | Multilingual emotional TTS |
| **OmniSync** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2505.21448-b31b1b.svg)](https://arxiv.org/abs/2505.21448) | Universal lip-sync, AIGC-LipSync benchmark |
| **MusicEval** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2501.10811-b31b1b.svg)](https://arxiv.org/abs/2501.10811) | Expert ratings for music generation |
| **SongEval** | arXiv 2025 | [![arXiv](https://img.shields.io/badge/arXiv-2505.10793-b31b1b.svg)](https://arxiv.org/abs/2505.10793) | Song aesthetics benchmark |

📚 [Full list →](docs/04-audio-layer.md) | 📦 [Archived papers →](docs/archived-papers.md)

## System Layer

Evaluation toolkits and integration frameworks.

| Tool | Type | Links | Description |
|------|------|-------|-------------|
| **DeepEval** | Framework | [![GitHub](https://img.shields.io/github/stars/confident-ai/deepeval.svg?style=social)](https://github.com/confident-ai/deepeval) | LLM evaluation framework |
| **t2v_metrics** | Library | [![GitHub](https://img.shields.io/github/stars/linzhiqiu/t2v_metrics.svg?style=social)](https://github.com/linzhiqiu/t2v_metrics) | Text-to-video/image metrics |
| **Prescene** | Commercial | [![Website](https://img.shields.io/badge/Website-prescene.ai-blue.svg)](https://www.prescene.ai/) | AI for screenplays |

📚 [Full list →](docs/05-system-layer.md) | 📦 [Archived papers →](docs/archived-papers.md)

## Documentation

| Document | Description |
|----------|-------------|
| [Full-Stack Overview](docs/00-full-stack-overview.md) | Framework explanation and evaluation dimensions |
| [Cognitive Layer](docs/01-cognitive-layer.md) | Agent intelligence papers |
| [Narrative Layer](docs/02-narrative-layer.md) | Story and screenplay papers |
| [Visual Layer](docs/03-visual-layer.md) | Visual generation papers |
| [Audio Layer](docs/04-audio-layer.md) | Audio generation papers |
| [System Layer](docs/05-system-layer.md) | Evaluation toolkits |
| [Benchmarks Summary](docs/06-benchmarks-summary.md) | Quick reference table |

## Contributing

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details on:
- How to add new papers
- Required metadata fields
- Paper naming conventions

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

This repository is inspired by the research report "多Agent驱动的有声漫画与动画生成系统：全栈评估与Benchmark体系构建研究报告" which provides a comprehensive framework for evaluating multi-agent comic and animation generation systems.

---

**Star this repo** if you find it useful! ⭐
