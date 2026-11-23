# 高等代数学精读讲义（LaTeX 源码与 PDF）

面向数学系本科同步精读与现代代数进阶的《高等代数学》系统讲义，以复旦大学《高等代数学（第四版）》（谢启鸿、姚慕生、吴泉水编著）的理论体系为蓝本编撰。

---

## 项目定位与特色

- **双重视角融合**：紧扣“几何赋予灵魂，代数赋予力量”的本科教学主线，同时自然融入现代代数学语言（对称群与交错多线性形式、外代数、商空间与同构定理、主理想整环上的有限生成模结构定理、算子泛函演算、辛几何与 Minkowski 伪欧氏几何）。
- **纯理论精读体例**：正文仅保留**定义、定理、命题、引理、推论与无跳步严格证明**，以及每章末尾的**逻辑脉络图**与**横向结构对照表**；**严格不含例题与习题**（计划后续单独编撰配套习题集）。
- **带星号进阶内容全覆盖**：完整纳入原教材全部带 `*` 号的进阶节与终章（Laplace 展开定理、Cauchy–Binet 公式、Gerschgorin 圆盘定理、矩阵函数与矩阵指数、Hermite 型、实正规矩阵标准型、谱分解与极分解、奇异值分解 SVD、最小二乘解与 Moore–Penrose 广义逆，以及 `*第十章` 双线性型）。
- **三色精读卡片导航**：
  - **【动机与直观】**（深海蓝）：揭示概念与定理的几何/代数起源；
  - **【现代视角】**（青黛色）：衔接抽象代数、泛函分析、数值线性代数与理论物理；
  - **【易错警示】**（绛红色）：点破常见概念陷阱与反例边界。
- **轻量、零脆弱依赖**：纯 `LuaLaTeX` + 标准宏包构建，流程图完全基于原生 `\fcolorbox` 与 `tabular` 实现，不依赖 `tikz` 或 `tcolorbox`，单章独立编译与全书合订均可开箱即用。

---

## 文件清单与章节总览

本项目同时提供**分章独立版本**与**全十章完整合订本**（均含 `.tex` 源码与编译好的 `.pdf`）：

| 章节 | 文件名（`.tex` / `.pdf`） | 核心内容（含带 `*` 号进阶内容） |
| :--- | :--- | :--- |
| **全书合订本** | `advanced_algebra_notes_full` | 封面扉页、前言、连续编号总目录 + 第一至第十章完整正文（124 页） |
| 第一章 行列式 | `ch01_determinants` | 归纳定义、行列展开与 Cramer 法则、对称群 $S_n$ 与 Leibniz 展开、公理化刻画与外代数视角、`*` Laplace 展开定理 |
| 第二章 矩阵 | `ch02_matrices` | 矩阵代数、基础矩阵与迹、逆阵与伴随矩阵、初等变换与阶梯形、分块矩阵与 Schur 补、`*` Cauchy–Binet 公式 |
| 第三章 线性空间 | `ch03_linear_spaces` | 数域与线性空间公理、线性相关性与 Steinitz 替换引理、矩阵秩与核心秩不等式、坐标同构、子空间/直和/商空间、线性方程组解空间 |
| 第四章 线性映射 | `ch04_linear_maps` | $\mathcal{L}(V,U)$ 与结合代数 $\mathcal{L}(V)$、表示矩阵与相抵/相似几何本质、像核维数公式与第一同构定理、不变子空间/商变换、幂等投影与 Fitting 分解 |
| 第五章 多项式 | `ch05_polynomials` | 一元多项式环与带余除法、Bézout 等式与中国剩余定理、唯一因式分解与形式导数判重、Lagrange 插值、$\C/\R/\Q$ 分解与 Gauss/Eisenstein 判别法、多元字典序、对称多项式基本定理与 Newton 公式、结式与判别式 |
| 第六章 特征值 | `ch06_eigenvalues` | 特征值与特征多项式、复方阵 Schur 上三角化、几何/代数重数与对角化判据、Cayley–Hamilton 定理与极小多项式、`*` Gerschgorin 圆盘第一/二定理 |
| 第七章 相似标准型 | `ch07_canonical_forms` | $\lambda$-矩阵与相抵等价、Smith 标准型与不变因子、有理（Frobenius）标准型、初等因子与 Jordan 标准型、准素分解/同时对角化/Jordan–Chevalley 分解、`*` 矩阵幂级数与矩阵指数 |
| 第八章 二次型 | `ch08_quadratic_forms` | 二次型与矩阵合同、Lagrange 配方法与合同初等变换、Jacobi 对角化、复/实规范型与 Sylvester 惯性定理、正定判别与 Cholesky/$LDL'$ 分解、`*` Hermite 型与正定 Hermite 矩阵 |
| 第九章 内积空间 | `ch09_inner_product_spaces` | 欧氏与酉空间、Cauchy–Schwarz、Gram–Schmidt 与正交投影、Riesz 表示与伴随算子、正交/酉变换与 QR/Cartan–Dieudonné、自伴与复正规谱定理、`*` 实正规标准型、`*` 谱分解与极分解、`*` 奇异值分解（SVD）与最小二乘解 |
| `*` 第十章 双线性型 | `ch10_bilinear_forms` | 对偶空间与二次对偶典范同构 $V\cong V^{**}$、双线性型与非退化性、纯量积二分定理、交错型与辛几何（辛基、辛群与 $\det=1$）、对称型正交几何（迷向向量、双曲平面、Witt 消去、Minkowski 时空与 Lorentz 群） |

---

## 编译指南

### 环境要求

- **TeX 发行版**：TeX Live 2021+ 或 MiKTeX（需包含 `lualatex` 引擎）
- **中文字体**：系统需安装思源宋体与思源黑体：
  - `Noto Serif CJK SC`
  - `Noto Sans CJK SC`
  > 若本机使用其他中文字体（如 macOS 的 `Songti SC` / `PingFang SC`，或 Windows 的 `SimSun` / `SimHei` / `FandolSong`），直接修改 `.tex` 导言区中的 `\babelfont{rm}{...}` 与 `\babelfont{sf}{...}` 即可。

### 编译命令

编译**全书合订本**（建议执行 2–3 遍以刷新总目录与交叉引用）：

```bash
lualatex -interaction=nonstopmode advanced_algebra_notes_full.tex
lualatex -interaction=nonstopmode advanced_algebra_notes_full.tex
lualatex -interaction=nonstopmode advanced_algebra_notes_full.tex
```

编译**任意单章**（以第一章为例）：

```bash
lualatex -interaction=nonstopmode ch01_determinants.tex
lualatex -interaction=nonstopmode ch01_determinants.tex
```

---

## 排版规范与符号约定

- **记号体系**：与《高等代数学（第四版）》保持一致——矩阵转置记作 $A'$，共轭转置记作 $A^*$，行列式记作 $|A|$ 或 $\det A$，数域记作 $\K$，秩记作 $r(A)$，伴随矩阵记作 $A^*$（仅在无歧义语境下使用）。
- **页面设置**：A4 纸张、单面排版（`oneside`）、页边距上下 `24mm` / 左右 `23mm`，`11pt` 正文字号与 `1.22` 倍行距，适合屏幕精读与双面打印装订。
- **自定义宏**：统一在导言区定义 `\modernview`、`\intuition`、`\warningbox` 三类精读卡片，以及 `\fnode`、`\mnode` 两类流程图节点，修改配色只需调整导言区顶部的 `\definecolor` 声明。

---

## 后续规划

- 编写与本讲义章节严格一一对应的**配套例题与习题集**（含典型例题精讲、思考题与现代代数进阶题）。
