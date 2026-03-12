# 示例评审报告：Major Revision / Sample Review Report: Major Revision

## 论文信息 / Paper Information

- **标题 / Title**: On the Capacity of Wireless Networks with Cooperative Relaying
- **作者 / Authors**: David Lee and Emily Zhang
- **评审日期 / Review Date**: 2026-03-12
- **评审类型 / Review Type**: Initial Review
- **评审人 / Reviewer**: [匿名]

---

## 总体评价 / Overall Assessment

### 推荐决定 / Recommendation

- [ ] **Accept** (接受)
- [ ] **Minor Revision** (小修)
- [x] **Major Revision** (大修)
- [ ] **Reject** (拒绝)

### 置信度 / Confidence Level

- [x] **High** (高) - 我对该领域非常熟悉，对评审意见有高度信心
- [ ] **Medium** (中)
- [ ] **Low** (低)

### 总体评分 / Overall Score

**6.0/10**

### 各维度评分 / Dimension Scores

1. **理论严谨性 / Theoretical Rigor**: 5/10
2. **数学证明完整性 / Mathematical Completeness**: 5/10
3. **创新性和贡献 / Novelty and Contribution**: 7/10
4. **实验验证 / Experimental Validation**: 6/10
5. **文献综述质量 / Literature Review**: 5/10
6. **写作清晰度 / Writing Clarity**: 6/10

---

## 核心贡献总结 / Summary of Contributions

本文研究了具有协作中继的无线网络容量问题。主要贡献包括：(1) 提出了一种新的中继协作策略；(2) 推导了网络容量的上界和下界；(3) 通过数值实验验证了所提策略的性能。

**总体评价**: 论文研究的问题有意义，提出的协作策略有一定新颖性，但存在**多个严重问题**需要解决：
- 主定理的证明有逻辑漏洞
- 遗漏了重要的相关工作
- 与现有工作的对比不充分
- 符号系统不一致

这些问题影响了论文的正确性和可发表性，需要进行**大修 (Major Revision)**。

---

## 主要优点 / Main Strengths

### 1. 问题有意义
- ✅ 协作中继是无线网络中的重要问题
- ✅ 研究多中继场景具有实用价值

### 2. 有一定创新性
- ✅ 提出的协作策略与现有方法有区别
- ✅ 考虑了中继之间的干扰

### 3. 数值实验较全面
- ✅ 对比了多种基线方法
- ✅ 考虑了不同的网络拓扑

---

## Major Issues (必须解决)

### [M1] 理论严谨性 - Theorem 1 的证明有逻辑漏洞

- **位置 / Location**: Page 6, Theorem 1, Proof
- **问题描述 / Description**:
  - Theorem 1 声称推导了网络容量的上界，但证明中从 (15) 到 (16) 的推导有问题
  - 在 (15) 中，使用了 Fano 不等式：H(W|Y^n) ≤ nε_n
  - 但在 (16) 中，直接假设 ε_n → 0，这需要证明译码错误概率趋于 0
  - 然而，Theorem 1 的陈述中**没有假设译码错误概率趋于 0**
  - 这导致证明不完整

- **影响 / Impact**:
  - 这是论文的主要结果，证明不完整严重影响论文的正确性
  - 如果不能证明译码错误概率趋于 0，则上界可能不成立

- **改进建议 / Suggestions**:
  1. 在 Theorem 1 的陈述中明确假设：对于任何可达速率 R，存在码字序列使得译码错误概率 P_e^(n) → 0
  2. 或者，修改证明方法，不依赖 Fano 不等式，使用其他方法推导上界
  3. 参考 Cover-Thomas 教科书第 14 章关于多址接入信道容量证明的标准方法

### [M2] 数学证明完整性 - Lemma 2 的证明缺失

- **位置 / Location**: Page 8, Lemma 2
- **问题描述 / Description**:
  - Lemma 2 是 Theorem 2（容量下界）的关键引理
  - 但 Lemma 2 的证明标注为"Proof is given in Appendix A"
  - 然而，Appendix A 中**没有 Lemma 2 的证明**，只有 Lemma 3 的证明
  - 这导致 Theorem 2 的证明不完整

- **影响 / Impact**:
  - Theorem 2 是论文的主要结果之一，缺少关键引理的证明严重影响论文的可信度

- **改进建议 / Suggestions**:
  1. 在 Appendix A 中补充 Lemma 2 的完整证明
  2. 如果 Lemma 2 是已知结果，明确引用出处
  3. 如果 Lemma 2 的证明过长，可以提供证明思路和关键步骤

### [M3] 创新性和贡献 - 与现有工作的本质区别不清晰

- **位置 / Location**: Page 2, Section I-B (Related Work)
- **问题描述 / Description**:
  - 论文声称提出了"新的协作策略"，但与 [15] (Kramer 2005) 的 decode-and-forward 策略的**本质区别不清晰**
  - 在 Related Work 中，只是简单提到 [15]，但没有详细对比
  - 在 Section III-A 中，描述了所提策略，但没有说明与 [15] 的区别
  - 从描述来看，所提策略似乎是 decode-and-forward 的一个特例

- **影响 / Impact**:
  - 如果所提策略与 [15] 没有本质区别，则论文的创新性不足
  - 这可能导致论文不符合 IEEE TIT 的发表标准（要求显著的理论贡献）

- **改进建议 / Suggestions**:
  1. 在 Related Work 中增加一个表格，详细对比本文策略与 [15] 的区别
  2. 明确说明本文策略在哪些方面改进了 [15]（如适用范围、性能、复杂度）
  3. 如果本文策略确实是 [15] 的特例，需要说明为什么这个特例值得研究（如在某些场景下性能更优）
  4. 提供理论分析或数值实验，证明本文策略在某些场景下严格优于 [15]

### [M4] 文献综述质量 - 遗漏重要相关工作

- **位置 / Location**: Page 2, Section I-B (Related Work)
- **问题描述 / Description**:
  - 论文遗漏了以下重要相关工作：
    1. **Cover-El Gamal 1979**: 中继信道的开创性工作，必须引用
    2. **Xie-Kumar 2005**: 多中继网络容量的经典结果
    3. **Avestimehr-Diggavi-Tse 2011**: 确定性模型，与本文的系统模型相关
  - 这些文献是中继网络研究的基础，遗漏它们严重影响文献综述的完整性

- **影响 / Impact**:
  - 遗漏开创性工作和重要相关工作是严重问题
  - 可能导致评审人质疑作者对该领域的了解程度

- **改进建议 / Suggestions**:
  1. 补充引用上述三篇文献
  2. 在 Related Work 中增加一段，系统梳理中继网络容量研究的发展历史
  3. 明确说明本文与这些经典工作的关系

### [M5] 写作清晰度 - 符号系统不一致

- **位置 / Location**: 全文
- **问题描述 / Description**:
  - 符号 h_i 在不同地方有不同含义：
    - Page 4, (3): h_i 表示信道增益
    - Page 7, (12): h_i 表示信道系数（复数）
    - Page 10, Figure 2: h_i 表示信道功率增益 |h_i|^2
  - 符号 R 的含义也不一致：
    - Page 5, Theorem 1: R 表示速率（bits per channel use）
    - Page 9, (18): R 表示速率区域（rate region）

- **影响 / Impact**:
  - 符号不一致严重影响论文的可读性
  - 可能导致读者误解论文的结果

- **改进建议 / Suggestions**:
  1. 统一符号系统：h_i 统一表示信道系数（复数），|h_i|^2 表示功率增益
  2. 使用不同符号表示不同概念：R 表示速率，C 表示容量，R 表示速率区域
  3. 在 Section II 增加一个符号表（Notation Table），列出所有符号及其含义
  4. 全文检查符号使用，确保一致性

---

## Minor Issues (建议解决)

### [m1] 理论严谨性 - 假设条件不够明确

- **位置 / Location**: Page 5, Theorem 1
- **问题描述 / Description**: Theorem 1 假设"信道是遍历的"，但没有明确定义什么是"遍历信道"
- **改进建议 / Suggestions**: 在 Theorem 1 前增加一个 Definition，明确定义"遍历信道"

### [m2] 数学证明完整性 - 证明步骤跳步

- **位置 / Location**: Page 7, equation (12) to (13)
- **问题描述 / Description**: 从 (12) 到 (13) 使用了 Jensen 不等式，但跳步较多
- **改进建议 / Suggestions**: 补充中间步骤，说明如何应用 Jensen 不等式

### [m3] 实验验证 - 缺少误差棒

- **位置 / Location**: Page 11, Figure 3
- **问题描述 / Description**: Figure 3 展示了数值实验结果，但没有误差棒（error bars）
- **改进建议 / Suggestions**: 增加误差棒，说明实验的统计显著性

### [m4] 文献综述质量 - 引用格式不统一

- **位置 / Location**: 参考文献
- **问题描述 / Description**: 部分引用格式不符合 IEEE 标准（如 [8], [12], [20]）
- **改进建议 / Suggestions**: 统一引用格式，符合 IEEE Transactions 标准

### [m5] 写作清晰度 - 图表说明不够详细

- **位置 / Location**: Page 10, Figure 2
- **问题描述 / Description**: Figure 2 的 caption 过于简短，没有说明横纵坐标的含义和实验设置
- **改进建议 / Suggestions**: 增加详细的 caption，说明实验参数和图表含义

---

## Suggestions (可选改进)

### [S1] 增加理论分析

- **位置 / Location**: Section IV (Numerical Results)
- **建议 / Suggestion**: 建议在数值实验部分增加理论分析，解释为什么所提策略在某些场景下性能更优

### [S2] 增加复杂度分析

- **位置 / Location**: Section III
- **建议 / Suggestion**: 建议增加所提策略的计算复杂度分析，与现有方法对比

### [S3] 增加讨论部分

- **位置 / Location**: Section V (Conclusion)
- **建议 / Suggestion**: 建议在结论前增加一个 Discussion 部分，讨论所提方法的局限性和未来研究方向

---

## 修改建议优先级 / Revision Priority

### 高优先级 (必须修改)
1. **[M1]** 修正 Theorem 1 的证明逻辑漏洞
2. **[M2]** 补充 Lemma 2 的证明
3. **[M3]** 明确与现有工作的本质区别
4. **[M4]** 补充遗漏的重要相关工作
5. **[M5]** 统一符号系统

### 中优先级 (建议修改)
1. [m1] 明确假设条件的定义
2. [m2] 补充证明的中间步骤
3. [m3] 增加实验误差棒
4. [m4] 统一引用格式
5. [m5] 改进图表说明

### 低优先级 (可选修改)
1. [S1] 增加理论分析
2. [S2] 增加复杂度分析
3. [S3] 增加讨论部分

---

## 给作者的总体建议 / Overall Suggestions for Authors

论文研究的问题有意义，提出的协作策略有一定新颖性，但存在**多个严重问题**需要解决：

### 关键问题
1. **证明完整性**: Theorem 1 的证明有逻辑漏洞，Lemma 2 的证明缺失
2. **创新性说明**: 与现有工作（特别是 [15] Kramer 2005）的本质区别不清晰
3. **文献综述**: 遗漏了重要的开创性工作和相关文献
4. **符号一致性**: 符号系统不一致，严重影响可读性

### 修改建议
1. **优先解决 Major Issues**: 这些问题影响论文的正确性和可发表性，必须在修订版中解决
2. **加强理论分析**: 补充完整的证明，明确假设条件
3. **完善文献综述**: 补充遗漏的重要文献，详细对比与现有工作的区别
4. **统一符号系统**: 全文检查符号使用，确保一致性
5. **改进写作质量**: 增加详细的图表说明，补充中间推导步骤

### 鼓励的话
尽管存在上述问题，但论文的核心思想是有价值的。如果作者能够认真解决这些问题，论文有潜力成为一篇高质量的理论论文。

**建议大修后重审 (Major Revision)**。

---

## 给编辑的意见 / Comments to Editor

论文研究的问题有意义，但存在多个严重问题：
1. 主定理的证明有逻辑漏洞
2. 关键引理的证明缺失
3. 遗漏了重要的相关工作
4. 符号系统不一致

这些问题影响了论文的正确性和可发表性。建议要求作者进行大修，解决上述问题后重新评审。

如果作者能够认真解决这些问题，论文有潜力达到 IEEE TIT 的发表标准。

---

**评审完成日期 / Review Completed**: 2026-03-12
**评审人签名 / Reviewer Signature**: [匿名]
