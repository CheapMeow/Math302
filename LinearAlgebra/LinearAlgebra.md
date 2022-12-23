---
title: "线性代数"
author: "CheapMeow"
date: 2023/12/23
---

- [线性代数](#线性代数)
  - [第一章 行列式](#第一章-行列式)
    - [1.1 行列式的性质与计算公式](#11-行列式的性质与计算公式)
      - [1.1.1 全排列和对换](#111-全排列和对换)
      - [1.1.2 行列式的性质](#112-行列式的性质)
      - [1.1.3 按行与按列展开](#113-按行与按列展开)
      - [1.1.4 特殊行列式](#114-特殊行列式)
    - [1.2 行列式的计算方法](#12-行列式的计算方法)
      - [1.2.1 分块矩阵的行列式](#121-分块矩阵的行列式)
      - [1.2.2 抽象矩阵的行列式](#122-抽象矩阵的行列式)
      - [1.2.3 提取公因式](#123-提取公因式)
      - [1.2.4 拆项](#124-拆项)
      - [1.2.5 每行（列）加和为定值](#125-每行列加和为定值)
      - [1.2.6 递推法](#126-递推法)
      - [1.2.7 两项积商](#127-两项积商)
      - [1.2.8 两项和差](#128-两项和差)
    - [1.3 常用结论](#13-常用结论)
  - [第二章 矩阵](#第二章-矩阵)
    - [2.1 矩阵乘运算](#21-矩阵乘运算)
    - [2.2 矩阵幂运算](#22-矩阵幂运算)
      - [2.2.1 概念](#221-概念)
      - [2.2.2 二项式公式](#222-二项式公式)
      - [2.2.3 对应成比例（由向量生成的矩阵）](#223-对应成比例由向量生成的矩阵)
      - [2.2.4 试算归纳](#224-试算归纳)
      - [2.2.5 行列结合](#225-行列结合)
      - [2.2.6 拆分矩阵](#226-拆分矩阵)
      - [2.2.7 其他计算方法](#227-其他计算方法)
    - [2.3 矩阵的初等变换与线性方程组](#23-矩阵的初等变换与线性方程组)
      - [2.3.1 矩阵的转置](#231-矩阵的转置)
      - [2.3.2 伴随矩阵](#232-伴随矩阵)
      - [2.3.3 逆矩阵](#233-逆矩阵)
      - [2.3.4 判断矩阵可逆性的方法](#234-判断矩阵可逆性的方法)
      - [2.3.5 求逆矩阵的方法](#235-求逆矩阵的方法)
      - [2.3.6 初等变换](#236-初等变换)
      - [2.3.7 矩阵等价](#237-矩阵等价)
      - [2.3.8 线性方程组](#238-线性方程组)
    - [2.4 矩阵方程](#24-矩阵方程)
      - [2.4.1 直接化简](#241-直接化简)
      - [2.4.2 凑目标式](#242-凑目标式)
    - [2.5 矩阵的秩与分块矩阵](#25-矩阵的秩与分块矩阵)
      - [2.5.1 矩阵的秩](#251-矩阵的秩)
      - [2.5.2 子式](#252-子式)
      - [2.5.3 分块矩阵](#253-分块矩阵)
    - [2.6 常用结论](#26-常用结论)
  - [第三章 向量](#第三章-向量)
    - [3.1 向量运算与线性关系](#31-向量运算与线性关系)
      - [3.1.1 线性相关判定](#311-线性相关判定)
      - [3.1.2 线性相关证明](#312-线性相关证明)
    - [3.2 向量组的极大线性无关组与秩](#32-向量组的极大线性无关组与秩)
      - [3.2.1 向量组的秩](#321-向量组的秩)
      - [3.2.2 向量组等价](#322-向量组等价)
    - [3.3 正交化与正交矩阵](#33-正交化与正交矩阵)
      - [3.3.1 Schmidt 正交化](#331-schmidt-正交化)
      - [3.3.2 正交矩阵](#332-正交矩阵)
    - [3.4 常用结论](#34-常用结论)
  - [第四章 线性方程组](#第四章-线性方程组)
    - [4.1 有解无解与解的性质](#41-有解无解与解的性质)
      - [4.1.1 解的性质](#411-解的性质)
      - [4.1.2 解的结构](#412-解的结构)
      - [4.1.3 使用非齐次解 1 - 非齐次解 2 = 基础解系时，注意两个非齐次解对应的非齐次项前的系数是相等的](#413-使用非齐次解-1---非齐次解-2--基础解系时注意两个非齐次解对应的非齐次项前的系数是相等的)
      - [4.1.4 n 阶微分方程对应通解中 n 个独立的常数](#414-n-阶微分方程对应通解中-n-个独立的常数)
    - [4.2 线性方程组解的求法](#42-线性方程组解的求法)
      - [4.2.1 齐次线性方程组基础解系的求法](#421-齐次线性方程组基础解系的求法)
      - [4.2.2 非齐次线性方程组通解的求法](#422-非齐次线性方程组通解的求法)
      - [4.2.3 克拉默法则](#423-克拉默法则)
      - [4.2.4 公共解](#424-公共解)
      - [4.2.5 同解](#425-同解)
      - [4.2.6 抽象线性方程](#426-抽象线性方程)
    - [4.3 常用结论](#43-常用结论)
  - [第五章 特征值、特征向量、相似矩阵](#第五章-特征值特征向量相似矩阵)
    - [5.1 特征值与特征向量](#51-特征值与特征向量)
      - [5.1.1 特征值的性质](#511-特征值的性质)
      - [5.1.2 特征向量的性质](#512-特征向量的性质)
      - [5.1.3 特征值与特征向量的关系](#513-特征值与特征向量的关系)
    - [5.2 特征值与特征向量的计算](#52-特征值与特征向量的计算)
      - [5.2.1 定义法](#521-定义法)
      - [5.2.2 具体型](#522-具体型)
      - [5.2.3 抽象型](#523-抽象型)
      - [5.2.4 特殊矩阵](#524-特殊矩阵)
      - [5.2.5 注意 A 的特征向量与 A^T 的特征向量无关](#525-注意-a-的特征向量与-at-的特征向量无关)
      - [5.2.6 两个矩阵有相同的特征值的证明](#526-两个矩阵有相同的特征值的证明)
      - [5.2.7 利用特征值/特征向量计算参数](#527-利用特征值特征向量计算参数)
    - [5.3 相似](#53-相似)
      - [5.3.1 相似](#531-相似)
      - [5.3.2 相似的性质](#532-相似的性质)
      - [5.3.3 相似的充要条件](#533-相似的充要条件)
      - [5.3.4 相似的必要条件](#534-相似的必要条件)
      - [5.3.5 相似相关的计算](#535-相似相关的计算)
    - [5.4 相似对角化](#54-相似对角化)
      - [5.4.1 能够对角化的充要条件](#541-能够对角化的充要条件)
      - [5.4.2 能够对角化的充分条件](#542-能够对角化的充分条件)
      - [5.4.3 对角化方法](#543-对角化方法)
      - [5.4.4 实对称矩阵的相似对角化方法](#544-实对称矩阵的相似对角化方法)
      - [5.4.5 对阵矩阵的性质](#545-对阵矩阵的性质)
      - [5.4.6 A 相似于 B，但 A 不能对角化时求解 P^(-1)AP 中的 P 的方法](#546-a-相似于-b但-a-不能对角化时求解-p-1ap-中的-p-的方法)
    - [5.5 常用结论](#55-常用结论)
  - [第六章 二次型](#第六章-二次型)
    - [6.1 化二次型为标准形、规范形](#61-化二次型为标准形规范形)
      - [6.1.1 二次型的矩阵表示](#611-二次型的矩阵表示)
      - [6.1.2 化二次型为标准形的方法](#612-化二次型为标准形的方法)
      - [6.1.3 配方法的易错点](#613-配方法的易错点)
    - [6.2 合同](#62-合同)
      - [6.2.1 惯性定理](#621-惯性定理)
      - [6.2.2 对称矩阵不与非对称矩阵合同](#622-对称矩阵不与非对称矩阵合同)
    - [6.3 正定矩阵与正定二次型](#63-正定矩阵与正定二次型)
    - [6.4 常用结论](#64-常用结论)

# 线性代数

## 第一章 行列式

### 1.1 行列式的性质与计算公式

提要：行列式的性质 按行与按列展开 行列式公式

#### 1.1.1 全排列和对换

**1.全排列**

n 个不同元素排成一列，叫做这 n 个元素的全排列（排列）

对于 n 个不同元素，先规定一个标准次序，然后对于这 n 个元素的任一排列，某一对元素的先后次序与标准次序不同时，构成一个逆序

一个排列中所有逆序的总数叫做这个排列的逆序数

逆序数为奇数：奇排列

逆序数为偶数：偶排列

**2.对换**

任意两个元素对调：对换

相邻元素对调：相邻对换

定理：

1. 一个排列中的任意两个元素对换，排列改变奇偶性

    推论：

    1. 奇排列对换成标准排列的对换次数为奇数

        偶排列对换成标准排列的对换次数为偶数

#### 1.1.2 行列式的性质

1. 对换行列式的两行（列），行列式变号

    推论：

    1. 行列式中两行（列）相同（或者成比例），行列式 = 0

3. $
\left|\begin{array}{cccc} 
    a_{11} & a_{12} & \cdots & a_{1n} \\
    \vdots & \vdots & \cdots & \vdots \\
    a_{i1}+a_{j1} & a_{i2}+a_{j2} & \cdots & a_{in}+a_{jn} \\
    \vdots & \vdots & \cdots & \vdots \\
    a_{n1} & a_{n2} & \cdots & a_{nn}
\end{array}\right| 
$ = $\left|\begin{array}{cccc} 
    a_{11} & a_{12} & \cdots & a_{1n} \\
    \vdots & \vdots & \cdots & \vdots \\
    a_{i1} & a_{i2} & \cdots & a_{in}\\
    \vdots & \vdots & \cdots & \vdots \\
    a_{n1} & a_{n2} & \cdots & a_{nn}
\end{array}\right|+
\left|\begin{array}{cccc} 
    a_{11} & a_{12} & \cdots & a_{1n} \\
    \vdots & \vdots & \cdots & \vdots \\
    a_{j1} & a_{j2} & \cdots & a_{jn} \\
    \vdots & \vdots & \cdots & \vdots \\
    a_{n1} & a_{n2} & \cdots & a_{nn}
\end{array}\right|$

#### 1.1.3 按行与按列展开

1. 代数余子式 $A_{ij}=(-1)^{i+j}M_{ij}$

2. 行列式等于其任一行或列的各元素与对应的代数余子式乘积之和
    
    即 $D = a_{i1}A_{i1} + a_{i2}A_{i2} + ... + a_{in}A_{in}$
    
    或 $D = a_{1j}A_{1j} + a_{2j}A_{2j} + ... + a_{nj}A_{nj}$

    推论：

    1. 任一行或列的各元素与其他行或列对应的代数余子式乘积之和 = 0

        因为相当于这个构造出来的新行列式中两行（列）相同

---

例：设 $D_n = \left(\begin{array}{cccc} 
        1 & 1 & \cdots & 1 \\
        0 & 2 & \cdots & 2 \\
          &   & \ddots & \vdots \\
        & &   & n
    \end{array}\right)$，则 $D_n$ 中所有元素的代数余子式之和为

答案：n!

因为 $D_n$ 中所有元素的代数余子式之和可以视为第一行的各元素·第一行对应的代数余子式 + 第一行的各元素·第二行对应的代数余子式 + ... + 第一行的各元素·第 n 行对应的代数余子式

= 第一行的各元素·第一行对应的代数余子式 + 0 + ... + 0

= |D_n| = 主对角线元素的乘积 = n!

对于简单的矩阵，比如稀疏矩阵，可以考虑法 2：求伴随矩阵 $A^*$，求 $A^*$ 的所有元素之和 = 原方程所有元素的代数余子式之和

稀疏矩阵，稍微分块一下，求逆也很方便

#### 1.1.4 特殊行列式

1. 主对角线行列式

    $\left|\begin{array}{cccc} 
        a_{11} & a_{12} & \cdots & a_{1n} \\
        & \ddots & \cdots & a_{2n} \\
        & & \ddots & \vdots  \\
        & & & a_{nn}
    \end{array}\right|=
    \left|\begin{array}{cccc} 
        a_{11} & & & \\
        a_{21} & \ddots & & \\
        \vdots & \cdots & \ddots &  \\
        a_{n1} & a_{n2} & \cdots & a_{nn}
    \end{array}\right|=
    \left|\begin{array}{cccc} 
        a_{11} & & & \\
        & \ddots & & \\
        & & \ddots &  \\
        & & & a_{nn}
    \end{array}\right|=a_{11}\cdots a_{nn}$

2. 副对角线行列式

    $\left|\begin{array}{cccc} 
        & & & a_{1n} \\
        & & \ddots & a_{2n} \\
        & \ddots & \cdots & \vdots  \\
        a_{n1} & a_{n2} & \cdots & a_{nn}
    \end{array}\right|=
    \left|\begin{array}{cccc} 
        a_{11} & a_{12} & \cdots & a_{1n} \\
        a_{21} & \cdots & \ddots & \\
        \vdots & \ddots & & \\
        a_{n1} & & &
    \end{array}\right|=
    \left|\begin{array}{cccc} 
        & & & a_{1n} \\
        & & \ddots & \\
        & \ddots & & \\
        a_{n1} & & &
    \end{array}\right|=(-1)^{\frac{n(n-1)}{2}}a_{1n}\cdots a_{n1}$

3. 范德蒙德行列式

    $\left|\begin{array}{cccc} 
        1 & 1 & \cdots & 1 \\
        a_1 & a_2  & \cdots & a_n \\
        \cdots & \cdots & \vdots & \cdots \\
        a_1^{n-1} & a_2^{n-1} & \cdots & a_n^{n-1} \\
    \end{array}\right| = \prod\limits_{1\leqslant j<i\leqslant n}(a_i-a_j)$

    高序号 - 低序号

    例：四阶范德蒙德行列式的结果为 $(a_4-a_1)(a_4-a_2)(a_4-a_3)(a_3-a_1)(a_3-a_2)(a_2-a_1)$

### 1.2 行列式的计算方法

提要：数字型行列式 分块矩阵的行列式 抽象矩阵的行列式

#### 1.2.1 分块矩阵的行列式

$\left|\begin{array}{cc}
    A & O \\
    O & B
\end{array}\right|=
\left|\begin{array}{cc}
    A & * \\
    O & B
\end{array}\right|=
\left|\begin{array}{cc}
    A & O \\
    * & B
\end{array}\right|=\vert A\vert\cdot\vert B\vert$

$\left|\begin{array}{cc}
    A & B \\
    B & A
\end{array}\right|=|A+B|·|A-B|$

#### 1.2.2 抽象矩阵的行列式

A 是 n 阶矩阵

1. $|A^T| = |A|$

2. $|kA| = k^n|A|$

3. $|AB| = |A||B|$

    特别地，$|A^2| = |A|^2,|A^n| = |A|^n$

    证：考虑行列式，$\left|\begin{array}{cc}
        A & O \\
        -E & B
    \end{array}\right|$ 根据分块矩阵的性质，它的行列式的值 = $|A||B|$

    使用初等变换：对第一列乘 $B$ 加到第二列，行列式不变，即

    $|A||B| = \left|\begin{array}{cc}
        A & O \\
        -E & B
    \end{array}\right| = \left|\begin{array}{cc}
        A & AB \\
        -E & 0
    \end{array}\right| = |AB|$

    非常重要！提供了**两边求行列式**的解题思路

4. $|A^*| = |A|^{n-1}$

    由定义 $AA^* = A^*A = |A|E$ 推出

5. $|A^{-1}| = |A|^{-1}$

6. $|A| = \prod_{i=1}^n{\lambda_i}$，$\lambda_i$ 是 $A$ 的特征值

7. 若 $A \sim B$，则 $|A| = |B|, |A + kE| = |B + kE|$

8. 一般情况下，$|A+B| \ne |A|+|B|,|A-B| \ne |A|-|B|, |kA| \ne k|A|$

例：已知 $A,B$ 均为 3 阶矩阵，$|A| = |B| = 3$，$|A+B| = 30$，则 $|A^{-1}+B^{-1}|=$

$|A^{-1}+B^{-1}| = |EA^{-1}+B^{-1}E| \\
= |B^{-1}BA^{-1}+B^{-1}AA^{-1}| \\
= |B^{-1}(B+A)A^{-1}| \\
= |B^{-1}||B+A||A^{-1}| \\
= 1/3*30*1/3 \\
= 10/3$

这种单位矩阵恒等变形的思想是很经典的

#### 1.2.3 提取公因式

注意可能每做一次初等行（列）变换就要化简一次

证明：$\left|\begin{array}{cccc} 
    1 & 1 & 1 & 1 \\
    a & b & c & d \\
    a^2 & b^2 & c^2 & d^2 \\
    a^4 & b^4 & c^4 & d^4
\end{array}\right|=(a-b)(a-c)(a-d)(b-c)(b-d)(c-d)(a+b+c+d)$。

证明：这个形式看起来像范德蒙德行列式，但是根据后面的结果，发现这无法通过范德蒙德行列式的公式来计算，所以按照一般方法相减得到因子：

$=\left|\begin{array}{cccc} 
    1 & 1 & 1 & 1 \\
    0 & b-a & c-a & d-a \\
    a^2-a^2 & b^2-ab & c^2-ac & d^2-ad \\
    a^4-a^4 & b^4-a^2b^2 & c^4-a^2c^2 & d^4-a^2d^2
\end{array}\right|$

$=\left|\begin{array}{cccc} 
    1 & 1 & 1 & 1 \\
    0 & b-a & c-a & d-a \\
    0 & b(b-a) & c(c-a) & d(d-a) \\
    0 & b^2(b+a)(b-a) & c^2(c+a)(c-a) & d^2(d+a)(d-a)
\end{array}\right|$

$=(b-a)(c-a)(d-a)\left|\begin{array}{cccc} 
    1 & 1 & 1 & 1 \\
    0 & 1 & 1 & 1 \\
    0 & b & c & d \\
    0 & b^2(b+a) & c^2(c+a) & d^2(d+a)
\end{array}\right|$

$=(b-a)(c-a)(d-a)\cdot 1\cdot(-1)^{1+1}\left|\begin{array}{ccc}
    1 & 1 & 1 \\
    b & c & d \\
    b^2(b+a) & c^2(c+a) & d^2(d+a)
\end{array}\right|$

$=(b-a)(c-a)(d-a)\left|\begin{array}{ccc}
    1 & 1 & 1 \\
    0 & c-b & d-b \\
    0 & c(c^2+ac-ab-b^2) & d(d^2+ad-ab-b^2)
\end{array}\right|$

$=(b-a)(c-a)(d-a)\left|\begin{array}{ccc}
    1 & 1 & 1 \\
    0 & c-b & d-b \\
    0 & c(a+b+c)(c-b) & d(a+b+d)(d-b)
\end{array}\right|$

$=(b-a)(c-a)(d-a)\left|\begin{array}{cc}
    c-b & d-b \\
    c(a+b+c)(c-b) & d(a+b+d)(d-b)
\end{array}\right|$

$=(b-a)(c-a)(d-a)(c-b)(d-b)\left|\begin{array}{cc}
    1 & 1 \\
    c(a+b+c) & d(a+b+d)
\end{array}\right|$

$=(b-a)(c-a)(d-a)(c-b)(d-b)(c(a+b+c)-d(a+b+d))$

$=(b-a)(c-a)(d-a)(c-b)(d-b)(ca+cb+c^2-da-db-d^2)$

$=(b-a)(c-a)(d-a)(c-b)(d-b)(a(c-d)+b(c-d)+(c+d)(c-d))$

$=(b-a)(c-a)(d-a)(c-b)(d-b)(c-d)(a+b+c+d)$

#### 1.2.4 拆项

若行列式某一行或一列是有两个值构成，则可以把其拆开，其他部分行列不变

证明：$\left|\begin{array}{ccc}
    ax+by & ay+bz & az+bx \\
    ay+bz & az+bx & ax+by \\
    az+bx & ax+by & ay+bz
\end{array}\right|=(a^3+b^3)\left|\begin{array}{ccc}
    x & y & z \\
    y & z & x \\
    z & x & y
\end{array}\right|$。

证明：首先因为上下因式的系数是 $ab$，所以无论怎么样减都无法消去多余的 $xy$ 或 $z$ 得到结果的行列式中只有单个因子的情况，所以只能拆项，从第一个项开始拆：

$=a\left|\begin{array}{ccc}
    x & ay+bz & az+bx \\
    y & az+bx & ax+by \\
    z & ax+by & ay+bz
\end{array}\right|+b\left|\begin{array}{ccc}
    y & ay+bz & az+bx \\
    z & az+bx & ax+by \\
    x & ax+by & ay+bz
\end{array}\right|$

$=a^2\left|\begin{array}{ccc}
    x & ay+bz & z \\
    y & az+bx & x \\
    z & ax+by & y
\end{array}\right|+b^2\left|\begin{array}{ccc}
    y & z & az+bx \\
    z & x & ax+by \\
    x & y & ay+bz
\end{array}\right|=a^3\left|\begin{array}{ccc}
    x & y & z \\
    y & z & x \\
    z & x & y
\end{array}\right|+b^3\left|\begin{array}{ccc}
    y & z & x \\
    z & x & y \\
    x & y & z
\end{array}\right|$

$=a^3\left|\begin{array}{ccc}
    x & y & z \\
    y & z & x \\
    z & x & y
\end{array}\right|+b^3\left|\begin{array}{ccc}
    x & y & z \\
    y & z & x \\
    z & x & y
\end{array}\right|=(a^3+b^3)\left|\begin{array}{ccc}
    x & y & z \\
    y & z & x \\
    z & x & y
\end{array}\right|
$

#### 1.2.5 每行（列）加和为定值

当行列式每一行或每一列相加都为一个固定的值，可以把第二行开始的各行都加到第一行或列，再提取公因式，提出后第一行或第一列变为1，再依次对每行或每列进行消去，最终变成对角线行列式

计算：$\left|\begin{array}{cccc} 
    x & a & \cdots & a \\
    a & x & \cdots & a \\
    \vdots & \vdots & \ddots & \vdots \\
    a & a & \cdots & x \\
\end{array}\right|$。

解：$=\left|\begin{array}{cccc} 
    x+(n-1)a & x+(n-1)a & \cdots & x+(n-1)a \\
    a & x & \cdots & a \\
    \vdots & \vdots & \ddots & \vdots \\
    a & a & \cdots & x \\
\end{array}\right|$

$=(x+(n-1)a)\left|\begin{array}{cccc} 
    1 & 1 & \cdots & 1 \\
    a & x & \cdots & a \\
    \vdots & \vdots & \ddots & \vdots \\
    a & a & \cdots & x \\
\end{array}\right|=(x+(n-1)a)\left|\begin{array}{cccc} 
    1 & 1 & \cdots & 1 \\
     & x-a & &  \\
     & & \ddots & \\
     & & & x-a \\
\end{array}\right|$

$=(x+(n-1)a)(x-a)^{n-1}$

---

由此可以总结出每行（列）加和为定值 $c$ 的推论

推论 1：$\lvert A \rvert = 0$

推论 2：$(1,1,...,1)^T$ 为 $Ax = b$ 的解，其中列向量 $b$ 为 $ (c,c,...,c)^T$

特殊情况：每行（列）加和 = 0 => $(1,1,...,1)^T$ 为 $Ax = 0$ 的解

例：设 $A = (a_{ij})_{n \times n}$，满足 $\sum_{j = 1}^n{a_{ij}} = 0(i = 1,2,...,n)$，$A_{ij}$ 为 $a_{ij}$ 的代数余子式，则下列各式必成立的是（）

A. $A_{11} = A_{12} = ... = A_{1n} = 0$

B. $A_{11} = A_{12} = ... = A_{1n} = n$

C. $A_{11} = A_{12} = ... = A_{1n} = 1$

D. $A_{11} = A_{12} = ... = A_{1n}$

答案：D

$\sum_{j = 1}^n{a_{ij}} = 0(i = 1,2,...,n)$ =>

1. $\lvert A \rvert = 0$ 即 $R(A) < n$

2. $(1,1,...,1)^T$ 为 $Ax = 0$ 的解

首先对于 $R(A) < n$ 来说，$R(A)$ 仍然可能有多种情况

根据 $R(A)$ 与 $R(A^*)$ 的关系：$
R(A^*) = \left\{
    \begin{array}{lcl}
        n, R(A) = n, \\
        1, R(A) = n - 1, \\
        0, R(A) \leqslant n -2  
    \end{array}
    \right.
$

可知，需要分两种情况：

(1) 若 $R(A) < n-1$，则 $R(A^*) = 0$ 即 $A^* = O$，则

$A_{11} = A_{12} = ... = A_{1n} = 0$

(2) 若 $R(A) = n-1$，则 $Ax = 0$ 只有一个基础解，即 $(1,1,...,1)^T$ 为 $Ax = 0$ 的全部基础解系

又因为 $AA^* = \lvert A \rvert E = 0$，所以 $A^*$ 的每一列均为 $Ax = 0$ 的解

所以 $A^*$ 的每一列均为 $k(1,1,...,1)^T$，$k$ 为任意常数

综上所述，$A_{11} = A_{12} = ... = A_{1n}$，D 正确

#### 1.2.6 递推法

通过行列式展开得到递推公式

用例：三对角行列式

#### 1.2.7 两项积商

简单

#### 1.2.8 两项和差

两项和差需要将方阵拆分为向量组的形式，然后根据矩阵与行列式的运算法则进行运算

差别：

两个矩阵相加：[>> 1.2.2 抽象矩阵的行列式](#122-抽象矩阵的行列式)

矩阵中某行（列）拆项：[>> 1.1.1 行列式的性质](#111-行列式的性质)

例：设四阶方阵 $A=[\alpha,\gamma_2,\gamma_3,\gamma_4]$，$B=[\beta,\gamma_2,\gamma_3,\gamma_4]$，其中 $\alpha$、$\beta$、$\gamma_i$ 均为四维向量，且 $\vert A\vert=5$，$\vert B\vert=-\dfrac{1}{2}$，求 $\vert A+2B\vert$

解：$=\vert[\alpha,\gamma_2,\gamma_3,\gamma_4]+2[\beta,\gamma_2,\gamma_3,\gamma_4]\vert=\vert[\alpha+2\beta,3\gamma_2,3\gamma_3,3\gamma_4]\vert=27\vert[\alpha+2\beta,\gamma_2,\gamma_3,\gamma_4]\vert=27\vert[\alpha,\gamma_2,\gamma_3,\gamma_4]\vert+54\vert[\beta,\gamma_2,\gamma_3,\gamma_4]\vert=27(\vert A\vert+2\vert B\vert)=108$

### 1.3 常用结论

## 第二章 矩阵

### 2.1 矩阵乘运算

一般情况下：

1. 没有交换律

    $AB \ne BA$

2. 相乘 = 0

    $AB = O$ 不能推出 $A = O$ 或 $B = O$

3. 没有消去律

    $BA = B, B \ne O$ 不能推出 $A = E$

    $A\alpha = A\beta,A \ne O$ 不能推出 $\alpha = \beta$

### 2.2 矩阵幂运算

提要：矩阵的运算 特殊矩阵

#### 2.2.1 概念

1. 幂

    $(AB)^k\neq A^kB^k$。只有 $AB$ 可交换时才相等

    $A\neq 0$ 不能推出 $A^k\neq 0$，例：

    $A=\left(
        \begin{array}{cc}
            0 & 2 \\
            0 & 0
        \end{array}
    \right)\neq 0$。$A^2=\left(
        \begin{array}{cc}
            0 & 2 \\
            0 & 0
        \end{array}
    \right)\left(
        \begin{array}{cc}
            0 & 2 \\
            0 & 0
        \end{array}
    \right)=\left(
        \begin{array}{cc}
            0 & 0 \\
            0 & 0
        \end{array}
    \right)=O$

2. 常见误区

    $(AB)^2 = (AB)(AB) \ne A^2B^2$

    $(A+B)^2 = A^2 + AB + BA + B^2 \ne A^2 + 2AB + B^2$

    $(A+B)(A-B) = A^2 - AB + BA + B^2 \ne A^2 - B^2$

#### 2.2.2 二项式公式

$(A+B)^n = \sum_{i=0}^n(C_n^iA^{n-i}B^i)$

常用于某个矩阵的高阶幂为 0 的情况，这样方便化简

#### 2.2.3 对应成比例（由向量生成的矩阵）

因为矩阵运算不满足交换率但是满足结合率，且一行矩阵乘一列矩阵的乘积为一个数，所以可以推出矩阵的幂的运算方法。

这个方法要求 $r(A)=1$，即对应成比例。

令 $A$ 为 $n$ 阶方阵，将 $A$ 拆为 $A=(a_1,a_2,\cdots,a_n)^T(b_1,b_2,\cdots,b_n)=\alpha^T\beta$，所以 $A^n=\alpha^T\beta\alpha^T\beta\cdots\alpha^T\beta$，利用结合率：$\alpha^T(\beta\alpha^T)(\beta\cdots\alpha^T)\beta$，中间一共 $n-1$ 个 $\beta\alpha^T$，$\beta\alpha^T$ 是一个数，即 $A^n=(\beta\alpha^T)^{n-1}\alpha^T\beta=(\beta\alpha^T)^{n-1}A$

其实本质上也是行列结合

例：$A=\left(\begin{array}{ccc}
    1 & 2 & 3 \\
    -2 & -4 & -6 \\
    3 & 6 & 9
\end{array}\right)$，求 $A^n$

解：$A=(1,-2,3)^T(1,2,3)$，所以 $A^n=((1,2,3)(1,-2,3)^T)^n(1,-2,3)^T(1,2,3)$

$=6^{n-1}A$

若矩阵 $A$ 的行与列都成比例，则 $A^n=[tr(A)]^{n-1}A$，$[tr(A)]=\sum a_{ii}$，即矩阵迹为对角线元素值之和

#### 2.2.4 试算归纳

对 $A$ 进行试算，如 $A^2$，若 $A^k$ 是一个数量阵，那么计算 $A^n$ 就只用找规律就可以了

例：$A=\left(\begin{array}{cccc}
    1 & -1 & -1 & -1 \\
    -1 & 1 & -1 & -1 \\
    -1 & -1 & 1 & -1 \\
    -1 & -1 & -1 & 1 \\
\end{array}\right)$，求 $A^n$（$n\geqslant2$）

解：通过计算得知 $A^2=4E$，这是一个数量阵

$\therefore A^n=\left\{\begin{array}{lcl}
    4^kE, & & n=2k \\
    4^kA, & & n=2k+1
\end{array}\right.$

#### 2.2.5 行列结合

将一个矩阵拆成 $\alpha\beta^T$ 的形式，其中都是列向量，从而进行幂运算可以进行结合 $\beta^T\alpha$ 为一个常数

#### 2.2.6 拆分矩阵

将 $A^n$ 拆分为两个矩阵 $A^n=(B+C)^n$，其中 $BC$ 应该是可逆的，即 $BC=CB$，所以一般有一个是 $E$

#### 2.2.7 其他计算方法

1. 当 $r(A) = 1$ 时，有 $A^2 = lA$，$l = \sum{a_{ii}}$ 是矩阵的迹

2. 特征值、特征向量、相似

### 2.3 矩阵的初等变换与线性方程组

提要：伴随矩阵 可逆矩阵 初等矩阵与初等变换 等价

#### 2.3.1 矩阵的转置

$(A+B)^T = A^T + B^T$

#### 2.3.2 伴随矩阵

**1.定义**

$A^* = \left(\begin{array}{cccc} 
    A_{11} & A_{21} & \cdots & A_{n1} \\
    A_{12} & A_{22} & \cdots & A_{n2} \\
    \vdots & \vdots & \ddots & \vdots \\
    A_{1n} & A_{n1} & \cdots & A_{nn} \\
\end{array}\right)$

不管 $A$ 是否可逆，伴随矩阵都会存在，因为伴随矩阵的定义不依靠可逆性

注意：伴随矩阵的元素——代数余子式的下标的行列号与它在伴随矩阵中的位置的行列号是相反的

这一点很容易忽略...然而就是因为这个相反的顺序，决定了伴随矩阵的性质

**2.性质**

1. $AA^* = A^*A = |A|E$

    证：矩阵乘法是行乘列，但注意到 $A^*$ 的代数余子式的下标与它在伴随矩阵中的位置是相反的，所以有：

    $A^*$ 左乘 $A$ 相当于用原矩阵每一行乘原矩阵每一行的伴随矩阵

    $A^*$ 右乘 $A$ 相当于用原矩阵每一列的伴随矩阵乘原矩阵每一列

    因此得到的乘积必然是主对角线上为 $|A|$，其他位置为 0 的矩阵

2. $(A^T)^*=(A^*)^T$，$(A^{-1})^*=(A^*)^{-1}$，$(AB)^*=B^*A^*$

其他式子可以自然推出，例如 $(A^*)^*=\vert A\vert^{n-2}A$

**3.重要结论**

$
R(A^*) = \left\{
    \begin{array}{lcl}
        n, R(A) = n, \\
        1, R(A) = n - 1, \\
        0, R(A) \leqslant n -2  
    \end{array}
    \right.
$

---

例：设 A 为 n 阶方阵，齐次线性方程组 $Ax = 0$ 有两个线性无关的解，$A^*$ 是 $A$ 的伴随矩阵，则有（）

A. $A^*x = 0$ 的解均为 $Ax = 0$ 的解

B. $Ax = 0$ 的解均为 $A^*x = 0$ 的解

C. $Ax = 0$ 与 $A^*x = 0$ 无非零公共解

D. $Ax = 0$ 与 $A^*x = 0$ 恰好有一个非零公共解

答案：B

齐次线性方程组有两个线性无关的解，意思是至少有两个线性无关的解

那么解空间的秩至少为 2，即 $R(A) \leqslant n-2$

根据 $R(A^*)$ 与 $R(A)$ 的关系，得 $R(A) = 0$

#### 2.3.3 逆矩阵

**1.定义**

对于 n 阶矩阵 A，如果有一个 n 阶矩阵 $B$，使 $AB = BA = E$

那么 $A$ 可逆，逆矩阵为 $B$

> 很多时候需要注意到一个矩阵乘另一个矩阵等于 $E$ 这种形式
>
> 如果 $A$ 乘了一个复杂的式子，一时间可能还没想到把这个式子看成一个整体 $B$
>
> 实际上这是没有深刻意识到逆矩阵的唯一性……就是说只要满足这个形式，那就一定是我的逆矩阵！

**2.性质**

$(AB)^{-1} = B^{-1}A^{-1}$

$(A^T)^{-1} = (A^{-1})^T$

一般来说，$(A+B)^{-1} \ne A^{-1} + B^{-1}$

#### 2.3.4 判断矩阵可逆性的方法

n 阶矩阵 $A$ 可逆 <=>

1. $|A| \ne 0$

    证 $|A| \ne 0$ => $A$ 可逆：
    
    因为 $AA^* = |A|E$，所以 $A\dfrac{A^*}{|A|} = E$

    根据可逆定义，$A$ 可逆，逆矩阵为 $\dfrac{A^*}{|A|}$

    证 $A$ 可逆 => $|A| \ne 0$：

    根据可逆定义，存在 $AA^{-1} = E$，两边求行列式，得

    $|AA^{-1}| = |A||A^{-1}| = |E| \ne 0$，所以 $|A| \ne 0$
    
    ---

    最常用的解题思路是**两边求行列式**
    
    已知 $AB = C$，已知 $C$ 可逆
    
    那么 $|C| \ne 0$，又由于 $|AB| = |A||B| = |C| \ne 0$，所以有 $|A| \ne 0, |B| \ne 0$，即 $A,B$ 也可逆

2. $A^T$ 可逆

    因为 $|A^T| = |A|$，所以化归为第 1 种情况

3. $A^*$ 可逆

    证 $A^*$ 可逆 => $A$ 可逆：

    未知 $A$ 是否可逆，所以未知 $|A|$ 是否 = 0

    所以由 $AA^* = |A|E$ 不能轻易得到 $A\dfrac{A^*}{|A|} = E$，而是有可能得到 $AA^* = 0$

    换一个思路，使用反证法：

    设已知 $A^*$ 可逆时，$A$ 不可逆

    根据 $AA^* = |A|E = 0$ 两边同乘 $A^*$ 的逆矩阵，得 $A = 0$，这就也导致 $A^* = 0$，与 $A^*$ 可逆矛盾

    于是假设错误，得证 $A$ 可逆

    证 $A$ 可逆 => $A^*$ 可逆：

    $A$ 可逆，所以 $|A| \ne 0$

    由 $A^*A = |A|E$，得 $A^*\dfrac{A}{|A|} = E$

    根据可逆的定义，$A^*$ 可逆，逆矩阵为 $\dfrac{A}{|A|}$

4. $A^k$ 可逆

    因为 $|A^k| = |A|^k$，所以化归为第 1 种情况

5. $R(A) = n$

    变形：

    1. 行向量组线性无关

    2. 列向量组线性无关

6. $Ax = 0$ 只有零解

7. $Ax = b$ 有唯一解

8. 特征值全不为零

    因为 $\prod\limits_{i=1}^n\lambda_i=\vert A\vert$，所以化归为第 1 种情况

9. 若 $AB = AC$，必有 $B = C$

10. 若 $BA = CA$，必有 $B = C$

11. $A$ 可写成初等矩阵的乘积

12. $A$ 和 $E$ 等价

#### 2.3.5 求逆矩阵的方法

**1.用伴随矩阵定义 $AA^* = A^*A = |A|E$**

$A = \left(\begin{array}{cc}
    a & b \\
    c & d
\end{array}\right),A^* = \left(\begin{array}{cc}
    d & -c \\
    -b & a
\end{array}\right)$

则 $A^{-1} = A^*/|A| = \dfrac{1}{ad-bc}\left(\begin{array}{cc}
    d & -c \\
    -b & a
\end{array}\right)$

特殊的，若 $A = \left(\begin{array}{cc}
    a & 0 \\
    0 & b
\end{array}\right),A^* = \left(\begin{array}{cc}
    d & 0 \\
    0 & a
\end{array}\right)$

则 $A^{-1} = A^*/|A| = \left(\begin{array}{cc}
    \dfrac{1}{a} & 0 \\
    0 & \dfrac{1}{b}
\end{array}\right)$

**2.初等变化法**

$(A|E) \to (E|A^{-1})$

**3.$AB = E$，若可求 $B$，则 $A^{-1} = B$**

**4.分块矩阵**

可以使用分块矩阵嵌套使用以上求逆方法

$\left(\begin{array}{cc}
    B & O \\
    O & C
\end{array}\right)^{-1}=
\left(\begin{array}{cc}
    B^{-1} & O \\
    O & C^{-1}
\end{array}\right)$

$\left(\begin{array}{cc}
    O & B \\
    C & O
\end{array}\right)^{-1}=
\left(\begin{array}{cc}
    O & C^{-1} \\
    B^{-1} & O
\end{array}\right)$

这只是分开写方便记，如果四个位置都有元素，主对角线上两个元素和副对角线上两个元素不相干的，照样都使用这个规律

**5.分解乘积求逆**

将 $A$ 分解为若干个可逆矩阵的乘积。若 $A=BC$，$B$，$C$ 可逆，则 $A$ 可逆，且 $A^{-1}=C^{-1}B^{-1}$

同理 $(ABC)^{-1}=C^{-1}B^{-1}A^{-1}$

考虑使用 [>> 1.2.2 抽象矩阵的行列式](#122-抽象矩阵的行列式) 中的单位恒等变换

#### 2.3.6 初等变换

例：设 $A = \left(\begin{array}{cc}
    1 & 0 & 0 \\
    2 & 0 & 3
\end{array}\right),B = \left(\begin{array}{cc}
    1 & 0 & 0 \\
    0 & 1 & 0
\end{array}\right)$，若可逆矩阵 $P$ 与 $Q$ 使得 $PAQ = B$，则 $P$ 与 $Q$ 依次可为（）

A. $\left(\begin{array}{cc}
    1 & 0 \\
    -2 & 1
\end{array}\right),\left(\begin{array}{cc}
    1 & 0 & 0 \\
    0 & 1 & 1 \\
    0 & \dfrac{1}{3} & 0
\end{array}\right)$

B. $\left(\begin{array}{cc}
    1 & 0 \\
    -2 & 3
\end{array}\right),\left(\begin{array}{cc}
    0 & 0 & 1 \\
    1 & 0 & 0 \\
    0 & 1 & 0
\end{array}\right)$

C. $\left(\begin{array}{cc}
    1 & 0 \\
    -\dfrac{1}{3} & \dfrac{2}{3}
\end{array}\right),\left(\begin{array}{cc}
    0 & 1 & 0 \\
    0 & 0 & 1 \\
    1 & 0 & 0
\end{array}\right)$

D. $\left(\begin{array}{cc}
    1 & 0 \\
    -\dfrac{2}{3} & \dfrac{1}{3}
\end{array}\right),\left(\begin{array}{cc}
    1 & 0 & 0 \\
    0 & 0 & 1 \\
    0 & 1 & 0
\end{array}\right)$

答案：D

对 A 作初等变换，有 $\left(\begin{array}{cc}
    1 & 0 \\
    0 & \dfrac{1}{3}
\end{array}\right)\left(\begin{array}{cc}
    1 & 0 \\
    -2 & 1
\end{array}\right)A\left(\begin{array}{cc}
    1 & 0 & 0 \\
    0 & 0 & 1 \\
    0 & 1 & 0
\end{array}\right) = B$

所以 $P = \left(\begin{array}{cc}
    1 & 0 \\
    0 & \dfrac{1}{3}
\end{array}\right)\left(\begin{array}{cc}
    1 & 0 \\
    -2 & 1
\end{array}\right) = \left(\begin{array}{cc}
    1 & 0 \\
    -\dfrac{2}{3} & \dfrac{1}{3}
\end{array}\right), Q = \left(\begin{array}{cc}
    1 & 0 & 0 \\
    0 & 0 & 1 \\
    0 & 1 & 0
\end{array}\right)$

> 题的正解的逻辑很简单，但是记录下来的原因是，我不知道这种题，变换矩阵一定要用初等变换矩阵来构造吗
>
> 我算了一个 A 选项，发现这个选项的两个矩阵也是符合题意的，但是为啥不选……
>
> A 选项的两个矩阵也是可逆的，也没有不符合条件
>
> 可能是我哪里又有一些隐秘的逻辑错误？

#### 2.3.7 矩阵等价

**1.定义**

设 $A$, $B$ 为 m\*n 矩阵，那么：

$A$ 能经过初等变换得到 $B$，则 $A$ 与 $B$ 等价

即 $A$ 与 $B$ 等价 <=> 存在 m 阶可逆矩阵 $P$ 及 n 阶可逆矩阵 $Q$，使 $PAQ = B$

**2.判断矩阵等价**

1. 根据定义，是否能找到这个初等变换

    易知符合矩阵等价定义的初等变换不是唯一的

2. 若 $A$ 与 $B$ 同型（行数列数相等），且秩相同 => $A$ 与 $B$ 等价

    本质上跟使用初等变换一样的，因为初等变换不改变秩

> 矩阵的等价与向量组的等价不是同一个概念！
>
> 矩阵 $A \sim B$ 不能得出 $A$ 的列向量组 $\sim$ B 的列向量组

#### 2.3.8 线性方程组

n 元线性方程组 $Ax = b$

1. 无解 <=> $R(A) < R(A, b)$

2. 有解 <=> $R(A) = R(A, b)$

    1. 有唯一解 <=> $R(A) = R(A, b) = n$

    2. 有无限多解 <=> $R(A) = R(A, b) < n$

推广：

1. n 元线性方程组 $Ax = 0$ 有非零解 <=> $R(A) = R(A, b)$

2. 矩阵方程 $Ax = B$ 有解 <=> $R(A) = R(A, B)$

    推广：

    1. 可证矩阵的秩的性质：若 $AB = C$，则 $R(C) \leqslant \min\{R(A), R(B)\}$

        证明：
        
        $B$ 是 $AX = C$ 的解，则 $R(A) = R(A, C)$

        又因为 $R(C) \leqslant R(A, C)$，所以得 $R(C) \leqslant R(A)$

        对 $AB = C$ 转置，得 $B^TA^T = C^T$，同理得，$R(C^T) \leqslant R(B^T)$，即 $R(C) \leqslant R(B)$

        综上得 $R(C) \leqslant \min\{R(A), R(B)\}$

> 转置是一个常用的证明方法！
>
> 类似这个证明，用在同时存在转置敏感的定理（矩阵方程 $Ax = B$）和转置不敏感的定理（$R(A) = R(A^T)$）的时候

### 2.4 矩阵方程

含有未知矩阵的方程就是矩阵方程，需要将方程进行恒等变形，化为 $AX=B$、$XA=B$ 或 $AXB=C$ 的形式

若 $A$、$B$ 可逆，且可以分别得到 $X=A^{-1}B$，$X=BA^{-1}$，$X=A^{-1}CB^{-1}$

#### 2.4.1 直接化简

简单

#### 2.4.2 凑目标式

有时候直接化简非常麻烦，因为所求的式子很复杂，甚至出现结果不能得到的情况

例：已知 $AB=A+B$，其中 $B=\left[\begin{array}{ccc}
    1 & 1 & 0 \\
    1 & 1 & 0 \\
    0 & 0 & 2
\end{array}\right]$，求 $(A-E)^{-1}$

解：已知 $AB=A+B$，求 $A-E$，则向目标计算

$AB-B=A$，即 $(A-E)B=A$，$(A-E)^{-1}=BA^{-1}$。因为 $A$ 未知，所以要消去 $A$

根据 $AB=A+B$，得到 $AB-A=B$，即 $A(B-E)=B$，$A^{-1}=(B-E)B^{-1}$

$(A-E)^{-1}=BA^{-1}=B(B-E)B^{-1}$，然后就不知道接下来怎么办了

我们很希望 $BB^{-1}$ 在一起消掉，但是无论如何操作都无法完成。但是也可以通过此得到解题的启示，按 $(A-E)(B-E)$ 去凑

回到 $(A-E)B=A$，去凑 $B-E$，先尝试两边减去 $E$，得到 $(A-E)B-E=A-E$，正好左移右项 $(A-E)(B-E)=E$，解得 $(A-E)^{-1}=B-E$

即 $=\left[\begin{array}{ccc}
    0 & 1 & 0 \\
    1 & 0 & 0 \\
    0 & 0 & 1
\end{array}\right]$

### 2.5 矩阵的秩与分块矩阵

提要：矩阵的秩 分块矩阵

#### 2.5.1 矩阵的秩

秩的本质就是组成矩阵的线性无关的向量个数

$r(A) = r(A^T), r(A^TA) = r(A)$（因为 $A$ 和 $A^TA$ 同解）

$max\{r(A),r(B)\}\leqslant r(A|B)\leqslant r(A)+r(B)$

$r(A+B)\leqslant r(A|B)\leqslant r(A)+r(B)$

$r(A^*)=\left\{\begin{array}{l}
    n, r(A)=n \\
    1, r(A)=n-1 \\
    0, r(A)<n-1
\end{array}\right.$

$r(AB)\leqslant\min\{r(A),r(B)\}$。当且仅当 $AB$ 满秩等号成立

若 $A$ 可逆，则 $r(AB) = r(BA) = r(B)$

因为初等变换矩阵是可逆的，所以经过初等变化的矩阵的秩不变

若 $A$ 为 m\*n 矩阵，$B$ 为 n\*s 矩阵，$AB = O$，则 $r(A)+r(B) \leqslant n$

分块矩阵 $r\left(\begin{array}{cc}
        A & O \\
        O & B
    \end{array}\right)=r(A)+r(B)$

> 常用夹逼方法求矩阵为满秩，例如使用以下两个定理
>
> 1.若 $A$ 为 m\*n 矩阵，$B$ 为 n\*s 矩阵，$AB = O$，则 $r(A)+r(B) \leqslant n$
>
> 2.$r(A+B)\leqslant r(A|B)\leqslant r(A)+r(B)$

例：若 $A$ 为 n 阶矩阵，且 $A^2 = E$，证明：$r(A+E)+r(A-E) = n$

由于 $A^2 - E = (A+E)(A-E) = 0$，所以这一眼就看出来可以用 $r(A) + r(B) \leqslant n$

即 $r(A+E)+r(A-E) \leqslant n$

又因为待证的等式 = n，所以看出来要夹逼

那么已知的规律中只有 $r(AB) \leqslant r(A) + r(B)$ 能够从左边夹

但是 $A+E+A-E = 2A$，$r(2A) \leqslant r(A+E)+r(A-E)$ 似乎没什么意义

什么东西加起来的秩一定等于 n？$E$ 的秩一定等于 n，如果 $A,B$ 加起来等于 $E$ 就好了

这个时候就需要变换了，$r(A-E) = r(E-A)$，这样，$r(2E) = n \leqslant r(A+E)+r(E-A) = r(A+E)+r(A-E)$

夹逼得到 $r(A+E)+r(A-E) = n$

#### 2.5.2 子式

在矩阵中，任取 $k$ 行和 $k$ 列 ，位于这些行和列的交点上的 $k^2$ 个元素原来的次序所组成的 $k$ 阶方阵的行列式，叫做 $A$ 的一个 $k$ 阶子式。

当 $r(A)=r$ 时：

1. $A$ 中一定有 $r$ 阶子式不为 0，但并不要求所有的 $r$ 阶子式都不为 0。即至少存在一个不为 0 的 $r$ 阶子式让原式秩保持 $r$

2. $A$ 中一定有 $r-1$ 阶子式不为 0，但并不要求所有的 $r-1$ 阶子式都不为 0

3. 而 $r+1$ 阶子式则必须全为 0

#### 2.5.3 分块矩阵

分块矩阵乘法进行的前提：进行乘法的各分块之间的维度要匹配，在不匹配的时候需要重新划分

1. $AB = O$

    若 $A$ 是 m\*n 矩阵，$B$ 是 n\*s 矩阵且 $AB = O$，对 $B$ 和 $O$ 矩阵按列分块有

    $AB = A[\beta_1, \beta_2,...,\beta_s] = [A\beta_1, A\beta_2,...,A\beta_s] = [0,0,...,0]$

    即 $A\beta_i = 0, i = 1,2,...,s$

    即 $B$ 的列向量是齐次方程组 $Ax = 0$ 的解

2. $AB = C$

    若 $AB = C$，其中 $A$ 是 m\*n 矩阵，$B$ 是 n\*s 矩阵，则对 $B,C$ 按行分块有

    $
    \left(\begin{array}{cccc} 
        a_{11} & a_{12} & \cdots & a_{1n} \\
        a_{21} & a_{22} & \cdots & a_{2n} \\
        \vdots & \vdots & \ddots & \vdots \\
        a_{m1} & a_{m2} & \cdots & a_{mn} \\
    \end{array}\right)\left(\begin{array}{cccc} 
        \beta_{1} \\
        \beta_{2} \\
        \vdots \\
        \beta_{n} \\
    \end{array}\right) = \left(\begin{array}{cccc} 
        \alpha_{1} \\
        \alpha_{2} \\
        \vdots \\
        \alpha_{m} \\
    \end{array}\right)$

    即 $\left\{\begin{array}{l}
        a_{11}\beta_{1} + a_{12}\beta_{2} + ... + a_{1n}\beta_{n} = \alpha_{1} \\
        a_{21}\beta_{1} + a_{22}\beta_{2} + ... + a_{2n}\beta_{n} = \alpha_{2} \\
        ... \\
        a_{m1}\beta_{1} + a_{m2}\beta_{2} + ... + a_{mn}\beta_{n} = \alpha_{m}
    \end{array}\right.$

    可见矩阵 $AB$ 的行向量 $\alpha_{1},\alpha_{2},...,\alpha_{m}$ 可由 $B$ 的行向量 $\beta_{1}, \beta_{2}, ..., \beta_{n}$ 线性表出

    类似得，对 $A,C$ 按列分块

    $
    (\gamma_1, \gamma_2,...,\gamma_n)\left(\begin{array}{cccc} 
        b_{11} & b_{12} & \cdots & b_{1n} \\
        b_{21} & b_{22} & \cdots & b_{2n} \\
        \vdots & \vdots & \ddots & \vdots \\
        b_{m1} & b_{m2} & \cdots & b_{mn} \\
    \end{array}\right) = (\delta_1, \delta_2, ..., \delta_n)$

    即 $\left\{\begin{array}{l}
        b_{11}\gamma_{1} + b_{12}\gamma_{2} + ... + b_{1n}\gamma_{n} = \delta_{1} \\
        b_{21}\gamma_{1} + b_{22}\gamma_{2} + ... + b_{2n}\gamma_{n} = \delta_{2} \\
        ... \\
        b_{m1}\gamma_{1} + b_{m2}\gamma_{2} + ... + b_{mn}\gamma_{n} = \delta_{m}
    \end{array}\right.$

    可见矩阵 $AB$ 的列向量 $\delta_{1},\delta_{2},...,\delta_{m}$ 可由 $A$ 的列向量 $\gamma_{1}, \gamma_{2}, ..., \gamma_{n}$ 线性表出

例：设 $A$ 是 m\*n 矩阵，$B$ 是 n\*s 矩阵，证明秩 $r(AB) \leqslant \min(r(A),r(B))$

法 1：

由于矩阵 $AB$ 的行向量 $\alpha_{1},\alpha_{2},...,\alpha_{m}$ 可由 $B$ 的行向量 $\beta_{1}, \beta_{2}, ..., \beta_{n}$ 线性表出，矩阵 $AB$ 的列向量 $\delta_{1},\delta_{2},...,\delta_{m}$ 可由 $A$ 的列向量 $\gamma_{1}, \gamma_{2}, ..., \gamma_{n}$ 线性表出

所以 $r(AB) \leqslant r(A),r(AB) \leqslant r(B)$

两不等式同时满足即 $r(AB) \leqslant \min(r(A),r(B))$

法 2：

用到线性方程组的知识：

若 $\alpha$ 是方程组 $Bx = 0$ 的一个解，则有 $AB\alpha = A0 = 0$，即 $\alpha$ 也是方程组 $ABx = 0$ 的一个解

那么 $Bx = 0$ 的解集合是 $ABx = 0$ 的解集合的子集

即 $s - r(B) \leqslant s - r(AB)$

即 $r(AB) \leqslant r(B)$

又因为 $r(AB) = r((AB)^T) = r(B^TA^T) \leqslant r(A^T) = r(A)$

两不等式同时满足即 $r(AB) \leqslant \min(r(A),r(B))$

### 2.6 常用结论

## 第三章 向量

### 3.1 向量运算与线性关系

提要：向量的运算 线性表出 线性相关与线性无关

#### 3.1.1 线性相关判定

**1.从齐次线性方程、非齐次线性方程到矩阵方程**

1. 利用齐次线性方程的性质
    
    $\alpha_1,\alpha_2,\cdots,\alpha_m$ 线性相关
    
    <=> 齐次线性方程 $Ax=0$ 有无穷个非零解
    
    <=> $r([\alpha_1,\alpha_2,\cdots,\alpha_n]) < s$

    <=> $|A| = 0$

    $\alpha_1,\alpha_2,\cdots,\alpha_m$ 线性无关
    
    <=> 齐次线性方程 $Ax=0$ 只有零解

    <=> $r([\alpha_1,\alpha_2,\cdots,\alpha_n]) = s$

    <=> $|A| \ne 0$

2. 利用非齐次线性方程的性质

    1. 向量 $\beta \ne 0$ 可由向量组 $\alpha_1,\alpha_2,\cdots,\alpha_n$ 表出
    
        <=> 非齐次线性方程 $Ax = b$ 有解
        
        <=> $r([\alpha_1,\alpha_2,\cdots,\alpha_n])=r([\alpha_1,\alpha_2,\cdots,\alpha_n,\beta])$
        
        此时：

        1. $r([\alpha_1,\alpha_2,\cdots,\alpha_n])=r([\alpha_1,\alpha_2,\cdots,\alpha_n,\beta]) < r$
        
            <=> 非齐次线性方程 $Ax = b$ 有无穷个解，表达式为基础解系

            => 齐次线性方程 $Ax=0$ 有无穷个非零解

        2. $r([\alpha_1,\alpha_2,\cdots,\alpha_n])=r([\alpha_1,\alpha_2,\cdots,\alpha_n,\beta]) = r$
        
            <=> 非齐次线性方程 $Ax = b$ 有唯一解

            => 齐次线性方程 $Ax=0$ 只有零解

    2. 相反地，向量 $\beta \ne 0$ 不能由向量组 $\alpha_1,\alpha_2,\cdots,\alpha_n$ 表出
    
        <=> 非齐次线性方程 $Ax = b$ 无解
        
        <=> $r([\alpha_1,\alpha_2,\cdots,\alpha_n])+1=r([\alpha_1,\alpha_2,\cdots,\alpha_n,\beta])$

    所以已知非齐次解情况能推出齐次解情况，但是反之不能

3. 推广到矩阵方程

    向量组 $\beta_1,\beta_2,\cdots,\beta_l$ 可由 $\alpha_1,\alpha_2,\cdots,\alpha_m$ 线性表示
    
    <=> $AX = B$ 有解 

    <=> $R(A) = R(A, B)$

    => $R(B) \leqslant R(A, B)$ => $R(B) \leqslant R(A)$

    例：一个平面两个基向量，能表示正负 x 轴，正负 x 轴的秩小于一对基向量的秩

**2.定义法**

1. 直接法

    可以直接看出：

    含有零向量、相等向量、坐标成比例的向量组都是线性相关的

    而阶梯形向量组一定是线性无关的

2. 用一个向量组表示一个向量

    $\alpha_1,\alpha_2,\cdots,\alpha_n$ 线性相关 <=> 向量组中至少有一个向量可由其他 $n-1$ 个向量线性表出
    
    $\alpha_1,\alpha_2,\cdots,\alpha_n$ 线性无关 <=> 向量组的任何一个向量都不能被其他 $n-1$ 个向量线性表出

    向量组 $\alpha_1,\alpha_2,\cdots,\alpha_n$ 线性无关，而 $\beta,\alpha_1,\alpha_2,\cdots,\alpha_n$ 线性相关，则 $\beta$ 可由 $\alpha_1,\alpha_2,\cdots,\alpha_n$ 线性表示，且表示方法唯一

3. 用一个向量组表示另一个向量组

    若向量组 $\alpha_1,\alpha_2,\cdots,\alpha_n$ 可由向量组 $\beta_1,\beta_2,\cdots,\beta_s$ 线性表示，且 $n>s$，则 $\alpha_1,\alpha_2,\cdots,\alpha_n$ 线性相关
    
    例：一个平面两个基向量，平面上的向量组的数目大于两个，则线性相关

    若向量组 $\alpha_1,\alpha_2,\cdots,\alpha_n$ 可由向量组 $\beta_1,\beta_2,\cdots,\beta_s$ 线性表示，且 $\alpha_1,\alpha_2,\cdots,\alpha_n$ 线性无关，则 $n\leqslant s$

    例：一个平面两个基向量，这两个基向量线性无关，如果能用一个向量组表示这两个基向量，那么这个向量组的数目一定不少于两个

4. 部分与整体

    向量组 $\alpha_1,\alpha_2,\cdots,\alpha_n$ 存在一部分向量线性相关，则整个向量组线性相关
    
    若 $\alpha_1,\alpha_2,\cdots,\alpha_n$ 线性无关，则任意一部分向量组线性无关

5. 增减维度

    设 $m$ 个 $n$ 维向量 $\alpha_1,\alpha_2,\cdots,\alpha_m$ 线性无关，则把这些向量中每个各任意添加 $s$ 个分量所得到的新向量组（$n+s$ 维）$\alpha_1^*,\alpha_2^*,\cdots,\alpha_m^*$ 也是线性无关的
    
    如果 $\alpha_1,\alpha_2,\cdots,\alpha_m$ 线性相关，则每个各去掉相同的若干分量得到的新向量组也线性相关（原来无关延长无关，原来相关缩短相关）

    n + 1 个 n 维向量必线性相关

#### 3.1.2 线性相关证明

**1.同乘**

若要求线性相关的式子存在一定的乘积关系，则可以用同乘一步步消去系数

例：设 $A$ 是 $n$ 阶矩阵，若存在正整数 $k$，使得线性方程组 $A^kx=0$ 有解向量 $\alpha$，且 $A^{k-1}\alpha\neq0$，证明向量组 $\alpha,A\alpha,\cdots,A^{k-1}\alpha$ 线性无关

证明：假设 $\alpha,A\alpha,\cdots,A^{k-1}\alpha$ 线性相关，则设存在系数 $\lambda_1,\lambda_2,\cdots,\lambda_k$ 使得 $\lambda_1\alpha+\lambda_2A\alpha+\cdots+\lambda_kA^{k-1}\alpha=0$

$\because A^kx=0$ 的解为 $\alpha$，$\therefore A^k\alpha=0$，$\therefore\cdots=A^{k+2}\alpha=A^{k+1}\alpha=A^k\alpha=0$

左乘 $A^{k-1}$，得到 $\lambda_1A^{k-1}\alpha+\lambda_2A^k\alpha+\cdots+\lambda_kA^{2k-2}\alpha=\lambda_1A^{k-1}\alpha=0$

$\because A^{k-1}\alpha\neq0$，$\therefore\lambda_1=0$，消去 $\lambda_1$：$\lambda_2A\alpha+\lambda_3A^2\alpha+\cdots+\lambda_kA^{k-1}\alpha=0$

左乘 $A^{k-2}$，得到 $\lambda_2A^{k-1}\alpha+\lambda_3A^k\alpha+\cdots+\lambda_kA^{2k-3}\alpha=\lambda_2A^{k-1}\alpha=0$

$\because A^{k-1}\alpha\neq0$，$\therefore\lambda_2=0$，消去 $\lambda_2$：$\lambda_3A^2\alpha+\lambda_4A^3\alpha+\cdots+\lambda_kA^{k-1}\alpha=0$

同理依次左乘 $A^n$，所以 $\lambda_1=\lambda_2=\cdots=\lambda_k=0$，所以 $\alpha,A\alpha,\cdots,A^{k-1}\alpha$ 线性无关

---

例：设 $A$ 是 n\*m 矩阵，$B$ 是 m\*n，其中 n < m，若 $AB = E$，证明 $B$ 的列向量线性无关

法 1：同乘

对 $B$ 按列分块，设 $Bx = 0$

对 $AB = E$ 两边同乘 $x$，得 $ABx = Ex = x$

又因为 $A(Bx) = A0 = 0$，所以有 $x = 0$，即 $B$ 的列向量线性无关

法 2：秩

首先，由于矩阵大小限制，$r(B) \leqslant n$

又由 $r(AB)\leqslant\min\{r(A),r(B)\}$ 得 $r(AB) = r(E) = n \leqslant r(B)$

夹逼得 $r(B) = n$，即 $B$ 的列向量线性无关

**2.行列式**

对向量的线性相关性可以从其向量组组成的行列式来计算，若行列式值为0则线性相关，若行列式值不为0则线性无关

注意这里容易失根。要仔细找出所有为0的因式，不要随便降低阶数

例：设 $a_1,a_2,\cdots,a_s$ 是 $s$ 个互不相同的数，探究 $s$ 个 $n$ 维列向量 $\alpha_i=[1,a_i,a_i^a,\cdots,a_i^{n-1}]^T$（$i=1,2,\cdots,s$）的线性相关性

解：当 $s>n$ 时，有 $n$ 个方程 $s$ 个未知数，所以必然存在自由变量，从而必然线性相关性

当 $s=n$ 时，$\vert\alpha_1 \alpha_2 \cdots \alpha_n\vert=\left|\begin{array}{cccc}
    1 & 1 & \cdots & 1 \\
    a_1 & a_2 & \cdots & a_n \\
    \vdots & \vdots & \ddots & \vdots \\
    a_1^{n-1} & a_2^{n-1} & \cdots & a_n^{n-1}
\end{array}\right|=\prod\limits_{1\leqslant j\leqslant i\leqslant n}(a_i-a_j)\neq0$。所以线性无关

当 $s<n$ 时，对方程矩阵切割保留方形的 $s$ 个 $=\left|\begin{array}{cccc}
    1 & 1 & \cdots & 1 \\
    a_1 & a_2 & \cdots & a_n \\
    \vdots & \vdots & \ddots & \vdots \\
    a_1^{n-1} & a_2^{n-1} & \cdots & a_n^{n-1} \\
    \vdots & \vdots & \vdots & \vdots
\end{array}\right|$，上面因为范德蒙德行列式已经不等于 0，即上面的方阵线性无关，原来无关延长无关，所以整个方程都线性无关

综上当 $s>n$ 时线性相关，$s\leqslant n$ 时线性无关

### 3.2 向量组的极大线性无关组与秩

提要：极大线性无关组 向量组的秩

#### 3.2.1 向量组的秩

很多都在前面写的，比如 [>> 3.1.1 线性相关判定](#311-线性相关判定)

1. 秩 = 行秩 = 列秩

2. 初等变换后秩不变

#### 3.2.2 向量组等价

**1.定义**

向量组 $\alpha_1,\alpha_2,\cdots,\alpha_n$ 与 $\beta_1,\beta_2,\cdots,\beta_n$ 等价

<=> 向量组 $\alpha_1,\alpha_2,\cdots,\alpha_n$ 与 $\beta_1,\beta_2,\cdots,\beta_n$ 可以相互线性表示

<=> $R(A) = R(B) = R(A, B)$，其中 $A$ 是向量组 $\alpha_1,\alpha_2,\cdots,\alpha_n$ 组成的矩阵，$B$ 是向量组 $\beta_1,\beta_2,\cdots,\beta_n$ 组成的矩阵

> 矩阵的等价与向量组的等价不是同一个概念！
>
> 矩阵 $A \sim B$ 不能得出 $A$ 的列向量组 $\sim$ B 的列向量组

例：已知 n 维向量组 (i) $\alpha_1,\alpha_2,\cdots,\alpha_s$ 和 (ii) $\beta_1,\beta_2,\cdots,\beta_t$ 的秩都为 r，则下列命题中不正确的是（）

A. 若 s = t，则向量组 (i) 和 (ii) 等价

B. 若向量组 (i) 是 (ii) 的部分组，则向量组 (i) 和 (ii) 等价

C. 若向量组 (i) 能由 (ii) 线性表示，则向量组 (i) 和 (ii) 等价

D. 若向量组 (iii) $\alpha_1,\alpha_2,\cdots,\alpha_s, \beta_1,\beta_2,\cdots,\beta_t$ 的秩为 r，则向量组 (i) 和 (ii) 等价

答案：A

A 指的是矩阵等价的条件而不是向量组等价的条件

反例：

向量组 $
\alpha_1 = \left(\begin{array}{cc}
    1 \\
    0 \\
    0
\end{array}\right), \alpha_2 = \left(\begin{array}{cc}
    0 \\
    1 \\
    0
\end{array}\right)$ 和向量组 $
\beta_1 = \left(\begin{array}{cc}
    0 \\
    1 \\
    0
\end{array}\right), \beta_2 = \left(\begin{array}{cc}
    0 \\
    0 \\
    1
\end{array}\right)$

B C D 都是充分条件

### 3.3 正交化与正交矩阵

提要：Schmidt 正交化 正交矩阵

#### 3.3.1 Schmidt 正交化

设向量组 $\alpha_1, \alpha_2, \alpha_3$ 线性无关，其正交规范化方法步骤如下：

令 $\beta_1 = \alpha_1,$

$\beta_2 = \alpha_2 - \dfrac{(\alpha_2,\beta_1)}{(\beta_1,\beta_1)}\beta_1,$

$\beta_3 = \alpha_3 - \dfrac{(\alpha_3,\beta_1)}{(\beta_1,\beta_1)}\beta_1- \dfrac{(\alpha_3,\beta_2)}{(\beta_2,\beta_2)}\beta_1,$

则 $\beta_1, \beta_2, \beta_3$ 两两正交

再将 $\beta_1, \beta_2, \beta_3$ 单位化

不用死记公式，本质就是把当前向量减去它在各个已知基向量上的投影

<img src = "./orthogonalization.svg" height = 200>

比如实际中如果 $cos<\alpha_1,\alpha_2>$ 方便求就直接求了，$n_1$ 也可以方便求，总之怎么写得顺手怎么来

#### 3.3.2 正交矩阵

$AA^T = A^TA = E$

=> $|A|$ = 1 或 -1

=> $A^{-1} = A^T$

---

例：设 3 阶实矩阵 $A$ 的特征向量为 $\alpha_1 = (-1,1,0)^T,\alpha_2 = (1,1,1)^T,\alpha_3 = (-1,-1,2)^T$，则 $A$ 必为（）

A. 可逆矩阵

B. 正交矩阵

C. 对称矩阵

D. 正定矩阵

答案：C

设 $Q = (\alpha_1, \alpha_2, \alpha_3)$，易知 $Q$ 为正交矩阵

有 $Q^TAQ = \Lambda$ 化为 $A = Q \Lambda Q^T$

即使 $A$ 有三个不同的特征向量，也不能确定 $A$ 是否有特征值 0，因此不能确定 $A$ 是否可逆，A 错 

$AA^T = Q \Lambda Q^T Q \Lambda Q^T = Q \Lambda^2 Q^T$ 不能确定是否等于 $E$，B 错

不能确定 $A$ 的特征值是否全为正，D 错

由 $A$ 的解析式易知 $A = A^T$，C 对

### 3.4 常用结论

## 第四章 线性方程组

### 4.1 有解无解与解的性质

提要：有解无解的判定方法 解的性质与结构定理

有解无解的判定方法在 [>> 3.1.1 线性相关判定](#311-线性相关判定)

#### 4.1.1 解的性质

非齐次通解 = 齐次的通解 + 非齐次一个特解

#### 4.1.2 解的结构

1. 基础解系

    假如 $\xi_1,\xi_2,\cdots,\xi_{n-r}$ 满足：

    1. 是方程组 $Ax=0$ 的解；

    2. 线性无关；

    3. 方程组 $Ax=0$ 的任一解均可由 $\xi_1,\xi_2,\cdots,\xi_{n-r}$ 线性表出
    
    则称 $\xi_1,\xi_2,\cdots,\xi_{n-r}$ 为 $Ax=0$ 的基础解系

    当 $r(A)<n$ 时才讨论基础解系

2. 齐次方程的通解

    设 $\xi_1,\xi_2,\cdots,\xi_{n-r}$ 是 $Ax=0$ 的基础解系，则 $k_1\xi_1+k_2\xi_2+\cdots+k_{n-r}\xi_{n-r}$ 是方程组 $Ax=0$ 的通解，$k_1,k_2,\cdots,k_{n-r}$ 为任意常数

3. 非齐次方程的通解

    $k_1\xi_1+k_2\xi_2+\cdots+k_{n-r}\xi_{n-r} + \eta$

$Ax = b$ 的线性无关的解向量的数目 = 基础解系数目 + 1

$k_1\xi_1+k_2\xi_2+\cdots+k_{n-r}\xi_{n-r} + \eta$ 是方程组 $Ax=b$ 的通解，则 $\xi_1,\xi_2,\cdots,\xi_{n-r},\eta$ 是 $Ax = b$ 的线性无关的解向量

#### 4.1.3 使用非齐次解 1 - 非齐次解 2 = 基础解系时，注意两个非齐次解对应的非齐次项前的系数是相等的

例：$\alpha_1,\alpha_2,\alpha_3$ 是四元非齐次线性方程组 $Ax = b$ 的三个解向量，且 $R(A) = 3,\alpha_1 = (1,2,3,4)^T,\alpha_2+\alpha_3 = (0,1,2,3)^T$，$c$ 表示任意常数，则线性方程组 $Ax = b$ 的通解 $x = $（）

A. $(1,2,3,4)^T + c(1,1,1,1)^T$

B. $(1,2,3,4)^T + c(0,1,2,3)^T$

C. $(1,2,3,4)^T + c(2,3,4,5)^T$

D. $(1,2,3,4)^T + c(3,4,5,6)^T$

答案：C

非齐次解 1 - 非齐次解 2 = 基础解系

基础解系 $\xi = 2\alpha_1 - (\alpha_2+\alpha_3) = c(2,3,4,5)^T$

基础解系再加一个非齐次解 = 通解

注意：**使用非齐次解 1 - 非齐次解 2 = 基础解系这个规律时，需要注意两个非齐次解对应的非齐次项前的系数是相等的**

我也不太会用数学的语言说吧，就是说，$A\alpha_1 = \beta$，但是 $A(\alpha_2+\alpha_3) = 2\beta$

所以为了两个非齐次解相减能得到齐次方程，需要 $\beta$ 前的系数一致，即 $A2\alpha_1 = 2\beta$

这样才有 $A2\alpha_1 - A(\alpha_2+\alpha_3) = 2\beta - 2\beta = 0$，即 $A[2\alpha_1 - (\alpha_2+\alpha_3)] = 0$

#### 4.1.4 n 阶微分方程对应通解中 n 个独立的常数

例：设 $y_1(x)$ 与 $y_2(x)$ 是微分方程 $y'+p(x)y = 0$ 的两个不同的解，则该方程的通解可以表示为（）

A. $C_1 y_1 + C_2 y_2$

B. $y_1 + C (y_1 + y_2)$

C. $y_1 + C y_2$

D. $C(y_2 - y_1)$

答案：D

一阶微分方程的通解中不能含有两个独立的任意常数，A 错

对于 B、C，常数 C = 0 时，只剩下一个 $y_1$，它是方程的一个特解，缺少一个任意常数，故错

排除 A、B、C 只有 D 对

实际上因为 $y'+p(x)y = 0$ 的通解的解析式是 $y = C e^{-\int{p(x)dx}}$

所以任两个解只相差一个常数因子，而 $y_1(x)$ 与 $y_2(x)$ 两个不同的解，故 $y_2 - y_1$ 是方程的一个非零解。所以对于方程的任一个解 $y$，都存在常数 $C$，使 $y = C(y_2 - y_1)$

---

当然也不是什么时候都要用猜的

如果给出了微分方程和解的，带参数的具体解析式，是有可能求出参数，进而求出特征根，确定具体通解的

> 遇到这种题的时候我的脑子却还在想着要猜，于是就错了……
>
> 做题做的人都傻了

### 4.2 线性方程组解的求法

提要：齐次线性方程组基础解系的求法 非齐次线性方程组通解的求法 克拉默法则 公共解与同解问题

#### 4.2.1 齐次线性方程组基础解系的求法

秩为 r 即有效方程的个数为 r

如果 n = r，有唯一确定的解

如果 r < n，则还有 n - r 个变量是不确定的

把它们移到方程右边使得 r 个未知数可由它们表示，这样每个未知数都可由这 n - r 个来表示了

或者说，通过给这 n - r 个赋值来得到基础解系

因此基础解系的个数 s = n - r(A)

基础解系中的所有解都是 $Ax = 0$ 的解，都是特征值 0 对应的线性无关的特征向量

步骤：

1. 将系数矩阵 $A$ 作为 初等行变换后化为阶梯形矩阵或最简阶梯形矩阵 $B$，因为初等行变换将方程组化为同解方程组，所以 $Ax=0$ 与 $Bx=0$ 同解，只需解 $Bx=0$，设 $r(A)=r$。其中 $A$ 为 $m$ 行 $n$ 列，$m$ 为约束方程组个数，$n$ 为变量个数

2. 在 $B$ 中按列找到一个秩为 $r$ 的子矩阵，即在每排阶梯都选出一列组合成子矩阵，则剩余列位置的未知数就是自由变量。（极大线性无关组）

3. 按基础解析定义求出 $\xi_1,\xi_2,\cdots,\xi_{n-r}$，并写出通解

    **自由项的赋值需要保证求得基础解系是线性无关的**

例：求齐次线性方程组 $\left\{\begin{array}{l}
    x_1+x_2-3x_4-x_5=0 \\
    x_1-x_2+2x_3-x_4=0 \\
    4x_1-2x_2+6x_3+3x_4-4x_5=0 \\
    2x_1+4x_2-2x_3+4x_4-7x_5=0
\end{array}\right.$ 的通解

解：系数矩阵 $A=\left(\begin{array}{ccccc}
    1 & 1 & 0 & -3 & -1 \\
    1 & -1 & 3 & -1 & 0 \\
    4 & -2 & 6 & 3 & -4 \\
    2 & 4 & -2 & 4 & -7
\end{array}\right)$，然后对其行变换，得到：

$=\left(\begin{array}{ccccc}
    1 & 1 & 0 & -3 & -1 \\
    0 & -2 & 2 & 2 & 1 \\
    0 & 0 & 0 & 3 & -1 \\
    0 & 0 & 0 & 0 & 0
\end{array}\right)=\left(\begin{array}{ccccc}
    1 & 0 & 1 & 0 & -\dfrac{7}{6} \\
    0 & 1 & -1 & 0 & -\dfrac{5}{6} \\
    0 & 0 & 0 & 1 & -\dfrac{1}{3} \\
    0 & 0 & 0 & 0 & 0
\end{array}\right)$，$r(A)=3$

然后找子矩阵，第一台阶选 $C_1$，第二台阶选 $C_2$ 或 $C_3$，第三台阶选 $C_4$ 或 $C_5$，随便找一个，如 $(C_1,C_2,C_4)$ 为子矩阵，则 $C_3$，$C_5$ 所代表的未知数 $x_3$，$x_5$ 就是自由变量

所以选择两个分量 $\xi_1=(\xi_{11},\xi_{12},\xi_{13},\xi_{14},\xi_{15})^T$ 和 $\xi_2=(\xi_{21},\xi_{22},\xi_{23},\xi_{24},\xi_{25})^T$ 作为基础解系

因为此时选择 $x_3$，$x_5$ 为自由变量，所以 $x_3$ 和 $x_5$ 所对应的 $\xi_{13}$、$\xi_{15}$、$\xi_{23}$、$\xi_{25}$ 可以任意取，但是为了保证秩为2，所以让 $\xi_{13}=1$、$\xi_{15}=0$、$\xi_{23}=0$、$\xi_{25}=1$。这四个分量组成的矩阵线性无关，原矩阵线性无关，延长矩阵线性无关，从而 $\xi_1$ 和 $\xi_2$ 必然线性无关

所以此时已经给定两组解，一种是 $\xi_1$ 的 $x_3=1$，$x_5=0$，另一种是 $\xi_2$ 的 $x_3=0$，$x_5=1$，这样就只有三个未知数和三个方程，分别代入 $A$ 矩阵所代表的方程组中（代入行阶梯矩阵就可以，不用代入最简行阶梯矩阵），解得 $\xi_1$ 和 $\xi_2$

#### 4.2.2 非齐次线性方程组通解的求法

步骤：

1. 写出 $Ax=b$ 的导出方程组 $Ax=0$ 并求出其通解 $k_1\xi_1+k_2\xi_2+\cdots+k_{n-r}\xi_{n-r}$

2. 求出 $Ax=b$ 的一个特解 $\eta$

    **自由项的赋值可以任取，为了方便一般取 0**

3. $Ax=b$ 的通解为 $k_1\xi_1+k_2\xi_2+\cdots+k_{n-r}\xi_{n-r}+\eta$

例：设 $\alpha_1, \alpha_2, \alpha_3, \alpha_4$ 为 4 维列向量，满足 $\alpha_2, \alpha_3, \alpha_4$ 线性无关，且 $\alpha_1 + \alpha_3 = 2\alpha_2$。令 $A = (\alpha_1, \alpha_2, \alpha_3, \alpha_4), \beta = \alpha_1 + \alpha_2 + \alpha_3 + \alpha_4$，求线性方程组 $Ax = \beta$ 的通解

解：

先求 $Ax = 0$ 的基础解系

由于 $\alpha_1 + \alpha_3 = 2\alpha_2$，所以 $R(A) = 3$，所以基础解析的只有一个解向量

又由 $\alpha_1 + \alpha_3 = 2\alpha_2$ 可得 $\alpha_1 - 2\alpha_2 + \alpha_3 + 0\alpha_4 = 0$

所以求得基础解系为 $(1, -2, 1, 0)^T$

再求 $Ax = \beta$ 的特解

由于 $\beta = \alpha_1 + \alpha_2 + \alpha_3 + \alpha_4$ 所以 $(1, 1, 1, 1)^T$ 是一个特解

所以 $Ax = \beta$ 的通解为 $k(1, -2, 1, 0)^T + (1, 1, 1, 1)^T$

> 1.对于抽象的线性方程组，无法利用消元法，即对增广矩阵进行初等变换求解，要考虑利用解的结构求解
>
> 2.要充分理解并灵活运用向量的线性关系与线性方程组的解之间的关系。这是考研的重点

#### 4.2.3 克拉默法则

克拉默法则本来是矩阵中的运算法则，但是与方程组有更密切的关系，所以放到线性方程组中

若 $Ax=b$ 的系数矩阵 $A$ 的行列式 $\vert A\vert\neq0$

则方程有唯一解，且 $x_i=\dfrac{\vert A_i\vert}{\vert A\vert}$

其中 $A_i$ 为把系数矩阵 $A$ 的第 $i$ 列的元素用方程组右侧的常数项代替后所得到的 $n$ 阶矩阵

#### 4.2.4 公共解

1. 如果都给出了方程组的具体形式，不妨设 $Ax = 0$ 和 $Bx = 0$，则有公共非零解 <=> 联立方程组有非零解

2. 如果一个给出了方程组 $Ax = 0$，一个给出了基础解系 $\eta_1, \eta_2, ..., \eta_s$，则有公共非零解 <=> $A\eta_1, A\eta_2, ..., A\eta_s$ 线性相关，通过线性相关的关系设系数，设方程求解

3. 两个都给出了基础解系 $\eta_1, \eta_2, ..., \eta_s$ 和 $\gamma_1, \gamma_2, ..., \gamma_s$，则有公共非零解 <=> $\eta_1, \eta_2, ..., \eta_s, \gamma_1, \gamma_2, ..., \gamma_s$ 线性相关，通过线性相关的关系设系数，设方程求解

#### 4.2.5 同解

若 $A_{m\times n}x=0$ 和 $B_{s\times n}x=0$ 有完全相同的解，就是同解方程组

考虑方程组：(I) $Ax = 0$ (II) $\left\{
   \begin{array}{lcl}
      Ax = 0 \\
      Bx = 0
   \end{array}
   \right.$ (III) $Bx = 0$

则 (I) (II) (III) 同解，故有 $r(A)=r(B)=r([A,B]^T)$

---

例：设 $A$ 是 n 阶实矩阵，$A^T$ 是 $A$ 的转置矩阵。证明：方程组 $Ax = 0$ 和 $A^TAx = 0$ 是同解方程组

证：若已知 $Ax = 0$ 则有 $A^T(Ax) = A^T0 = 0$

若已知 $A^TAx = 0$ 两边左乘 $x^T$，得 $x^TA^TAx = (Ax)^T(Ax) = 0$

取行列式，得 $|(Ax)^T(Ax)| = |(Ax)^T||Ax| = |Ax|^2 = 0$，即 $Ax = 0$

---

例：$Ax = 0$ 与 $Bx = 0$ 同解的充要条件是 $A$ 与 $B$ 等价（）

答案：x

反例：$A = \left(\begin{array}{cc}
        1 & 1 \\
        0 & 0
    \end{array}\right),B = \left(\begin{array}{cc}
        1 & -1 \\
        0 & 0
    \end{array}\right)$，$A,B$ 秩相同，等价，但不同解

---

例：设 $A,B$ 均是 $m \times n$ 矩阵，则方程组 $Ax = 0$ 与 $Bx = 0$ 同解的充分必要条件是（）

A. $A,B$ 的列向量组等价

B. $A,B$ 的行向量组等价

C. $A,B$ 是等价矩阵

D. $A^x = 0$ 与 $B^Tx = 0$ 同解

答案：B

有 $r(A)=r(B)=r([A,B]^T)$ 即 $A,B$ 的行向量组等价，A 错 B 对

C 只给出 $r(A)=r(B)$ 没出现 $r([A,B]^T$，所以是必要不充分条件，C 错

对 D，举反例：

$A = \left(\begin{array}{ccccc}
    1 & 0 & 0 \\
    2 & 0 & 0
\end{array}\right),B = \left(\begin{array}{ccccc}
    2 & 0 & 0 \\
    1 & 0 & 0
\end{array}\right)$

显然，$Ax = 0$ 与 $Bx = 0$ 同解，但 $A^x = 0$ 与 $B^Tx = 0$ 不同解

#### 4.2.6 抽象线性方程

例：设 $A$ 为三阶方阵，$A=(a_{ij})_{3 \times 3}$，且 $a_{ij}=A_{ij}$（$i,j=1,2,3$），其中 $A_{ij}$ 为 $a_{ij}$ 的代数余子式，$a_{33} \neq 0$，$b=(a_{13},a_{23},a_{33})^T$，求非齐次线性方程组 $Ax=b$ 的解。

解：由于是抽象线性方程，所以必须要充分利用方程和矩阵的性质。题目中给出的主要是代数余子式，由行列式的一行或一列的元素乘上对应的代数余子式可得行列式值的性质：

$b$ 为第三列元素，乘上对应的代数余子式得行列式值：$b(A_{13},A_{23},A_{33})=a_{13}A_{13}+a_{23}A_{23}=a_{13}^2+a_{23}^2+a_{33}^2 \geqslant 0$

又 $a_{33} \neq 0$，$\therefore b(A_{13},A_{23},A_{33})= \vert A \vert > 0$

之后就可以用克拉默法则了

### 4.3 常用结论

## 第五章 特征值、特征向量、相似矩阵

### 5.1 特征值与特征向量

#### 5.1.1 特征值的性质

定义：存在 $\lambda$ 满足 $Ax = \lambda x$ <=> $(A-\lambda E)x = 0$

有解的充分必要条件是 $\lvert A-\lambda E \rvert = 0$ 

设 $A=(a_{ij})_{n\times n}$，$\lambda_i$（$i=1,2,\cdots,n$）是 $A$ 的特征值，则：

1. $\sum\limits_{i=1}^n\lambda_i=\sum\limits_{i=1}^n=tr(A)$。主对角线元素和即矩阵的迹

2. $\prod\limits_{i=1}^n\lambda_i=\vert A\vert$

3. $f(A)\xi=f(\lambda)\xi$

4. $A^{-1}\xi=\dfrac{1}{\lambda}\xi$

5. $A^*\alpha=\dfrac{\vert A\vert}{\lambda}\xi$

---

例：设 $A$ 为 3 阶方阵，如果 $A^{-1}$ 的特征值是 1, 2, 3，则 $|A|$ 的代数余子式 $A_{11} + A_{22} + A_{33}$ =

答案：1

$A_{11} + A_{22} + A_{33}$ 是伴随矩阵的迹，所以需要研究伴随矩阵

提到伴随矩阵就不得不提：$AA^* = |A|E$

其中，$|A|$ 可以求，因为 $A^{-1}$ 的特征值是 1, 2, 3，所以 $A$ 的特征值是 1, 1/2, 1/3，因为 $\prod\limits_{i=1}^n\lambda_i=\vert A\vert$，所以 $|A| = \dfrac{1}{6}$

所以 $AA^* = \dfrac{1}{6}E$，所以 $A^* = \dfrac{1}{6}A^{-1}$，所以 $A^*$ 的特征值为 1/6, 1/3, 1/2

又因为 $\sum\limits_{i=1}^n\lambda_i=\sum\limits_{i=1}^n=tr(A)$，所以 $A_{11} + A_{22} + A_{33}$ = 1/6 + 1/3 + 1/2 = 1

#### 5.1.2 特征向量的性质

1. $k$ 重特征值 $\lambda$ 至多只有 $k$ 个线性无关的特征向量。一共有 $k$ 个特征向量

2. 若 $\xi_1$ 和 $\xi_2$ 是 $A$ 的属于不同特征值 $\lambda_1$ 和 $\lambda_2$ 的特征向量，则 $\xi_1$ 和 $\xi_2$ 线性无关

3. 若 $\xi_1$ 和 $\xi_2$ 是 $A$ 的属于同特征值 $\lambda$ 的特征向量，则 $k_1\xi_1+k_2\xi_2$（$k_1k_2$ 不同时为0）仍是 $A$ 的属于特征值 $\lambda$ 的特征向量

4. 若 $A$ 可逆，则 $A$、$A^{-1}$、$A^*$ 的特征向量相同

#### 5.1.3 特征值与特征向量的关系

1. 若特征值不相等，则特征向量线性无关

2. 若特征值相等，则特征向量可能线性相关也可能线性无关

    也可以表述为：$k_i$ 重特征值对应的线性无关特征向量小于等于 $k_i$ 个

### 5.2 特征值与特征向量的计算

#### 5.2.1 定义法

例：$A$ 满足 $A^2 + 2A = 0$，则 $A$ 的特征值是 0, 2

要么就转换为 $\lambda^2 + 2\lambda = 0$

要不就把原式拆成 $A(A+2E) = 0$ => $|A(A+2E)| = 0$ => $|A||A+2E| = 0$ => $|A-0E| = 0$ 或 $|A + 2E| = 0$

#### 5.2.2 具体型

当计算 $\vert\lambda E-A\vert$ 时往往难点就是从多项式中解出 $\lambda$，对于 $f(\lambda)=a_k\lambda^k+\cdots+a_1\lambda+a_0=0$，可以使用试根法：

1. 若 $a_0=0$，$\lambda=0$ 就是其根

2. 若 $a_k+\cdots+a_1+a_0=0$，$\lambda=1$ 就是其根

3. 若 $a_0+a_2+\cdots+a_{2k}=a_1+a_3\cdots+a_{2k-1}$，$\lambda=-1$ 就是其根

4. 若 $a_k=1$，且系数都是整数，则有理根是整数，且均为 $a_0$ 的因子

#### 5.2.3 抽象型

矩阵 | $A$ | $kA$ | $A^k$ | $f(A)$ | $A^{-1}$ | $A^*$ | $P^{-1}AP$ | $A^T$
:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:
特征值 | $\lambda$ | $k\lambda$ | $\lambda^k$ | $f(\lambda)$ | $\lambda^{-1}$ | $\vert A\vert/\lambda$ | $\lambda$ | $\lambda$
特征向量 | $\xi$ | $\xi$ | $\xi$ | $\xi$ | $\xi$ | $\xi$ | $P^{-1}\xi$ | 无关

#### 5.2.4 特殊矩阵

若矩阵 $A$ 为对角线矩阵，则特征值为对角线上元素

若 $n$ 阶矩阵 $A$ 行或列对应成比例，即 $r(A)=1$，则 $\lambda_1=\lambda_2=\cdots=\lambda_{n-1}=0$，$\lambda_n=tr(A)$

#### 5.2.5 注意 A 的特征向量与 A^T 的特征向量无关

例：设 $\lambda = 2$ 是方阵 $A$ 的特征值，对应的特征向量为 $\alpha$，$\mu = 1$ 是 $A^T$ 的特征值，对应的特征向量为 $\beta$，则必有（）

A. $\beta = 2\alpha$

B. $\alpha = 2\beta$

C. $\alpha,\beta$ 线性无关

D. $\alpha$ 与 $\beta$ 正交

答案：D

由定义：

$A\alpha = 2\alpha$

$A^T\beta = \beta$

对第一式两边转置得 $\alpha^T A^T = 2\alpha^T$

两边乘 $\beta$ 得 $\alpha^T A^T \beta = 2\alpha^T \beta$
 
又因为 $A^T\beta = \beta$ 所以上式化为 $\alpha^T \beta = 2\alpha^T \beta$

得 $\alpha^T \beta= 0$ 即 $\alpha$ 与 $\beta$ 正交

> 不记得这个无关的时候，我还以为可以使用“若特征值不相等，则特征向量线性无关”的规律
>
> 实际上是无关的……

#### 5.2.6 两个矩阵有相同的特征值的证明

证明两个矩阵有相同的特征方程 $|\lambda E - A| = 0$

#### 5.2.7 利用特征值/特征向量计算参数

**1.使用特征向量的定义**

例：设 $A = \left(\begin{array}{cc}
        2 & 1 & 1 \\
        1 & 2 & 1 \\
        1 & 1 & 2
    \end{array}\right)$，若 $\alpha = (1,k,1)^T,k>0$ 是 $A^{-1}$ 的特征向量，则 $k = $

根据特征向量的定义有 $A^{-1}\alpha = \lambda \alpha$，其中 $\lambda$ 为 $\alpha$ 对应的特征值

变形为 $A\alpha = \lambda^{-1} \alpha$，解方程求得 $\lambda$ 和 $k$

**2.使用“若特征值不相等，则特征向量线性无关”的规律**

例：设 $A$ 是 $3 \times 4$ 实矩阵，$\lambda$ 是 $AA^T$ 仅有的非零特征值，对应的特征向量为 $\alpha = (-1,1,1)^T$，$k_1,k_2$ 为任意常数，则方程组 $AA^Tx = 0$ 的通解可为（）

A. $k_1(1,1,0)^T + k_2(1,-1,0)^T$

B. $k_1(-1,1,0)^T + k_2(0,1,1)^T$

C. $k_1(-1,1,0)^T + k_2(1,0,1)^T$

D. $k_1(1,1,0)^T + k_2(1,0,1)^T$

答案：D

可知 $AA^T \sim diag(\lambda, 0, 0), \lambda \ne 0$

故特征值 0 与 $\lambda$ 对应的特征向量必正交

则 $x^T\alpha = -x_1+x_2+x_3 = 0$

解得 $x$ 为 $(1,1,0)^T,(1,0,1)^T$

由特征向量的定义，$AA^Tx = 0 \dot x = 0$

因此特征值 0 对应的两个特征向量就是 $AA^Tx = 0$ 的两个基础解系

### 5.3 相似

#### 5.3.1 相似

若存在可逆矩阵 $P^{-1}AP = B$，则称 $A$ 相似于 $B$

#### 5.3.2 相似的性质

1. 反身性：$A\sim A$

2. 对称性：若 $A\sim B$，则 $B\sim A$

3. 传递性：若 $A\sim B$，$B\sim C$，则 $A\sim C$

#### 5.3.3 相似的充要条件

$A\sim B$ <=>

1. $r(A)=r(B)$

2. $\vert A\vert=\vert B\vert$

3. $tr(A)=tr(B)$

4. $\lambda_A=\lambda_B$

    相应的特征向量一般不同

    变形：
    
    1. 特征多项式相同

> 在网上看到一个相似的充要条件是初等因子相同...没看懂说实话

#### 5.3.4 相似的必要条件

> 常常用来判别两个矩阵是否能相似
>
> 判断相似难道要你找合适的可逆矩阵 $P$ 吗？不至于，只需要用必要条件找出不可能的情况就好了
>
> 比如特征值不相等，秩不相等的情况那一看就不可能相似

$A\sim B$ =>

1. 充要条件 $r(A)=r(B)$，$\vert A\vert=\vert B\vert$，$\vert\lambda E-A\vert=\vert\lambda E-B\vert$，$tr(A)=tr(B)$，$A, B$ 具有相同的特征值

    反之不一定成立的例子：$A = \left(\begin{array}{cc}
        0 & 0 \\
        0 & 0
    \end{array}\right),B = \left(\begin{array}{cc}
        0 & 1 \\
        0 & 0
    \end{array}\right),A,B$ 有相同的二重特征值 $\lambda = 0$，但 $A,B$ 不相似，因为对任意 $P$，都有 $P^{-1}AP = P^{-1}OP = O \ne B$

    举反例应举有重特征值的例子，若 $A,B$ 有相同的且均为单根的特征值，则必有 $A \sim B$

2. $AB\sim BA$

    证：$P^{-1}AP = B$ => $P^{-1}A = BP^{-1}$

    代入 $P^{-1}ABP = (P^{-1}A)BP = BP^{-1}BP = BA$

3. $A^2=B^2$ 推广得 $A^m\sim B^m$，$f(A)\sim f(B)$

    证：$A = P^{-1}BP$ => $A^2 = P^{-1}BPP^{-1}BP = P^{-1}B^2P$

4. 若 $A$ 可逆，则 $A^{-1}\sim B^{-1}$，$f(A^{-1})\sim f(B^{-1})$

5. $A^T\sim B^T$，$A^*\sim B^*$

作为对比，只知 $A$ 可逆时，也可推出 $AB \sim BA$

证：$A^{-1}ABA = BA$

#### 5.3.5 相似相关的计算

1. 若 $A\sim B$，则可以使用充要条件：$\vert A\vert=\vert B\vert$，$r(A)=r(B)$，$tr(A)=tr(B)$，$\lambda_A=\lambda_B$，通过等式计算参数

2. 若 $\xi$ 是 $A$ 属于特征值 $\lambda$ 的特征向量，则有 $A\xi=\lambda\xi$，建立若干等式或方程组来计算参数

3. 若 $\lambda$ 是 $A$ 的特征值，则与 $\vert\lambda E-A\vert=0$，通过该等式计算参数

### 5.4 相似对角化

#### 5.4.1 能够对角化的充要条件

$A\sim\Lambda$ <=>

1. $A$ 有 $n$ 个线性无关的特征向量

2. $A$ 对应每个 $k_i$ 重特征值都有 $k_i$ 个线性无关的特征向量

#### 5.4.2 能够对角化的充分条件

$A\sim\Lambda$ <=

1. $n$ 解矩阵 $A$ 有 $n$ 个不同的特征值 => $A$ 有 $n$ 个线性无关的特征向量

2. $A$ 为实对称方阵

> 常用夹逼方法求矩阵为满秩 [>> 2.5.1 矩阵的秩](#251-矩阵的秩)
>
> 求得满秩之后就能求出每个特征值对应的线性无关的特征向量
>
> 然后就能证明矩阵可以对角化

例：设 A 是一个 n 阶方阵，满足 $A^2 = A, R(A) = r$ 且 $A$ 有两个不同的特征值。试证 $A$ 可对角化

由 $A^2 = A$ 得 $A(A-E) = 0$，根据定理，若 $A$ 为 m\*n 矩阵，$B$ 为 n\*s 矩阵，$AB = O$，则 $r(A)+r(B) \leqslant n$，得 $R(A) + R(A-E) \leqslant n$

又根据定理，$r(A+B) \leqslant r(A)+r(B)$，得 $R(E) = n \leqslant R(A) + R(E-A) = R(A) + R(A-E)$

夹逼得 $R(A) + R(A-E) = n$

所以 $R(A) = r, R(A-E) = n-r$，特征值 0 对应的线性无关的特征向量有 r 个，特征值 1 对应的线性无关的特征向量有 n-r 个，总共有 n 个线性无关的特征向量，所以 $A$ 可以对角化

#### 5.4.3 对角化方法

1. 求出 $A$ 的所有特征值 $\lambda$

2. 求出 $A$ 的所有 $\lambda$ 的特征向量 $\xi$

3. 令 $P=(\xi_1,\xi_2,\cdots,\xi_n)$，则 $P^{-1}AP=\Lambda$（$\xi$ 线性无关，$\vert P\vert\neq0$，$P$ 可逆）

#### 5.4.4 实对称矩阵的相似对角化方法

1. 实对称矩阵的特征值全部是实数

2. 实对称矩阵的属于不同特征值对应的特征向量相互正交

    同一特征值对应的不同特征向量也相互正交

故实对称矩阵必然可以相似对角化

步骤

1. 求出 $A$ 的所有特征值 $\lambda$

2. 求出 $A$ 的所有 $\lambda$ 的特征向量 $\xi$

3. 将 $(\xi_1,\xi_2,\cdots,\xi_n)$ 正交化 [>> 3.3.1 Schmidt 正交化](#331-schmidt-正交化)、单位化为 $(\eta_1,\eta_2,\cdots,\eta_n)$

4. 令 $Q=(\eta_1,\eta_2,\cdots,\eta_n)$，则 $Q^{-1}AQ=Q^TAQ=\Lambda$

    注意 $\lambda_i$ 和 $\xi_i$ 的排列顺序一致

其中，正交矩阵：$Q^TQ = E$，得 $Q^T = Q^{-1}$

#### 5.4.5 对阵矩阵的性质

若 $A,B$ 均为 n 阶实对称矩阵，但 $AB$ 不一定是实对称矩阵

例：$A = \left(\begin{array}{cc}
        0 & 0 \\
        0 & 1
    \end{array}\right),B = \left(\begin{array}{cc}
        1 & 1 \\
        1 & 0
    \end{array}\right)$，则 $AB = \left(\begin{array}{cc}
        0 & 0 \\
        1 & 0
    \end{array}\right)$ 不是实对称矩阵

---

例：设 $A,B$ 均为 $n$ 阶实对称矩阵，且都可逆，则下列命题错误的是（）

A. 存在可逆矩阵 $P$，使得 $P^{-1}(A+B)P = \Lambda_1$

B. 存在可逆矩阵 $P$，使得 $P^{-1}(AB)P = \Lambda_2$

C. 存在正交矩阵 $Q$，使得 $Q^T(A^*+B^*)Q = \Lambda_3$

D. 存在正交矩阵 $Q$，使得 $Q^T(A^{-1}+B^{-1})Q = \Lambda_4$

答案：B

由 $A^T = A,B^T = B$ 得 $(A+B)^T = A^T + B^T = A + B$

所以 $A+B$ 也是实对称矩阵，因此可以相似对角化，A 正确

由 $(A^{-1})^T = (A^T)^{-1} = A^{-1}$ 得 $A^{-1}$ 也是实对称矩阵，同理 $B$ 也是实对称矩阵

那么根据选项 A 的证明，$A^{-1}+B^{-1}$，也是实对称矩阵，因此可以相似对角化，D 正确

由 $AA^* = \lvert A \rvert E$ 得 $A^* = \lvert A \rvert A^{-1}$，即 $A^*$ 可用 $A^{-1}$ 表示

那么根据选项 D 的证明，$A^*$ 也是实对称矩阵，同理 $B^*$ 也是实对称矩阵，进一步 $A^*+B^*$ 也是实对称矩阵，因此可以相似对角化，C 正确

$A,B$ 均为 n 阶实对称矩阵，但 $AB$ 不一定是实对称矩阵。对于未知特征向量情况的一般矩阵，无法判断是否能相似对角化，因此 $AB$ 不一定可以相似对角化，B 错误

#### 5.4.6 A 相似于 B，但 A 不能对角化时求解 P^(-1)AP 中的 P 的方法

数学功底不够，标题很丑，不知道怎么总结hhh

A 相似于 B 时，若

1. 可以对角化

    有 $P_1^{-1}AP_1 = \Lambda = P_2^{-1}BP_2$
    
    按照前面所讲的对角化方法求 $P_1,P_2$ 则有 $P = P_2P_1^{-1}$ 使得 $P^{-1}AP = B$

2. 不能对角化
   
    没有 n 个线性无关的特征向量，就构不成一个完整的 $P$

    但是不代表 P 不存在

    可以设 $P = \left(\begin{array}{cc}
        x_1 & x_2 \\
        x_3 & x_4
    \end{array}\right)$，由于 $P^{-1}AP = B$，即有 $AP = PB$

    整理可得关于 x 的齐次线性方程组，解这个方程组，给定 x 的基础解系前的系数，得到 $P$

### 5.5 常用结论

1. 若 $A \sim B$，则 $|B-\lambda E| = |P^{-1}(A - \lambda E)P| = |P^{-1}||A - \lambda E||P| = |A - \lambda E|$

2. 若 $A$ 的每行的行内元素之和都等于 k，则 $A \left(\begin{array}{cc}
        1 \\
        1 \\
        \vdots \\
        1
    \end{array}\right) = k \left(\begin{array}{cc}
        1 \\
        1 \\
        \vdots \\
        1
    \end{array}\right)$

    即 k 是 A 的一个特征值，$\left(\begin{array}{cc}
        1 \\
        1 \\
        \vdots \\
        1
    \end{array}\right)$ 是特征值 k 对应的特征向量

## 第六章 二次型

### 6.1 化二次型为标准形、规范形

提要：标准形 规范形

#### 6.1.1 二次型的矩阵表示

只有当 $A$ 是对称阵时，二次型 $f(x_1,x_2,\cdots,x_n) = x^TAx$ 才和 $A$ 一一对应

$A$ 不是对称阵时，二次型 $f(x_1,x_2,\cdots,x_n) = x^TAx$ 有无穷种表示

设 $f = x^TAx$，有

1. $A = B$ <=> $f = g$

2. $A \simeq B$ <=> $f$ 合同于 $g$

3. $r(A) = r$ <=> $r(f) = r$

4. $A$ 正定 <=> $f$ 正定

例：将二次型 $f(x_1,x_2,x_3) = (ax_1+bx_2+cx_3)^2$ 表示成矩阵形式，其中 $a,b,c$ 不全为 0

简便方法：同一个行列式，可以有不同的矩阵乘法表达

$f(x_1,x_2,x_3) = (ax_1+bx_2+cx_3)^2 \\
= (x_1,x_2,x_3)\left(\begin{array}{cc}
    a \\
    b \\
    c
\end{array}\right)(a,b,c)\left(\begin{array}{cc}
    x_1 \\
    x_2 \\
    x_3
\end{array}\right) \\
= x^T\left(\begin{array}{cc}
    a^2 & ab & ac \\
    ab & b^2 & bc \\
    ac & bc & c^2
\end{array}\right)x$

#### 6.1.2 化二次型为标准形的方法

1. 正交变换

2. 配方法

    1. 若二次型中含有平方项，不妨设 $a_{11} \ne 0$，则对**所有含 $x_1$ 的项**配完全平方

        配方后，其余各项不再含 $x_1$，再配第二个平方项……

        最后对完全平方项换元

    2. 若二次型中没有平方项，只有混合项，不妨设 $a_{12} \ne 0$，则令 $x_1 = y_1 + y_2,x_2 = y_1 - y_2, x_3 = y_3, ..., x_n = y_n$，使二次型中出现 $a_{12}y_1^2-a_{12}y_2^2$，再按法 1 配方

    连续使用法 1 法 2 可以对任意二次型配方

#### 6.1.3 配方法的易错点

1.正交变换与配方法是两个东西

配方得到 $y = C_1x$，容易转换成 $x = C_2y$，然后代入 $f = x^TAx$，就得到 $f = y^TC_2^TAC_2y = y^TBy$，变换就是 $C_2^TAC_2=B$

但是 $C_2$ 不一定是正交矩阵，题目如果要求正交矩阵还得正交化

### 6.2 合同

$C^TAC=B$ <=> $A \simeq B$ <=> $f$ 合同于 $g$

标准形：$A$ 为对角阵

规范形：$A$ 为只含 1, -1, 0 的对角阵

因为 $A$ 为实对称矩阵，所以一定能化为对角阵，所以二次型一定能化为标准形

#### 6.2.1 惯性定理

无论选取什么样的可逆线性变换，**将二次型化为标准形或规范形**，其正项个数 $p$，负项个数 $q$ 都是不变的，$p$ 称为正惯性指数，$q$ 称为负惯性指数

若二次型的矩阵秩为 $r$，则 $r=p+q$，可逆线性变换不改变正负惯性指数

实对称阵 $A \simeq B$ <=> $x^TAx$ 与 $x^TBx$ 有相同的正负惯性指数 => $r(A) = r(B)$

判断两矩阵是否合同时可以使用这个充要条件

> 注意先要**将二次型化为标准形或规范形**，才能用惯性定理！

#### 6.2.2 对称矩阵不与非对称矩阵合同

假设 $A$ 为对称矩阵，$A \simeq B$

那么存在矩阵 $C$ 使得 $C^TAC=B$，那么 $B^T = C^TA^TC = C^TAC = B$

所以与对称矩阵 $A$ 合同的 $B$ 也一定是对称矩阵

### 6.3 正定矩阵与正定二次型

$f(x_1,x_2,\cdots,x_n) = x^TAx > 0$ 为正定二次型，对应的 $A$ 为正定矩阵

对于任意 $x \neq 0$，有 $x^TAx>0$

**1.充要条件**

$f = x^TAx > 0$ <=>

1. $f$ 的正惯性指数 $p=n$，即所有系数全为正

2. 存在可逆矩阵 $D$，使得 $A=D^TD$

3. $A\simeq E$

4. $A$ 的特征值 $\Lambda_i>0$（$i=1,2,\cdots,n$）

5. $A$ 的全部顺序主子式均大于 0

由 1 - i 行和 1 - i 列所确定的子式即为 n 阶行列式的 i 阶顺序主子式

**2.必要条件**

$f = x^TAx > 0$ =>

1. $a_{ii}>0$（$i=1,2,\cdots,n$）

2. $\vert A\vert>0$

---

例：设 $f(x_1,x_2,x_3) = (ax_1 + 2x_2 - 3x_3)^2 + (x_2 - 2x_3)^2 + (x_1 + ax_2 - x_3)^2$ 是正定二次型，则（）

A. $a \ne 1$ 且 $a \ne -\dfrac{1}{2}$

B. $a \ne -1$ 且 $a \ne \dfrac{1}{2}$

C. $a \ne \dfrac{1}{2}$ 且 $a \ne 1$

D. $a \ne \dfrac{1}{2}$ 且 $a \ne 0$

答案：A

已知 $f = x^TAx > 0$

但是 $f(x_1,x_2,x_3) = (ax_1 + 2x_2 - 3x_3)^2 + (x_2 - 2x_3)^2 + (x_1 + ax_2 - x_3)^2 \geqslant 0$

等号成立的条件是各项为 0，设 $C = \left(\begin{array}{cc}
    a & 2 & -3 \\
    0 & 1 & -2 \\
    1 & a & -1
\end{array}\right)$

则等号成立的条件等价于 $Cx = 0$ 有非零解

于是使 $Cx = 0$ 只有零解，等号就一定不成立，就有 $f = x^TAx > 0$

$\lvert C \rvert \ne 0$ 时，$Cx = 0$ 只有零解

解得 $a \ne 1$ 且 $a \ne -\dfrac{1}{2}$

### 6.4 常用结论

1. 二次型最值

    若 $A$ 的特征值大小排序 $\lambda_1\leqslant\lambda_2\leqslant\cdots\leqslant\lambda_n$，则：

    1. $\lambda_1x^Tx\leqslant x^TAx\leqslant\lambda_nx^Tx$

    2. 若 $x^Tx=1$，则 $f_{\min}=\lambda_1$，$f_{\max}=\lambda_n$