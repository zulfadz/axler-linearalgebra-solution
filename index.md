---
title: "Solutions to Axler's Linear Algebra"
description: "Solutions to linear algebra"
author: "Zul Fadzli"
---
[Home](https://zul.rocks)

Solutions that need polishing are marked 🔄 and unfinished solutions are marked ❎

<a name="toc"></a>

# Table of contents

[Chapter 1](#c1)  | Chapter 2 
:------------ | :-------------
[1a.1](#1a1)  | 
[1a.2](#1a2)  | 
[1a.3](#1a3)  |    
[1a.4](#1a4) ❎ |  

_COUNT: 561-3 = 558 EXERCISES LEFT_




<a name="c1"></a>

## Chapter 1 

<a name="1a1"></a>

### [1a.1](#toc) 

Suppose $a$ and $b$ are real numbers, not both 0. Find real numbers $c$ and $d$ such that:

$$ 1/(a+bi) = c + di$$
  
---

$$\begin{align*}
1/(a+bi)*(a-bi)/(a-bi) & = c+di \\
(a-bi)/(a^2 + b^2) &= c+di 
\end{align*}$$

$\implies c = a/(a^2+b^2)$

$\implies d = -b(a^2+b^2)$

<a name="1a2"></a>

### [1a.2](#toc) 

Show that 

$$ \dfrac{-1+\sqrt{3}i}{2}$$

is a cube root of 1 (meaning that its cube equals 1).
  
---

$$\begin{align*}(\dfrac{-1+\sqrt{3}i}{2})(\dfrac{-1+\sqrt{3}i}{2}) &= \dfrac{1-\sqrt{3}i -\sqrt{3}i-3}{4} \\
&= \dfrac{-2-2\sqrt{3}i}{4}
\end{align*}$$

Multiply again with $\dfrac{-1+\sqrt{3}i}{2}$ leads to

$$\dfrac{2-2\sqrt{3}i+2\sqrt{3}i+6}{8}=1$$

<a name="1a3"></a>

### [1a.3](#toc) 

Find two distinct square roots of $i$.

  
---

Suppose square root of $i$ is $a+bi$. Its square is $$a^2 +2abi-b^2 = 0 +1i.$$

Thus, $a^2 -b^2 =0$ and $2ab = 1$. The first equation tells that $a$ and $b$ has the same magnitude. The second equation tells that they have the same sign. Therefore $a =b$

$\implies 2a^2 =1 \implies a = \pm 1/\sqrt{2}$.

Therefore the square roots of $i$ are $1/\sqrt{2}+1/\sqrt{2}i$ and $-1/\sqrt{2}-1/\sqrt{2}i.$ 

<a name="1a4"></a>

### [1a.4](#toc) 

Show that $\alpha + \beta = \beta+\alpha$ for all $\alpha,\beta \in \mathbf{C}$.

  
---