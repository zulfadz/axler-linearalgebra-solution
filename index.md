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
[1a.4](#1a4) |  
[1a.5](#1a5) |  
[1a.6](#1a6) |  
[1a.7](#1a7) |  
[1a.8](#1a8) |  
[1a.9](#1a9) | 
[1a.10](#1a10) |   
[1a.11](#1a11) |  
[1a.12](#1a12) |  
[1a.13](#1a13) |  
[1a.14](#1a14) |  
[1a.15](#1a15) |  
[1a.16](#1a16) |  

_COUNT: 561-16 = 545 EXERCISES LEFT_




<a name="c1"></a>

## Chapter 1 

<a name="1a1"></a>

### [1a.1](#toc) 

Suppose $a$ and $b$ are real numbers, not both 0. Find real numbers $c$ and $d$ such that:

$$ 1/(a+bi) = c + di$$
  
---

$$\begin{align*}
(1/(a+bi))((a-bi)/(a-bi)) & = c+di \\
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

Trivial. Apply the definition of addition in $\mathbf{C}$.

 <a name="1a5"></a>

### [1a.5](#toc) 

Show that $(\alpha + \beta) + \lambda = \alpha +(\beta+\lambda)$ for all $\alpha,\beta, \lambda \in \mathbf{C}$.

  
---

Let $\alpha = a+bi$, $\beta = c+di$ and $\lambda = e+fi$, for $a,b,c,d,e,f \in \mathbf{R}$.

$$\begin{align*}
(\alpha + \beta) + \lambda &= ((a+bi)+(c+di)) +(e+fi) \\
&= ((a+c)+(b+d)i) +(e+fi) \text{  by definition of addition in $\mathbf{C}$}\\
&= ((a+c)+e)+(((b+d)+f)i) \text{  by definition of addition in $\mathbf{C}$}\\
&= (a+(c+e))+((b+(d+f))i) \text{  by definition of associativity in $\mathbf{R}$}\\
&= (a+bi)+((c+e)+(d+f)i) \text{  by definition of addition in $\mathbf{C}$}\\
&= (a+bi)+((c+di)+(e+fi)) \text{  by definition of addition in $\mathbf{C}$}\\
&=\alpha + (\beta +\lambda)
\end{align*}$$

 <a name="1a6"></a>

### [1a.6](#toc) 

Show that $(\alpha\beta)\lambda = \alpha(\beta\lambda)$ for all $\alpha,\beta, \lambda \in \mathbf{C}$.

  
---

Let $\alpha = a+bi$, $\beta = c+di$ and $\lambda = e+fi$, for $a,b,c,d,e,f \in \mathbf{R}$.

$$\begin{align*}
(\alpha\beta)\lambda &= [(a+bi)(c+di)](e+fi) \\
&= [(ac-bd)+(ad+bc)i](e+fi) \text{  by definition of multiplication in $\mathbf{C}$}\\
&= [(ac-bd)e-(ad+bc)f]+[((ac-bd)f+(ad+bc)e)i]\text{  by definition of multiplication in $\mathbf{C}$}\\
&=[ace-bde-adf-bcf] +[acf-bdf+ade+bce]i \text{  by definition of distributive in $\mathbf{R}$}\\
&=[(ace-adf)-(bcf+bde)]+[(acf+ade)+(bce-bdf)]i \text{  by definition of associativity in $\mathbf{R}$}\\
&= [a(ce-df)-b(cf+de)]+[a(cf+de) + b(ce-df)]i\text{  by definition of distributive in $\mathbf{R}$}\\
&= (a+bi)[(ce-df)+(cf+de)i] \text{  by definition of multiplication in $\mathbf{C}$}\\
&= (a+bi)[(c+di)(e+fi)] \\
&=\alpha(\beta\lambda)
\end{align*}$$

<a name="1a7"></a>

### [1a.7](#toc) 

Show that for  every $\alpha \in \mathbf{C}$, there exists a unique $\beta \in \mathbf{C}$ such that $\alpha + \beta = 0.$

  
---

Let $\alpha = a+bi$, for $a,b,=\in \mathbf{R}$. There exists a unique $-a$ and $-b$ such that $a-a=0$ and $b-b=0$ by property of real numbers.

Thus $\beta = -a - bi$, and we are done.

<a name="1a8"></a>

### [1a.8](#toc) 

Show that for  every $\alpha \in \mathbf{C}$, there exists a unique $\beta \in \mathbf{C}$ such that $\alpha + \beta = 0.$

---

Trivial. Follow same steps as 1a.7. If $a \neq0$, then there exists $1/a$. If $b \neq0$, then there exists $1/b$.

<a name="1a9"></a>

### [1a.9](#toc) 

Show that for  $\lambda(\alpha+\beta) = \lambda\alpha + \lambda\beta$ for all $\lambda, \alpha, \beta \in \mathbf{C}$.

---

$$\begin{align*}
\lambda(\alpha + \beta) &= (e+fi)[(a+bi)+(c+di)] \\
&= [e+fi][(a+c)+(b+d)i]  \text{  by definition of addition in $\mathbf{C}$}\\
&=[e(a+c)-f(b+d)]+[e(b+d)+f(a+c)]i \text{  by definition of multiplication in $\mathbf{C}$} \\
&=[ea+ec-fb-fd]+[eb+ed+fa+fc]i \text{  by definition of distributive in $\mathbf{R}$}\\
&=[(ea-fb)+(ec-fd)]+[(eb+fa)+(fc+ed)]i \text{  by definition of associativity in $\mathbf{R}$}\\
&=[(ea-fb)+(eb+af)i]+[(ec-fd)+(fc+ed)]i \text{  by definition of addition in $\mathbf{C}$}\\
&= (e+fi)(a+bi) + (e+fi)(c+di) \text{  by definition of multiplication in $\mathbf{C}$}\\
&=\lambda\alpha + \lambda\beta
\end{align*}$$

<a name="1a10"></a>

### [1a.10](#toc) 

Find $x \in \mathbf{R}^{4}$ such that 

$$(4,-3,1,7)+2x = (5,9,-6,8)$$

---

$2x = (1,12,-7,1)$

$x = (1/2,6,-7/2,1/2)$

<a name="1a11"></a>

### [1a.11](#toc) 

Explain why there does not exist $\lambda \in \mathbf{C}$ such that

$$\lambda(2-3i,5+4i,-6+7i) = (12-5i,7+22i,-32-9i)$$

---
Suppose there is such $\lambda$. Then

$$\lambda(2-3i)=12-5i$$

and


$$\lambda(5+4i) = 7+22i$$

which means

$$(2-3i)(7+22i) = (2-3i)\lambda(5+4i) = (12-5i)(5+4i)$$

The first term is equal to $14+66-21i+44i =80+23i.$ The last term is equal to $60+20-25i+48i=80+32i$. So consistent.

Repeat the steps above with the following instead:

$$\lambda(-6+7i) = -32-9i$$

which means

$$(2-3i)(-32-9i) =(2-3i)\lambda(-6-7i) =(12-5i)(-6-7i)$$

The first term is equal to $-64-27+96i-18i=-91+78i$. The last term is equal to $-72-35+30i-84i=-107-54i$. Contradiction.

<a name="1a12"></a>

### [1a.12](#toc) 

Show that $(x+y)+z=x+(y+z)$ for all $x,y,z \in F^{n}$

---

$$\begin{align*}
((x_1,...,x_n) + (y_1,...,y_n))+(z_1,...,z_n) &= (x_1+y_1,...,x_n+y_n)+(z_1,...,z_n)\\
&=((x_1+y_1)+z_1,...,(x_n+y_n)+z_n)\\
&=(x_1+(y_1+z_1),...,x_n+(y_n+z_n))\\
&=(x_1,...,x_n)+(y_1+z_1,...,y_n+z_n)\\
&=(x_1,...,x_n)+((y_1,...,y_n)+(z_1,...,z_n))\\
&=x+(y+z)
\end{align*}$$

<a name="1a13"></a>

### [1a.13](#toc) 

Show that $(ab)x = a(bx)$ for all $x\in F^{n}$ and all $a,b \in F$.

---

$$\begin{align*}
(ab)(x_1,...,x_n) &= ((ab)x_1,...,(ab)x_n) \\
&=((a)(bx_1),...,(a)(bx_n))\\
&=a(bx_1,...,bx_n)\\
&=a(b(x_1,...,x_n)\\
&=a(bx)
\end{align*}$$

<a name="1a14"></a>

### [1a.14](#toc) 

Show that $1x = x$ for all $x\in F^{n}$.

---

$1(x_1,...,x_n)=(1x_1,...,1x_n)=(x_1,...,x_n) = x$

<a name="1a15"></a>

### [1a.15](#toc) 

Show that $\lambda(x+y) = \lambda x + \lambda y$ for all $\lambda\in F$ and all $x,y \in F^n$.

---

$$\begin{align*}
\lambda ((x_1,...,x_n) + (y_1,...,y_n)) &= \lambda(x_1 +y_1,...,x_n + y_n) \\
&=(\lambda (x_1+y_1),..., \lambda (x_n+y_n))\\
&= (\lambda x_1 + \lambda y_1,..., \lambda x_n + \lambda y_n)\\
&= (\lambda x_1,...,\lambda x_n)+ (\lambda y_1,...,\lambda y_n)\\
&=\lambda (x_1,...,x_n) + \lambda (y_1,...,y_n) \\
&=\lambda x + \lambda y\\
\end{align*}$$

<a name="1a16"></a>

### [1a.16](#toc) 

Show that $(a+b)x = ax+bx$ for all $a,b,\in F$ and all $x\in F^n$

---

$$\begin{align*}
(a+b)x &= (a+b)(x_1,...,x_n) \\
&=((a+b)x_1,...,(a+b)x_n)\\
&=(ax_1+bx_1,...,ax_n+bx_n)\\
&=(ax_1,...,ax_n) + (bx_1,...,bx_n)\\
&=a(x_1,...,x_n) + b(x_1,...,x_n)\\
&= ax+bx
\end{align*}$$

