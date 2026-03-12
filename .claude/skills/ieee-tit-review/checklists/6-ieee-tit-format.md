# IEEE TIT 格式检查清单 / IEEE TIT Format Checklist

## 目的 (Purpose)

检查论文是否符合 IEEE Transactions on Information Theory 的格式要求。

**重要说明**:
- **初稿 (Initial Submission)**: 单栏、双倍行距、12点字体、最多35页
- **最终版 (Camera-Ready)**: 双栏 IEEE 格式

本检查清单主要针对最终版格式，但也会标注初稿的特殊要求。

## 使用方法 (How to Use)

1. 确认论文处于哪个阶段（初稿或最终版）
2. 根据阶段选择相应的检查项
3. 逐项检查格式要求
4. 记录发现的问题

---

## 1. 页面设置 / Page Setup

### 1.1 初稿格式 (Initial Submission Format)

- [ ] **单栏**: 使用单栏格式
- [ ] **行距**: 双倍行距
- [ ] **字体大小**: 12点字体
- [ ] **页面大小**: 8.5" × 11" (Letter)
- [ ] **页边距**: 1英寸（上下左右）
- [ ] **页数限制**: 不超过35页（包括图表和参考文献）

**IEEE TIT 初稿要求**:
- ✅ 单栏、双倍行距、12点字体
- ✅ 最多35页
- ✅ 便于评审人阅读和批注

---

### 1.2 最终版格式 (Camera-Ready Format)

- [ ] **双栏**: 使用双栏格式
- [ ] **页面大小**: 8.5" × 11" (Letter)
- [ ] **栏宽**: 3.5英寸
- [ ] **栏间距**: 0.25英寸
- [ ] **页边距**: 上下0.75英寸，左右0.625英寸
- [ ] **字体**: Times New Roman 或类似字体

**IEEE 双栏格式**:
- 使用 IEEE 提供的 LaTeX 模板或 Word 模板
- 模板下载: https://www.ieee.org/publications/authors/author-templates.html

---

## 2. 标题和作者信息 / Title and Author Information

### 2.1 标题 (Title)

- [ ] **标题位置**: 居中，页面顶部
- [ ] **标题字体**: 24点，粗体
- [ ] **标题大小写**: 每个主要单词首字母大写
- [ ] **标题长度**: 不超过12个单词（推荐）
- [ ] **标题准确性**: 准确反映论文内容

**标题格式示例**:
```
Channel Capacity of Gaussian MIMO Channels
with Imperfect Channel State Information
```

**常见问题**:
- 标题过长
- 标题过于笼统或过于具体
- 标题不准确

---

### 2.2 作者信息 (Author Information)

- [ ] **作者姓名**: 居中，标题下方
- [ ] **作者单位**: 居中，作者姓名下方
- [ ] **作者邮箱**: 脚注或单位下方
- [ ] **通讯作者**: 标注通讯作者（如适用）
- [ ] **ORCID**: 提供 ORCID（推荐）

**作者信息格式**:
```
John Doe, Member, IEEE, and Jane Smith, Senior Member, IEEE

Department of Electrical Engineering
University of Example
City, State, Country
Email: {john.doe, jane.smith}@example.edu
```

**IEEE 会员等级**:
- Student Member, IEEE
- Member, IEEE
- Senior Member, IEEE
- Fellow, IEEE

---

## 3. 摘要和关键词 / Abstract and Keywords

### 3.1 摘要 (Abstract)

- [ ] **位置**: 作者信息下方，正文前
- [ ] **格式**: 斜体或普通字体（根据模板）
- [ ] **长度**: 150-250词
- [ ] **结构**: 包含背景、问题、方法、结果
- [ ] **独立性**: 摘要可以独立理解，不依赖正文

**摘要格式**:
```
Abstract—This paper investigates the capacity of...
[150-250 words]
```

**常见问题**:
- 摘要过长或过短
- 摘要缺少关键信息（如主要结果）
- 摘要包含引用或公式（应避免）

---

### 3.2 关键词 (Keywords)

- [ ] **位置**: 摘要下方
- [ ] **格式**: "Index Terms—" 开头
- [ ] **数量**: 5-8个关键词
- [ ] **选择**: 使用 IEEE 术语规范

**关键词格式**:
```
Index Terms—Channel capacity, MIMO systems, information theory, wireless communications.
```

**常见问题**:
- 关键词数量不合适
- 关键词过于笼统或过于具体
- 关键词不符合 IEEE 术语规范

---

## 4. 章节格式 / Section Formatting

### 4.1 章节标题 (Section Headings)

- [ ] **一级标题**: 罗马数字，居中，大写，12点粗体
- [ ] **二级标题**: 大写字母，左对齐，斜体
- [ ] **三级标题**: 阿拉伯数字，左对齐，斜体
- [ ] **编号**: 使用 IEEE 编号系统

**章节编号示例**:
```
I. INTRODUCTION
   A. Background
      1) Historical Context
      2) Motivation
   B. Contributions
```

**常见问题**:
- 章节编号不规范
- 章节标题格式不一致
- 章节层次过多（建议不超过3层）

---

### 4.2 段落格式 (Paragraph Formatting)

- [ ] **首行缩进**: 段落首行缩进0.5英寸
- [ ] **对齐**: 两端对齐
- [ ] **行距**: 单倍行距（最终版）
- [ ] **段间距**: 段落之间无额外空行

---

## 5. 公式格式 / Equation Formatting

### 5.1 公式编号 (Equation Numbering)

- [ ] **编号位置**: 公式右侧，括号内
- [ ] **编号顺序**: 按出现顺序编号
- [ ] **编号格式**: (1), (2), (3), ...
- [ ] **引用格式**: "由公式 (15)" 或 "由 (15)"

**公式格式示例**:
```
C = log(1 + SNR)                    (1)
```

---

### 5.2 公式排版 (Equation Typesetting)

- [ ] **居中**: 公式居中
- [ ] **字体**: 使用数学字体（斜体变量，正体函数）
- [ ] **间距**: 公式前后有适当间距
- [ ] **断行**: 长公式适当断行
- [ ] **符号一致**: 符号使用一致

**公式排版规范**:
- 变量使用斜体: $x$, $y$, $z$
- 函数使用正体: $\log$, $\sin$, $\max$
- 向量使用粗体: $\mathbf{x}$, $\mathbf{y}$
- 矩阵使用粗体大写: $\mathbf{A}$, $\mathbf{B}$

**常见问题**:
- 公式编号位置不对
- 公式字体不规范
- 长公式未适当断行
- 公式间距不当

---

### 5.3 多行公式 (Multi-line Equations)

- [ ] **对齐**: 使用等号或关系符对齐
- [ ] **编号**: 只编号最后一行或每行都编号
- [ ] **间距**: 行间距适当

**多行公式示例**:
```
I(X;Y) = H(X) - H(X|Y)              (2a)
       = H(Y) - H(Y|X)              (2b)
       = H(X) + H(Y) - H(X,Y)       (2c)
```

---

## 6. 图表格式 / Figure and Table Formatting

### 6.1 图格式 (Figure Format)

- [ ] **图编号**: Fig. 1, Fig. 2, ...
- [ ] **图标题**: 图下方，居中
- [ ] **图质量**: 矢量图（PDF、EPS）或高分辨率位图（≥300 DPI）
- [ ] **图大小**: 适合单栏或双栏宽度
- [ ] **图标注**: 坐标轴标签、图例清晰
- [ ] **图引用**: 正文中引用所有图

**图标题格式**:
```
Fig. 1. Capacity region of the Gaussian MAC channel.
```

**图尺寸**:
- 单栏图: 宽度 ≤ 3.5英寸
- 双栏图: 宽度 ≤ 7.16英寸
- 高度: 根据内容调整，但不超过页面高度

**常见问题**:
- 图质量低（模糊、像素化）
- 图标题不够详细
- 图中字体过小
- 图未在正文中引用

---

### 6.2 表格式 (Table Format)

- [ ] **表编号**: TABLE I, TABLE II, ...
- [ ] **表标题**: 表上方，居中
- [ ] **表格线**: 使用三线表（顶线、中线、底线）
- [ ] **表内容**: 清晰、对齐
- [ ] **表引用**: 正文中引用所有表

**表标题格式**:
```
TABLE I
COMPARISON OF DIFFERENT CODING SCHEMES
```

**三线表示例**:
```
─────────────────────────────────
Method      Rate    Complexity
─────────────────────────────────
Turbo       0.5     O(n²)
LDPC        0.5     O(n log n)
Polar       0.5     O(n log n)
─────────────────────────────────
```

**常见问题**:
- 表格线过多（应使用三线表）
- 表标题不够详细
- 表内容不对齐
- 表未在正文中引用

---

### 6.3 图表位置 (Figure and Table Placement)

- [ ] **位置**: 图表在引用后出现
- [ ] **对齐**: 图表居中或左对齐
- [ ] **跨栏**: 大图表可以跨双栏
- [ ] **避免孤立**: 避免图表单独占一页（除非必要）

**LaTeX 位置参数**:
- `[t]`: 页面顶部
- `[b]`: 页面底部
- `[h]`: 当前位置（尽可能）
- `[p]`: 单独一页
- `[!]`: 忽略某些限制

---

## 7. 参考文献格式 / Reference Formatting

### 7.1 参考文献列表 (Reference List)

- [ ] **标题**: "REFERENCES" 或 "参考文献"
- [ ] **编号**: [1], [2], [3], ...
- [ ] **顺序**: 按引用顺序排列
- [ ] **格式**: 符合 IEEE 引用格式（见检查清单5）

**参考文献格式**:
```
REFERENCES

[1] C. E. Shannon, "A mathematical theory of communication," Bell Syst. Tech. J., vol. 27, no. 3, pp. 379-423, Jul. 1948.
[2] T. M. Cover and J. A. Thomas, Elements of Information Theory, 2nd ed. Hoboken, NJ, USA: Wiley, 2006.
```

---

### 7.2 参考文献排版 (Reference Typesetting)

- [ ] **字体大小**: 9点或10点
- [ ] **行距**: 单倍行距
- [ ] **缩进**: 悬挂缩进
- [ ] **间距**: 条目之间无额外空行

---

## 8. 附录格式 / Appendix Formatting

### 8.1 附录标题 (Appendix Heading)

- [ ] **编号**: APPENDIX A, APPENDIX B, ...
- [ ] **标题**: 附录标题（如有）
- [ ] **位置**: 参考文献前

**附录格式**:
```
APPENDIX A
PROOF OF LEMMA 1

[附录内容...]
```

---

### 8.2 附录内容 (Appendix Content)

- [ ] **格式**: 与正文格式一致
- [ ] **公式编号**: 可以使用 (A1), (A2), ... 或继续正文编号
- [ ] **图表编号**: 可以使用 Fig. A1, TABLE A-I, ... 或继续正文编号

---

## 9. 字体和排版 / Font and Typography

### 9.1 字体选择 (Font Selection)

- [ ] **正文字体**: Times New Roman 或类似字体
- [ ] **正文大小**: 10点（双栏）或12点（单栏）
- [ ] **标题字体**: 与正文相同，但加粗
- [ ] **代码字体**: 等宽字体（如 Courier）

---

### 9.2 特殊字符 (Special Characters)

- [ ] **希腊字母**: 使用正确的希腊字母符号
- [ ] **数学符号**: 使用正确的数学符号
- [ ] **特殊符号**: 避免使用非标准符号

**常见符号**:
- 不等号: ≤, ≥, ≠
- 箭头: →, ⇒, ↔
- 集合: ∈, ⊂, ∪, ∩
- 逻辑: ∀, ∃, ∧, ∨
- 其他: ∞, ∂, ∇, ∑, ∏, ∫

---

### 9.3 标点符号 (Punctuation)

- [ ] **句号**: 句末使用句号
- [ ] **逗号**: 适当使用逗号
- [ ] **连字符**: 复合词使用连字符
- [ ] **引号**: 使用双引号 "..."
- [ ] **破折号**: 使用 em dash (—) 或 en dash (–)

**常见问题**:
- 公式后缺少标点
- 连字符使用不当
- 引号使用不规范

---

## 10. 页眉页脚 / Headers and Footers

### 10.1 页眉 (Header)

- [ ] **奇数页**: 作者姓名（最终版）
- [ ] **偶数页**: 期刊名和卷号（最终版）
- [ ] **初稿**: 通常不需要页眉

**页眉格式**:
```
奇数页: DOE AND SMITH: CHANNEL CAPACITY OF GAUSSIAN MIMO CHANNELS
偶数页: IEEE TRANSACTIONS ON INFORMATION THEORY, VOL. XX, NO. Y, MONTH 2026
```

---

### 10.2 页脚 (Footer)

- [ ] **页码**: 居中，底部
- [ ] **初稿**: 所有页面编号
- [ ] **最终版**: 根据 IEEE 要求

---

## 11. 其他格式要求 / Other Format Requirements

### 11.1 脚注 (Footnotes)

- [ ] **编号**: 使用上标数字
- [ ] **位置**: 页面底部
- [ ] **字体**: 小于正文字体
- [ ] **分隔线**: 脚注与正文之间有分隔线

**脚注使用**:
- 作者信息（第一页）
- 致谢（可选）
- 补充说明（少用）

---

### 11.2 列表 (Lists)

- [ ] **项目符号**: 使用标准项目符号（•）
- [ ] **编号列表**: 使用 1), 2), 3), ... 或 a), b), c), ...
- [ ] **缩进**: 列表项适当缩进
- [ ] **间距**: 列表项之间间距适当

---

### 11.3 代码和算法 (Code and Algorithms)

- [ ] **字体**: 使用等宽字体
- [ ] **格式**: 使用算法环境或代码块
- [ ] **编号**: 算法编号（Algorithm 1, Algorithm 2, ...）
- [ ] **标题**: 算法标题清晰

**算法格式示例**:
```
Algorithm 1: Polar Encoding
Input: Information bits u
Output: Encoded bits x
1: Initialize x ← 0
2: for i = 1 to n do
3:    x[i] ← u[i] ⊕ x[i-1]
4: end for
5: return x
```

---

## 12. 版权和许可 / Copyright and Licensing

### 12.1 版权声明 (Copyright Notice)

- [ ] **位置**: 第一页左下角（最终版）
- [ ] **内容**: IEEE 版权声明
- [ ] **格式**: 根据 IEEE 要求

**版权声明示例**:
```
Copyright © 2026 IEEE. Personal use of this material is permitted. However, permission to use this material for any other purposes must be obtained from the IEEE by sending a request to pubs-permissions@ieee.org.
```

---

### 12.2 开放获取 (Open Access)

- [ ] **OA 选项**: 是否选择开放获取
- [ ] **许可证**: 选择合适的许可证（CC BY, CC BY-NC, etc.）
- [ ] **费用**: 了解开放获取费用

---

## 问题记录 / Issue Log

### 格式问题 (Format Issues)

| 问题类型 | 问题描述 | 位置 | 严重程度 |
|---------|---------|------|---------|
| [示例] 页数超限 | 初稿超过35页 | 全文 | Major |
| [示例] 图质量低 | 图3模糊，非矢量图 | 第5页 | Minor |
|         |         |      |         |

### 排版问题 (Typesetting Issues)

| 问题类型 | 问题描述 | 位置 | 严重程度 |
|---------|---------|------|---------|
| [示例] 公式编号 | 公式(15)编号位置不对 | 第8页 | Minor |
|         |         |      |         |

---

## 检查结果总结 / Summary

- **论文阶段**: [ ] 初稿 / [ ] 最终版
- **页数**: [ ] 页（初稿限制35页）
- **完成项目数**: [ ] / [ ]
- **Major Issues**: [ ] 个
- **Minor Issues**: [ ] 个
- **总体评价**: [优秀 / 良好 / 需改进 / 不合格]

---

## 改进建议 / Recommendations

### 高优先级 (High Priority)

1. [建议 1: 减少页数至35页以内（如果是初稿）]
2. [建议 2: 改进图表质量]

### 中优先级 (Medium Priority)

1. [建议 1: 统一格式]
2. [建议 2: 修正公式编号]
3. [建议 3: 完善参考文献格式]

### 低优先级 (Low Priority)

1. [建议 1: 优化排版]
2. [建议 2: 改进图表标题]
3. [建议 3: 统一标点符号]

---

## 有用资源 / Useful Resources

### IEEE 官方资源

- **作者中心**: https://www.ieee.org/publications/authors.html
- **模板下载**: https://www.ieee.org/publications/authors/author-templates.html
- **投稿指南**: https://www.ieee.org/publications/authors/author-guidelines.html
- **IEEE TIT 主页**: https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=18

### LaTeX 资源

- **IEEE LaTeX 模板**: IEEEtran.cls
- **使用指南**: IEEEtran_HOWTO.pdf
- **示例文件**: bare_jrnl.tex

### 格式检查工具

- **PDF 检查**: IEEE PDF eXpress
- **引用格式**: JabRef, Zotero, Mendeley
- **拼写检查**: Grammarly, LanguageTool

---

**检查人**: [姓名]
**检查日期**: [YYYY-MM-DD]
