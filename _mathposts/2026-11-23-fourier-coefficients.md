---
title: 'Fourier Coefficients of Modular Forms'
date: 2026-11-23
author_profile: false
permalink: /posts/2026/11/fourier-coefficients/
tags:
  - Number Theory
  - Automoprhic Representations
---

When you first learn about modular forms, from the jump one immediately decomposes them with a fourier expansion. 

>Definition: A modular form of weight $$k$$ level $$\Gamma=SL_2(\mathbb{Z})$$ is a function $$\mathbb{H}\to \mathbb{C}$$ which is 
>1(Modular with Respect to $$\Gamma$$): $$\forall \gamma=\begin{bmatrix}a&b\\c&d\end{bmatrix} \in \Gamma$$, $$f(\gamma z)=(cz+d)^{k}f(z)$$\
>2: Holomorphic on $$\mathbb{H}$$\
>3(Holomorphic at $$\infty$$): For $$q=e^{2\pi i z} $$ we have a fourier expansion as $$f(z)=\sum_{n\in \mathbb{Z}} a_n q^n$$ and that $$a_n=0$$ if $$n<0$$\

This definition is only for modular forms with respect to the full sugroup $$\Gamma=SL_2(\mathbb{Z})$$. Before we discuss the correct definition for congruence subgroups, we should remark about how we achieve our fourier expansion.We have $$\begin{bmatrix}1&1\\0&1 \end{bmatrix}\in SL_2(\mathbb{Z)$$ which acts via $$z\to z+1$$ thus $$f(z)=f(z+1)$$ so modular forms of level $$SL_2(\mathbb{Z})$$ are periodic with period 1, so by general fourier analysis have an expansion as $$f(z)=\sum_{n\in \mathbb{Z}} a_n e^{2\pi i z}$$ where $$a_n=e^{2\pi n y}\int_0^1f(x+iy)e^{-2\pi i nx}dx$$. We should really think of $$e^{2\pi i z}$$ as a character coming out of the fourier expansion rather than first thinking of it as a coordinate $$q$$.




For $$GL_n$$ more generally, we have a Whitaker expansion.

Lets check for $$SL_2$$ that the Whitaker expansion collapses back to our classical fourier expansion.



------
