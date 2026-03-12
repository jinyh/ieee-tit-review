# 符号一致性检查清单 / Symbol Consistency Checklist

## 目的 (Purpose)

检查论文中符号系统的一致性、完整性和规范性。符号混乱是信息论论文的常见问题，会严重影响可读性。

## 使用方法 (How to Use)

1. 第一遍阅读：记录所有符号及其定义
2. 第二遍阅读：检查符号使用的一致性
3. 填写问题记录表

---

## 1. 符号定义完整性 / Symbol Definition Completeness

- [ ] **首次使用时定义**: 所有符号在首次使用时都有定义
- [ ] **符号表**: 论文提供完整的符号表（推荐放在引言后）
- [ ] **特殊符号说明**: 特殊符号（如 ⊕, ⊗, ∼ 等）有明确说明
- [ ] **缩写定义**: 所有缩写在首次使用时都有定义

**IEEE TIT 要求**:
- ✅ 所有符号首次出现时必须定义
- ✅ 推荐提供完整的符号表
- ✅ 符号定义应该清晰、无歧义

**常见问题**:
- 符号未定义就使用
- 符号定义不清晰或有歧义
- 缺少符号表

---

## 2. 符号一致性 / Symbol Consistency

### 2.1 同一符号多个含义 (One Symbol, Multiple Meanings)

- [ ] **检查完成**: 检查是否有同一符号表示不同含义的情况

**常见冲突**:
- H: 熵 (Entropy) vs. 哈密顿量 (Hamiltonian) vs. 矩阵 (Matrix)
- C: 容量 (Capacity) vs. 码本 (Codebook) vs. 常数 (Constant)
- P: 概率 (Probability) vs. 功率 (Power) vs. 概率分布 (Distribution)
- X: 随机变量 (Random Variable) vs. 集合 (Set) vs. 矩阵 (Matrix)
- N: 噪声 (Noise) vs. 码长 (Code Length) vs. 自然数集 (Natural Numbers)

**解决方案**:
- 使用不同的符号（如 H_ent 和 H_ham）
- 使用不同的字体（如 H 和 ℋ）
- 在符号表中明确说明上下文

---

### 2.2 同一含义多个符号 (One Meaning, Multiple Symbols)

- [ ] **检查完成**: 检查是否有同一含义使用不同符号的情况

**常见问题**:
- 互信息: I(X;Y) vs. I(X:Y) vs. MI(X,Y)
- 条件熵: H(X|Y) vs. H_Y(X)
- 期望: E[X] vs. 𝔼[X] vs. ⟨X⟩
- 概率: P(X=x) vs. p(x) vs. Pr(X=x)

**解决方案**:
- 选择一种符号并全文统一使用
- 在符号表中说明选择的符号约定

---

## 3. 信息论符号规范 / Information Theory Notation Standards

### 3.1 基本信息论量 (Basic Information-Theoretic Quantities)

- [ ] **熵 (Entropy)**: H(X) - 使用大写 H
- [ ] **条件熵 (Conditional Entropy)**: H(X|Y) - 使用竖线 |
- [ ] **联合熵 (Joint Entropy)**: H(X,Y) - 使用逗号
- [ ] **互信息 (Mutual Information)**: I(X;Y) - 使用分号 ;
- [ ] **条件互信息 (Conditional MI)**: I(X;Y|Z) - 使用分号和竖线
- [ ] **相对熵/KL散度 (Relative Entropy)**: D(P||Q) - 使用双竖线 ||
- [ ] **容量 (Capacity)**: C - 使用大写 C

**IEEE TIT 推荐符号**:
- ✅ 互信息使用分号: I(X;Y) 而非 I(X:Y)
- ✅ KL散度使用双竖线: D(P||Q) 而非 D(P|Q)
- ✅ 条件使用竖线: H(X|Y) 而非 H(X/Y)

---

### 3.2 概率和随机变量 (Probability and Random Variables)

- [ ] **随机变量 (Random Variables)**: 使用大写字母 X, Y, Z
- [ ] **随机变量取值 (Values)**: 使用小写字母 x, y, z
- [ ] **字母表 (Alphabet)**: 使用花体或大写 𝒳, 𝒴, 𝒵 或 X, Y, Z
- [ ] **概率质量函数 (PMF)**: P_X(x) 或 p(x)
- [ ] **概率密度函数 (PDF)**: f_X(x) 或 p(x)
- [ ] **概率 (Probability)**: P(·) 或 Pr(·)
- [ ] **期望 (Expectation)**: E[·] 或 𝔼[·]
- [ ] **方差 (Variance)**: Var[·] 或 σ²

**一致性要求**:
- ✅ 全文统一使用 P(·) 或 Pr(·)
- ✅ 全文统一使用 E[·] 或 𝔼[·]
- ✅ 区分随机变量（大写）和取值（小写）

---

### 3.3 编码理论符号 (Coding Theory Notation)

- [ ] **码 (Code)**: C - 使用大写 C 或花体 𝒞
- [ ] **码字 (Codeword)**: c 或 x - 使用小写或粗体
- [ ] **码长 (Code Length)**: n - 使用小写 n
- [ ] **码率 (Code Rate)**: R - 使用大写 R
- [ ] **信息位数 (Message Length)**: k - 使用小写 k
- [ ] **最小距离 (Minimum Distance)**: d_min 或 d
- [ ] **汉明距离 (Hamming Distance)**: d_H(·,·)
- [ ] **汉明重量 (Hamming Weight)**: w_H(·)

---

### 3.4 渐近符号 (Asymptotic Notation)

- [ ] **大O符号 (Big-O)**: O(·) - 上界
- [ ] **大Ω符号 (Big-Omega)**: Ω(·) - 下界
- [ ] **大Θ符号 (Big-Theta)**: Θ(·) - 紧界
- [ ] **小o符号 (Little-o)**: o(·) - 严格上界
- [ ] **小ω符号 (Little-omega)**: ω(·) - 严格下界

**使用规范**:
- ✅ 明确说明是关于哪个变量的渐近（如 O(n) 中的 n）
- ✅ 区分 O(1) 和常数

---

## 4. 数学符号规范 / Mathematical Notation Standards

### 4.1 集合论符号 (Set Theory Notation)

- [ ] **集合 (Set)**: 使用花体或大写 𝒜, ℬ, 𝒞 或 A, B, C
- [ ] **元素 (Element)**: a ∈ A - 使用 ∈
- [ ] **子集 (Subset)**: A ⊆ B - 使用 ⊆ 或 ⊂
- [ ] **真子集 (Proper Subset)**: A ⊂ B - 使用 ⊂ 或 ⊊
- [ ] **并集 (Union)**: A ∪ B - 使用 ∪
- [ ] **交集 (Intersection)**: A ∩ B - 使用 ∩
- [ ] **补集 (Complement)**: A^c 或 Ā - 统一使用一种
- [ ] **空集 (Empty Set)**: ∅ - 使用 ∅ 而非 {}
- [ ] **幂集 (Power Set)**: 2^A 或 𝒫(A)

---

### 4.2 线性代数符号 (Linear Algebra Notation)

- [ ] **向量 (Vector)**: 使用粗体小写 **x** 或带箭头 x⃗
- [ ] **矩阵 (Matrix)**: 使用粗体大写 **A** 或普通大写 A
- [ ] **转置 (Transpose)**: A^T 或 A^⊤ - 统一使用一种
- [ ] **共轭转置 (Conjugate Transpose)**: A^H 或 A^† - 统一使用一种
- [ ] **逆 (Inverse)**: A^(-1)
- [ ] **行列式 (Determinant)**: det(A) 或 |A|
- [ ] **迹 (Trace)**: tr(A) 或 Tr(A) - 统一使用一种
- [ ] **秩 (Rank)**: rank(A)
- [ ] **范数 (Norm)**: ||x|| 或 ||x||_p

**一致性要求**:
- ✅ 全文统一向量和矩阵的表示方式
- ✅ 全文统一转置符号

---

### 4.3 分析符号 (Analysis Notation)

- [ ] **极限 (Limit)**: lim_{n→∞}
- [ ] **求和 (Summation)**: ∑_{i=1}^n
- [ ] **乘积 (Product)**: ∏_{i=1}^n
- [ ] **积分 (Integral)**: ∫_a^b
- [ ] **导数 (Derivative)**: df/dx 或 f'(x) 或 ∂f/∂x
- [ ] **梯度 (Gradient)**: ∇f 或 grad f
- [ ] **对数 (Logarithm)**: log(·) 或 ln(·) - 明确底数

**IEEE TIT 要求**:
- ✅ 信息论中的对数默认以 2 为底（除非另有说明）
- ✅ 自然对数使用 ln(·)，常用对数使用 log₁₀(·)

---

## 5. 字体和格式一致性 / Font and Format Consistency

- [ ] **随机变量**: 统一使用斜体大写 (X, Y, Z)
- [ ] **向量**: 统一使用粗体小写 (**x**, **y**, **z**)
- [ ] **矩阵**: 统一使用粗体大写 (**A**, **B**, **C**)
- [ ] **集合**: 统一使用花体或大写 (𝒜, ℬ, 𝒞 或 A, B, C)
- [ ] **常数**: 统一使用普通字体
- [ ] **函数**: 统一使用普通字体 (f, g, h)

---

## 6. 下标和上标规范 / Subscript and Superscript Standards

- [ ] **下标一致性**: 同一含义的下标统一（如时间索引统一使用 t 或 i）
- [ ] **上标一致性**: 同一含义的上标统一（如迭代次数统一使用 (k) 或 ^k）
- [ ] **避免多层下标**: 尽量避免 x_{i_j} 这样的多层下标
- [ ] **下标说明**: 复杂下标有说明（如 x_{i,j}^{(k)} 中各下标的含义）

**常见问题**:
- 时间索引混用 t, i, n
- 迭代次数混用 (k), ^k, _k
- 多层下标难以阅读

---

## 7. 特殊符号检查 / Special Symbol Check

### 7.1 运算符 (Operators)

- [ ] **异或 (XOR)**: ⊕ - 统一使用
- [ ] **张量积 (Tensor Product)**: ⊗ - 统一使用
- [ ] **卷积 (Convolution)**: * 或 ⊛ - 统一使用
- [ ] **点积 (Dot Product)**: · 或 ⟨·,·⟩ - 统一使用

### 7.2 关系符号 (Relation Symbols)

- [ ] **等于 (Equal)**: = - 用于定义或等式
- [ ] **定义为 (Defined as)**: ≜ 或 := - 统一使用
- [ ] **约等于 (Approximately Equal)**: ≈ - 用于近似
- [ ] **渐近等于 (Asymptotically Equal)**: ∼ - 用于渐近分析
- [ ] **正比于 (Proportional to)**: ∝

### 7.3 逻辑符号 (Logic Symbols)

- [ ] **对于所有 (For all)**: ∀
- [ ] **存在 (Exists)**: ∃
- [ ] **逻辑与 (AND)**: ∧
- [ ] **逻辑或 (OR)**: ∨
- [ ] **逻辑非 (NOT)**: ¬

---

## 问题记录 / Issue Log

### 符号冲突 (Symbol Conflicts)

| 符号 | 位置1 | 含义1 | 位置2 | 含义2 | 严重程度 |
|------|-------|-------|-------|-------|---------|
| [示例] H | 第2页 | 熵 | 第5页 | 哈密顿量 | Major |
|      |       |       |       |       |         |

### 未定义符号 (Undefined Symbols)

| 符号 | 首次出现位置 | 严重程度 | 说明 |
|------|-------------|---------|------|
| [示例] λ | 第3页，公式(7) | Minor | 符号λ未定义 |
|      |             |         |      |

### 符号不一致 (Inconsistent Symbols)

| 含义 | 符号1 | 位置1 | 符号2 | 位置2 | 严重程度 |
|------|-------|-------|-------|-------|---------|
| [示例] 互信息 | I(X;Y) | 第2页 | I(X:Y) | 第6页 | Minor |
|      |       |       |       |       |         |

### 格式不一致 (Inconsistent Formatting)

| 对象 | 格式1 | 位置1 | 格式2 | 位置2 | 严重程度 |
|------|-------|-------|-------|-------|---------|
| [示例] 向量 | 粗体 **x** | 第2页 | 箭头 x⃗ | 第4页 | Minor |
|      |       |       |       |       |         |

---

## 检查结果总结 / Summary

- **完成项目数**: [ ] / [ ]
- **符号冲突**: [ ] 个
- **未定义符号**: [ ] 个
- **符号不一致**: [ ] 个
- **格式不一致**: [ ] 个
- **总体评价**: [优秀 / 良好 / 需改进 / 不合格]

---

## 改进建议 / Recommendations

### 高优先级 (High Priority)

1. [建议 1: 解决符号冲突]
2. [建议 2: 定义所有符号]

### 中优先级 (Medium Priority)

1. [建议 1: 统一符号使用]
2. [建议 2: 统一格式]

### 低优先级 (Low Priority)

1. [建议 1: 增加符号表]
2. [建议 2: 改进符号可读性]

---

## 符号表模板 / Notation Table Template

建议在论文中包含以下符号表（放在引言后）：

```markdown
## 符号说明 / Notation

### 一般符号 (General Notation)
- ℝ: 实数集
- ℂ: 复数集
- ℕ: 自然数集
- [n]: 集合 {1, 2, ..., n}

### 信息论符号 (Information-Theoretic Notation)
- H(X): 随机变量 X 的熵
- I(X;Y): X 和 Y 的互信息
- D(P||Q): P 和 Q 的 KL 散度
- C: 信道容量

### 概率符号 (Probability Notation)
- P(·): 概率
- E[·]: 期望
- Var[·]: 方差

### 编码符号 (Coding Notation)
- C: 码
- n: 码长
- R: 码率
- d_min: 最小距离

### 其他符号 (Other Notation)
- [根据论文具体内容添加]
```

---

**评审模式**: [标准评审 / 快速评审]
**检查完成度**: [已检查项数 / 总项数]
**检查日期**: [YYYY-MM-DD]
