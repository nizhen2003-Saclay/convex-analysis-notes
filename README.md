# 凸分析与最优化中文复习笔记：LaTeX 源文件

编译：在本目录运行 `xelatex main.tex` 两遍（第二遍生成目录和交叉引用）。框架沿用《线性规划复习笔记》。

## 文件分工
- `main.tex`、`preamble.tex`、`guide.tex`、`glossary.tex`：框架（宏包、环境、导读、术语表）。
- `chapters/chNN.tex`：第 NN 章正文，开头自带 `\chapter`；`chapters/appA.tex`：附录 A。
- `exercises/chNN.tex`：第 NN 章练习（原讲义附录 B，只有题目），标题由 `main.tex` 自动加。
- `修改报告.md`：对原讲义的全部内容改动（第一轮：翻译整理）。
- `修改报告-证明审查.md`：第二轮证明审查（用前文结论简化证明、补严重跳步）的改动。
- `第一版存档/`：证明审查之前的完整版本（tex 与 PDF）。
- 第 4 章开头新增的引理标签为 `new:ch04-nonsep`，因此第 4 章其余结果的显示编号比第一版后移 1。

## 可用环境与宏
definition、theorem、lemma、proposition、corollary、example、remark、proof（按章共用编号）；exercise、solution。
常用宏：`\R \Rbar \X \Xs \pair{x^*}{x} \norm \Gammaz \conv \clconv \dom \epi \interior \cont \lev \Nor \prox \argmin`，示性函数统一写 `\iota_K`。

## 标签约定
原讲义的编号是全书连续的，标签按原编号取：定理/命题/引理/推论 N 为 `res:N`，定义 N 为 `def:N`，例 N 为 `exa:N`，注 N 为 `rem:N`，公式 (N) 为 `eq:N`，附录 B.k 第 m 题为 `exo:Bk-m`。整理时新增的结果用 `new:chNN-…`。
