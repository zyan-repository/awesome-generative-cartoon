# Contributing Guidelines

Thank you for your interest in contributing to Awesome Generative Cartoon!

## How to Add a New Paper

### 1. Required Information

Each paper entry requires:

| Field | Required | Example |
|-------|----------|---------|
| Paper Title | Yes | AgentBench |
| Venue/Year | Yes | ICLR 2024 |
| arXiv/Paper Link | Yes | arxiv.org/abs/2308.03688 |
| Code Repository | If available | github.com/THUDM/AgentBench |
| Key Metrics | Recommended | Success Rate, Pass@k |
| Layer Category | Yes | Cognitive / Narrative / Visual / Audio / System |

### 2. Entry Format

Use the table format with shields.io badges:

```markdown
| **Paper Name** | Venue Year | [![arXiv](https://img.shields.io/badge/arXiv-XXXX.XXXXX-b31b1b.svg)](https://arxiv.org/abs/XXXX.XXXXX) [![GitHub](https://img.shields.io/github/stars/org/repo.svg?style=social)](https://github.com/org/repo) | Key contribution description |
```

### 3. Steps to Contribute

1. Fork the repository
2. Add paper entry to appropriate `docs/*.md` file
3. Update `CHANGELOG.md`
4. Submit a Pull Request

## Bilingual Requirements

All documentation in `docs/` folder must be bilingual:
- English section first
- Horizontal rule separator (`---`)
- Chinese section below

Example:
```markdown
# Paper Category

[English content...]

---

# 论文分类

[Chinese content...]
```

## Code of Conduct

- Be respectful and inclusive
- Provide accurate paper information
- Link to official sources only

## Questions?

Open an issue if you have questions about contributing.

---

# 贡献指南

感谢您有兴趣为 Awesome Generative Cartoon 做贡献！

## 如何添加新论文

### 1. 必填信息

每个论文条目需要：

| 字段 | 是否必填 | 示例 |
|------|----------|------|
| 论文标题 | 是 | AgentBench |
| 会议/年份 | 是 | ICLR 2024 |
| arXiv/论文链接 | 是 | arxiv.org/abs/2308.03688 |
| 代码仓库 | 如有 | github.com/THUDM/AgentBench |
| 核心指标 | 建议 | 成功率, Pass@k |
| 层级分类 | 是 | 认知层 / 叙事层 / 视觉层 / 听觉层 / 系统层 |

### 2. 条目格式

使用带 shields.io 徽章的表格格式：

```markdown
| **论文名称** | 会议 年份 | [![arXiv](https://img.shields.io/badge/arXiv-XXXX.XXXXX-b31b1b.svg)](https://arxiv.org/abs/XXXX.XXXXX) [![GitHub](https://img.shields.io/github/stars/org/repo.svg?style=social)](https://github.com/org/repo) | 核心贡献描述 |
```

### 3. 贡献步骤

1. Fork 仓库
2. 将论文条目添加到相应的 `docs/*.md` 文件
3. 更新 `CHANGELOG.md`
4. 提交 Pull Request

## 双语要求

`docs/` 文件夹中的所有文档必须是双语的：
- 英文部分在前
- 水平分隔线（`---`）
- 中文部分在下

示例：
```markdown
# Paper Category

[English content...]

---

# 论文分类

[Chinese content...]
```

## 行为准则

- 尊重和包容
- 提供准确的论文信息
- 仅链接到官方来源

## 有问题？

如果您有关于贡献的问题，请开一个 issue。

---

# Private Rules / 私人规则

> **Note:** These rules are for repository maintainers only.
> **注意：** 这些规则仅供仓库维护者使用。

## Rule 1: Language Policy / 语言策略

| Location / 位置 | Language / 语言 |
|-----------------|-----------------|
| `README.md`, `README_CN.md` | Bilingual (EN default) / 双语（默认英文） |
| `docs/*.md` | Bilingual (EN first, CN after ---) / 双语（英文在前，中文在---之后） |
| `papers/` folder | **Chinese only / 仅中文** |
| User interaction / 用户交互 | **Chinese only / 仅中文** |

## Rule 2: Paper Sync Policy / 论文同步策略

When adding new papers / 添加新论文时：
1. Add entry to appropriate `docs/*.md` file / 添加条目到相应的 `docs/*.md` 文件
2. **Must** sync PDF to corresponding `papers/` subfolder / **必须**同步 PDF 到对应的 `papers/` 子文件夹
3. Create appropriate subfolder if it doesn't exist / 如不存在，创建合适的子文件夹
4. Update `CHANGELOG.md` / 更新 `CHANGELOG.md`

## Rule 3: PDF Naming Convention / PDF 命名规范

Format / 格式: `[年份]_[会议]_[论文简名].pdf`

Examples / 示例:
- `2024_ICLR_AgentBench.pdf`
- `2025_arXiv_ViStoryBench.pdf`
- `2023_NeurIPS_StoryBench.pdf`

## Rule 4: Commit Message Policy / 提交信息策略

**Do NOT include co-author in commit messages / 提交信息中不要包含共同作者**

Bad / 错误:
```
Add new paper

Co-Authored-By: xxx
```

Good / 正确:
```
Add new paper: ViStoryBench for story visualization
```

## Rule 5: Archive Policy / 归档策略

Papers older than 1 year from the current date are automatically archived.
距今超过1年的论文会自动归档。

| Scope / 范围 | Policy / 策略 |
|--------------|---------------|
| Main README | Only 2025-2026 papers / 仅显示2025-2026年论文 |
| Archive location / 归档位置 | `docs/archived-papers.md` |
| Archive format / 归档格式 | Same table format / 保持相同表格格式 |

When archiving / 归档时:
1. Move paper entry from main README to `docs/archived-papers.md` / 将论文条目从主README移至归档
2. Keep the same table format with badges / 保持相同的徽章表格格式
3. Organize by layer category / 按层级分类组织
