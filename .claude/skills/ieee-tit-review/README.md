# IEEE TIT 论文评审 Skill

## 概述

这是一个专门用于评审 IEEE Transactions on Information Theory (IEEE TIT) 论文的 skill。包含完整的评审框架、检查清单、模板和示例。

## 目录结构

```
ieee-tit-review/
├── SKILL.md                           # 主 skill 文件（核心）
├── templates/                         # 模板文件
│   ├── review-report-template.md      # 评审报告模板
│   ├── decision-matrix.md             # 决策矩阵
│   ├── revision-checklist.md          # 修改检查清单
│   └── quality-checklist.md           # 评审报告质量检查清单 (v1.1.0 新增)
├── checklists/                        # 检查清单
│   ├── 0-quick-checklist.md           # 快速检查清单 (v1.1.0 新增)
│   ├── 1-structure.md                 # 结构完整性检查清单
│   ├── 2-symbols.md                   # 符号一致性检查清单
│   ├── 3-proofs.md                    # 证明逻辑检查清单（⭐核心）
│   ├── 4-experiments.md               # 实验可重复性检查清单
│   ├── 5-citations.md                 # 引用规范性检查清单
│   └── 6-ieee-tit-format.md           # IEEE TIT 格式检查清单
└── examples/                          # 示例评审报告
    ├── sample-review-accept.md        # Accept 示例 (v1.1.0 新增)
    ├── sample-review-minor.md         # Minor Revision 示例
    ├── sample-review-major.md         # Major Revision 示例 (v1.1.0 新增)
    └── sample-review-reject.md        # Reject 示例 (v1.1.0 新增)
```

## 核心特色

### 六大评审维度

1. **理论严谨性** (Theoretical Rigor) ⭐ TIT 核心要求
2. **数学证明完整性** (Mathematical Completeness) ⭐ TIT 核心要求
3. **创新性和贡献** (Novelty and Contribution) ⭐ TIT 核心要求
4. **实验验证** (Experimental Validation)
5. **文献综述质量** (Literature Review) ⭐ TIT 重要要求
6. **写作清晰度** (Writing Clarity) ⭐ TIT 重要要求

### 三级反馈结构

- **Major Issues** (必须解决): 影响论文正确性、完整性或可发表性
- **Minor Issues** (建议解决): 影响论文质量或可读性
- **Suggestions** (可选改进): 进一步提升论文质量

### 四阶段工作流程

1. **初步筛选** (30 分钟): 快速判断是否符合基本要求
2. **详细评审** (5-6 小时): 深入评审各个方面
3. **撰写报告** (1-2 小时): 生成结构化评审报告
4. **复审流程** (3-4 小时): 评估修订版

## 使用方法

### 快速开始

1. 阅读 `SKILL.md` 了解评审框架
2. 使用六个检查清单逐项检查论文
3. 使用 `review-report-template.md` 生成评审报告
4. 参考 `decision-matrix.md` 做出推荐决定

### 适用场景

✅ **适用**:
- 投稿 IEEE TIT 前的自查
- 作为评审人评审 IEEE TIT 投稿
- 指导学生撰写信息论论文
- 学习如何写高质量论文

❌ **不适用**:
- 非信息论领域的论文
- 会议论文（ISIT 等）
- 其他 IEEE 期刊（JSAC, Communications Letters）

## 文件说明

### 核心文件

- **SKILL.md**: 主 skill 文件，包含完整的评审框架、六大维度详细说明、工作流程等
- **review-report-template.md**: 中英双语评审报告模板，包含所有必需章节
- **decision-matrix.md**: 决策矩阵，帮助做出 Accept/Minor/Major/Reject 决定

### 检查清单

每个检查清单都是独立的，可以单独使用：

1. **1-structure.md**: 检查论文结构是否完整（章节、图表、参考文献等）
2. **2-symbols.md**: 检查符号系统是否一致（信息论符号、数学符号等）
3. **3-proofs.md**: 检查证明是否完整严格（⭐最重要，IEEE TIT 核心要求）
4. **4-experiments.md**: 检查实验是否可重复（如果有实验）
5. **5-citations.md**: 检查引用是否完整准确（文献综述、引用格式等）
6. **6-ieee-tit-format.md**: 检查格式是否符合 IEEE TIT 要求

### 示例

- **sample-review-minor.md**: 一个完整的 Minor Revision 评审报告示例，展示如何使用本 skill

## IEEE TIT 特色

本 skill 特别强调 IEEE TIT 的以下特色：

1. **理论深度优先**: 必须有显著的理论创新，不接受增量改进
2. **数学严谨性**: 所有定理必须有完整且严格的证明
3. **可读性要求**: 技术深度高，但必须对广泛读者清晰
4. **创新性判断**: 区分突破性贡献、显著贡献和增量贡献
5. **文献综述完整**: 必须引用开创性工作、最接近工作和最新进展

## 统计信息

- **总文件数**: 15 个 Markdown 文件
- **总大小**: 约 280 KB
- **总字数**: 约 85,000 字（中英双语）
- **检查清单项目**: 约 225+ 项
- **预计评审时间**:
  - 快速检查: 30-45 分钟
  - 详细评审: 6-8 小时

## 版本信息

- **版本**: v1.1.0
- **创建日期**: 2026-03-12
- **最后更新**: 2026-03-12
- **语言**: 中英双语
- **维护者**: Claude & User

## v1.1.0 更新内容

### 新增功能
1. **快速检查清单** (`checklists/0-quick-checklist.md`)
   - 25 个核心检查项
   - 适用于快速评审和初步筛选
   - 预计检查时间: 30-45 分钟

2. **多个示例评审报告**
   - Accept 决策示例
   - Major Revision 决策示例
   - Reject 决策示例
   - 覆盖所有决策场景

3. **评审报告质量检查清单** (`templates/quality-checklist.md`)
   - 10 个维度的质量检查
   - 确保评审报告符合标准
   - 包含质量评分系统

4. **详细的执行协议** (在 SKILL.md 中)
   - PDF 分阶段读取策略
   - 评审笔记组织策略
   - 报告生成流程
   - 质量自检流程
   - 工具使用优先级

5. **精确的触发条件** (在 SKILL.md 中)
   - 应该触发的场景
   - 不应该触发的场景
   - 需要确认的场景

### 改进内容
- 重构了使用流程，增加了详细的工具调用指导
- 明确了 AI 助手如何实际执行评审任务
- 改进了文档结构和可读性

## 使用建议

### 对于评审人

1. **首次使用**: 先阅读 `SKILL.md` 和 `sample-review-minor.md`，了解评审框架
2. **评审时**: 使用六个检查清单逐项检查，记录问题
3. **撰写报告**: 使用 `review-report-template.md` 生成报告
4. **做出决定**: 参考 `decision-matrix.md` 做出推荐决定

### 对于作者

1. **投稿前自查**: 使用六个检查清单自查论文
2. **收到评审意见后**: 使用 `revision-checklist.md` 系统地解决问题
3. **学习优秀论文**: 参考 `sample-review-minor.md` 了解评审人的期望

### 对于导师

1. **指导学生**: 使用本 skill 指导学生撰写和修改论文
2. **模拟评审**: 使用本 skill 对学生论文进行模拟评审
3. **培训**: 使用本 skill 培训学生如何评审论文

## 注意事项

1. **保密性**: 评审内容严格保密
2. **公平性**: 基于论文质量评审，不受作者身份影响
3. **建设性**: 即使拒绝，也提供建设性反馈
4. **专业性**: 保持专业和礼貌的态度
5. **一致性**: 对所有论文使用相同的标准

## 相关资源

- **IEEE TIT 主页**: https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=18
- **IEEE 作者中心**: https://www.ieee.org/publications/authors.html
- **IEEE 模板**: https://www.ieee.org/publications/authors/author-templates.html

## 反馈和改进

如果您在使用过程中发现问题或有改进建议，欢迎反馈。

---

**最后更新**: 2026-03-12
