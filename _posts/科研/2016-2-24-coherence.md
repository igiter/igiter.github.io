---
layout: post
title: 矩阵内积
category: 科研
tags: 数学
---

Matrix Inner Product and Schur Complement（矩阵内积和Schur补）

> Many problems in the field of signal processing have been expended into matrix problems.So it's necessary for us to know some basic knowledge,including matrix inner product and Schur Complement.
信号领域的很多问题已经扩展到矩阵问题。所以我们很必要学习一些相关的基本知识，例如内积和Schur补。

## 矩阵内积
理论上，只要我们定义的矩阵内积满足内积空间的定义就可以了，但是，我们比较常用的
$$<A,B>=\sqrt{tr(A^HB)}=\sqrt{vec(A)^Hvec(B)}$$

## Schur Complement
最近看的好几篇文章中，都提到了Schur补方法。主要是通过这个理论将一个矩阵的减法表达式换成一种约束一个更大矩阵的形式。
令
$$
\begin{array}{l}
X = \left[ {\begin{array}{*{20}{c}}
{\rm{A}}&B\\
{{{\rm{B}}^H}}&C
\end{array}} \right],S{\rm{ = }}C - {B^H}{A^{ - 1}}B\\
if{\rm{ }}A \succ =0,then{\rm{ }}X \succ =0 \Leftrightarrow S\succ=0
\end{array}
$$

```flow
st=>start: Start
op=>operation: Your Operation
cond=>condition: Yes or No?
e=>end

st->op->cond
cond(yes)->e
cond(no)->op
```