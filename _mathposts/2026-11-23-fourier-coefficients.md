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
>1(Modular with Respect to $$\Gamma$$): $$\forall \gamma=\begin{bmatrix}a&b\\ c&d\end{bmatrix} \in \Gamma$$, $$f(\gamma z)=j(\gamma,z)^{k}f(z)$$ where $$j(\gamma,z)=cz+d$$\
>2: Holomorphic on $$\mathbb{H}$$\
>3(Holomorphic at $$\infty$$): For $$q=e^{2\pi i z} $$ we have a fourier expansion as $$f(z)=\sum_{n\in \mathbb{Z}} a_n q^n$$ and that $$a_n=0$$ if $$n<0$$

This definition is only for modular forms with respect to the full sugroup $$\Gamma=SL_2(\mathbb{Z})$$. Before we discuss the correct definition for congruence subgroups, we should remark about how we achieve our fourier expansion. We have $$\begin{bmatrix}1&1\\0&1 \end{bmatrix} \in SL_2(\mathbb{Z}$$ which acts via $$z\to z+1$$ thus $$f(z)=f(z+1)$$ so modular forms of level $$SL_2(\mathbb{Z})$$ are periodic with period 1, so by general fourier analysis have an expansion as $$f(z)=\sum_{n\in \mathbb{Z}} a_n e^{2\pi i n z}$$ where $$a_n=e^{2\pi n y}\int_0^1f(x+iy)e^{-2\pi i nx}dx$$. We should really think of $$e^{2\pi i z}$$ as a character coming out of the fourier expansion rather than first thinking of it as a coordinate $$q$$.

In order to define modular forms with respect to congruence subgroups, it is fruitful to define an action of $$GL_2(\mathbb{Q})^+$$ on the space of holomorphic functions on $$\mathbb{H}$$.

> Proposition: If $$f$$ is a modular form of weight $$k$$ and level $$\Gamma$$ and $$\rho \in GL_2(\mathbb{Q})^+$$, then $$f|_{\rho}(z)=det(\rho)^{k/2}j(\rho,z)^{-k}f(\rho z)$$ is a modular with respect to $$\rho^{-1}\Gamma\rho$$.
[Add Proof]

> Proposition: With the setup above, if $$\Gamma$$ is a congruence subgroup then $$\rho^{-1}\Gamma\rho^{-1}$$ is also a congruence subgroup
[Add Proof]

Looking forward, we want our modular forms to be function on $$\Gamma \\ \mathbb{P}^1(\mathbb{C})$$ and our boundary will end up being $$\Gamma \\ \mathbb{P}^1(\mathbb{Q})$$ which will be finite. A representative of each orbit $$\alpha_i$$ is called a cusp. Since  $$SL_2{\mathbb{Z}}$$ acts transitively we can find some $$\rho$$ such that $$\rho \alpha_i=[0,1]=\infty$$. 

Thus $$f\vert_{\rho^{-1}}(z)$$  is modular with respect to $$\rho\Gamma\rho^{-1}$$ which is a cogruence subgroup containing some $$\begin{bmatrix}1&M \\ 0&1 \end{bmatrix}$$ thus we get periods of size $$M$$ and a fourier expansion $$f(z)=\sum_{n\in \mathbb{Z}} a_n e^{2\pi i nz/M}$$. We define a modular for to be holomorphic at a cusp if the fourier coefficients in this expansion vanish for $$n<0$$.

Remark: The same definitions work for $$\Gamma$$ a subgroup of $$SL_2(\mathbb{R})$$ which has finite volume and with cusps being representatives of $$\Gamma \\ \mathbb{P}^1(\mathbb{R})$$. The action described on the space of holomorphic functions by $$GL_2(\mathbb{Q})^+$$ extends to $$Gl_2(\mathbb{R})^+$$. 

We mean that a modular form $$f$$ with respect to a general congruence subgroup $$\Gamma\subset SL_2(\mathbb{R})$$ with finite volume is one with satisfies modularity with respect to our subgroup, is holomorphic on $$\mathbb{H}$$ and is holomorphic at the cusps of $$\Gamma \\ \mathbb{P}^1(\mathbb{R})$$ by translating each to $$\infty=[0,1]$$ with some $$\rho \in GL_2(\mathbb{R})^+$$ then expanding $$f\vert_{\rho^{-1}}(z)$$ which will be a congruence subgroup with respect to $$\rho\Gamma\rho^{-1}$$ which will still be a finite volume subgroup[Check this] and will contain some $$\begin{bmatrix}1&t\\ 0&1 \end{bmatrix}$$ for a real $$t$$ and then we can expand as before and consider the condition on the fourier coefficients.

It is clear in both these scenarios that if we start with a modular form with respect to $$\Gamma$$ then our action preserves modularity, holomorphy on $$\mathbb{H}$$ and holormophy at $$\infty$$ since if we could already translate cusps to be holomoprhic then we can just translate the cusps of the new function to those same places. Thus we have an action of $$GL_2(\mathbb{Q})^+$$ (or more generally $$GL_2(\mathbb{R})^+$$) on the space of modular forms of fixed level which changes the congruence subgroup. In the sequel to this post we can continue this story to define Hecke Operators but for now we will be happy knowing how to define modular forms with respect to congruence subgroups.

>New Definition: A modular form with respect to a congruence subgroup $$\Gamma(M)$$ and level $$k$$ is a function $$f: \mathbb{H}\to \mathbb{C}$$ which is 
>1: Modular with respect to $$\Gamma(M)$$ 
>2: Holomorphic on $$\mathbb{H}$$
>3: Holomorphic at the cusps. 

These functions have fourier expansions at $$\infty$$ as $$f(z)=\sum_{n\geq 0} a_n e^{2\pi i nz/M}$$

For $$GL_n$$ more generally, we have a Whitaker expansion.

Lets check for $$SL_2$$ that the Whitaker expansion collapses back to our classical fourier expansion.



------
