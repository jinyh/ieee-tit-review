# IEEE TIT Review Skill

一个专业的 IEEE Transactions on Information Theory (IEEE TIT) 论文评审工具，提供完整的评审框架、检查清单和模板。

[English](#english) | [中文](#中文)

---

## 中文

### 概述

这是一个专门用于评审 IEEE Transactions on Information Theory (IEEE TIT) 论文的 Claude Code Skill。包含完整的评审框架、详细的检查清单、评审报告模板和示例。

### 核心特色

#### 六大评审维度
1. **理论严谨性** (Theoretical Rigor) ⭐ TIT 核心要求
2. **数学证明完整性** (Mathematical Completeness) ⭐ TIT 核心要求
3. **创新性和贡献** (Novelty and Contribution) ⭐ TIT 核心要求
4. **实验验证** (Experimental Validation)
5. **文献综述质量** (Literature Review) ⭐ TIT 重要要求
6. **写作清晰度** (Writing Clarity) ⭐ TIT 重要要求

#### 三级反馈结构
- **Major Issues** (必须解决): 影响论文正确性、完整性或可发表性
- **Minor Issues** (建议解决): 影响论文质量或可读性
- **Suggestions** (可选改进): 进一步提升论文质量

#### 四阶段工作流程
1. **初步筛选**: 快速判断是否符合基本要求
2. **详细评审**: 深入评审各个方面
3. **撰写报告**: 生成结构化评审报告
4. **复审流程**: 评估修订版

### 目录结构

```
.claude/skills/ieee-tit-review/
├── SKILL.md                           # 主 skill 文件（核心）
├── README.md                          # 说明文档
├── IMPLEMENTATION.md                  # 实现报告
├── templates/                         # 模板文件
│   ├── review-report-template.md      # 评审报告模板
│   ├── decision-matrix.md             # 决策矩阵
│   ├── revision-checklist.md          # 修改检查清单
│   └── quality-checklist.md           # 评审报告质量检查清单
├── checklists/                        # 检查清单
│   ├── 0-quick-checklist.md           # 快速检查清单 (25 项)
│   ├── 1-structure.md                 # 结构完整性检查清单
│   ├── 2-symbols.md                   # 符号一致性检查清单
│   ├── 3-proofs.md                    # 证明逻辑检查清单（⭐核心）
│   ├── 4-experiments.md               # 实验可重复性检查清单
│   ├── 5-citations.md                 # 引用规范性检查清单
│   └── 6-ieee-tit-format.md           # IEEE TIT 格式检查清单
└── examples/                          # 示例评审报告
    ├── sample-review-accept.md        # Accept 示例
    ├── sample-review-minor.md         # Minor Revision 示例
    ├── sample-review-major.md         # Major Revision 示例
    └── sample-review-reject.md        # Reject 示例
```

### 使用方法

#### 在 Claude Code 中使用

1. 将此 skill 放置在 `.claude/skills/ieee-tit-review/` 目录
2. 当需要评审论文时，说"请评审这篇 IEEE TIT 论文"
3. Skill 会自动触发，引导你完成评审流程

#### 适用场景

✅ **适用**:
- 投稿 IEEE TIT 前的自查
- 作为评审人评审 IEEE TIT 投稿
- 指导学生撰写信息论论文
- 学习如何写高质量论文

❌ **不适用**:
- 非信息论领域的论文
- 会议论文（ISIT 等）
- 其他 IEEE 期刊（JSAC, Communications Letters）

### 统计信息

- **总文件数**: 16 个 Markdown 文件
- **总大小**: 约 280 KB
- **总字数**: 约 85,000 字（中英双语）
- **检查清单项目**: 465+ 项
- **评审模式**:
  - 快速评审: 25 项核心检查
  - 标准评审: 465+ 项完整检查

### 版本信息

- **当前版本**: v1.2.0
- **创建日期**: 2026-03-12
- **最后更新**: 2026-03-12
- **语言**: 中英双语
- **维护者**: Claude & User

### v1.1.0 更新内容

**新增功能**:
1. 快速检查清单（25 个核心检查项）
2. 多个示例评审报告（Accept、Major、Reject）
3. 评审报告质量检查清单
4. 详细的执行协议（6 个协议）
5. 精确的触发条件说明

**改进内容**:
- 重构了使用流程，增加了详细的工具调用指导
- 明确了 AI 助手如何实际执行评审任务
- 改进了文档结构和可读性

### IEEE TIT 特色

本 skill 特别强调 IEEE TIT 的以下特色：

1. **理论深度优先**: 必须有显著的理论创新，不接受增量改进
2. **数学严谨性**: 所有定理必须有完整且严格的证明
3. **可读性要求**: 技术深度高，但必须对广泛读者清晰
4. **创新性判断**: 区分突破性贡献、显著贡献和增量贡献
5. **文献综述完整**: 必须引用开创性工作、最接近工作和最新进展

### 许可证

MIT License

### 贡献

欢迎提交 Issue 和 Pull Request！

---

## English

### Overview

A professional review tool for IEEE Transactions on Information Theory (IEEE TIT) papers, providing a complete review framework, checklists, and templates.

### Key Features

#### Six Review Dimensions
1. **Theoretical Rigor** ⭐ Core TIT requirement
2. **Mathematical Completeness** ⭐ Core TIT requirement
3. **Novelty and Contribution** ⭐ Core TIT requirement
4. **Experimental Validation**
5. **Literature Review** ⭐ Important TIT requirement
6. **Writing Clarity** ⭐ Important TIT requirement

#### Three-Level Feedback Structure
- **Major Issues** (must fix): Affect correctness, completeness, or publishability
- **Minor Issues** (should fix): Affect quality or readability
- **Suggestions** (optional): Further improvements

#### Four-Stage Workflow
1. **Initial Screening**: Quick assessment
2. **Detailed Review**: In-depth evaluation
3. **Report Writing**: Generate structured report
4. **Re-review**: Evaluate revised version

### Usage

#### In Claude Code

1. Place this skill in `.claude/skills/ieee-tit-review/`
2. Say "Please review this IEEE TIT paper"
3. The skill will automatically trigger and guide you through the review process

#### Applicable Scenarios

✅ **Suitable for**:
- Self-check before submitting to IEEE TIT
- Peer review for IEEE TIT submissions
- Guiding students in writing information theory papers
- Learning how to write high-quality papers

❌ **Not suitable for**:
- Papers outside information theory
- Conference papers (ISIT, etc.)
- Other IEEE journals (JSAC, Communications Letters)

### Statistics

- **Total files**: 16 Markdown files
- **Total size**: ~280 KB
- **Total words**: ~85,000 words (bilingual)
- **Checklist items**: 465+ items
- **Review modes**:
  - Quick review: 25 core checks
  - Standard review: 465+ full checks

### Version

- **Current version**: v1.2.0
- **Created**: 2026-03-12
- **Last updated**: 2026-03-12
- **Language**: Chinese-English bilingual
- **Maintainer**: Claude & User

### License

MIT License

### Contributing

Issues and Pull Requests are welcome!

---

**Repository**: https://github.com/[username]/ieee-tit-review
**Documentation**: See `.claude/skills/ieee-tit-review/README.md` for detailed usage
