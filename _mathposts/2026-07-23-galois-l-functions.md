---
title: 'L Functions associated to galois representations'
date: 2026-07-23
permalink: /posts/2026/07/blog-post-1/
tags:
  - cool posts
  - category1
  - category2
---

We review how to construct an L-function from a representation $$ \rho\colon Gal(\bar{K}/K) \to GL(V) $$

Assume that the representation factors through some $$Gal(\bar{K}/K)\to Gal(L/K)\to GL(V)$$, then we can define 
$$L(s,\rho)=\prod_{\mathfrak{p}\subset \mathcal{O}_K}det(1-N(\mathfrak{q})^{-s}\rho(Frob_{\mathfrak{q}}) | V^{I_{\mathfrak{q}}} )^{-1}$$ where $$\mathfrak{q}$$ is an arbitrary prime above $$\mathfrak{p}$$.

We will prove that this definition is well defined. First note that if $$ I_{\mathfrak{p}}\neq \{1\}$$ then for two representatives $$g$$ and $$gh$$ with $$h\in I_{\mathfrak{p}}$$ then $$gh\dot v =g\dot v$$ since $$v\in V^{I_{\mathfrak{p}}}$$ so the action of any two representatives of $$Frob_{\mathfrak{p}}$$ are equal.

Last we must check our definition is well defined for primes $$\mathfrak{q}$$ over $$\mathfrak{p}$$. The idea is that since all primes above $$\mathfrak{p}$$ are conjugate, then we have that 

#We get conjugate inertia grops with the conjugate element giving an isomorphism, #which won't change the characteristic polynomial.

------
