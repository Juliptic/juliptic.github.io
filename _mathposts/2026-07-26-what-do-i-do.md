---
title: 'What do I do'
date: 2026-07-26
permalink: /posts/2026/07/what_do_I_do/
tags:
  - cool posts
  - category1
  - category2
---

I will attempt to explain what I am currently working on at varying levels of detail.

Non-Math Overview
========

You may have heard before that there are different sizes of infinity. Maybe the best example is the set $$\mathbb{R}$$ of real numbers, the number line, is larger in size than the set $$\mathbb{Q}$$ of rational numbers, those of the form $$\frac{a}{b}$$ where $$a$$ and $$b$$ are whole numbers. What we will take from this is an important fact, if you picked some real numbers at random, ones with tons of decimals and added some of them up, it would be incredibly unlikely that you end up with a rational number. 

What I am working on is proving that some objects, which are defined over the comlpex numbers $$\mathbb{C}$$ but which you can think of as being defined over $$\mathbb{R}$$ can be added up to give an object defined over $$\mathbb{Q}$$, or in this case something close to $$\mathbb{Q}$$. 

This type of result is oftentimes refered to as a rationality result. The actual objects we are dealing with are called cohomolog classes but it easiest to just think of them as functions. 


Full detail
=========

Let $$f$$ be a hilbert modular form associated to a totally real field $$F$$ of degree $$d$$. Assume $$f$$ has weight $$(1,\cdots 1)$$, full level $$SL_{2,F}$$ and is a normalized eigenform with eigenvalues in $$\mathcal{O}_E$$. Assoociated to $$f$$
is a Hilbert modular variety $$X$$ and differential bunde $$\omega$$ such that $$f\in H^1(X,\omega)\otimes \mathcal{O}_E$$. We then have an action of the Hecke algebra on $$H^i(X,\omega)$$ so we can define $$H^i(X,\omega)_f$$ as the subspace of $$H^i(X,\omega)$$ which have the same eigenvalues as $$f$$. It is a theorem that the dimension of this is $$\binom{d}{i}$$. We expect an action of a motivic cohomology group here, which takes the form of an action by the stark unit group $$U_f$$ on $$H^i(X,\omega)_f$$ which shifts the degree and generates all of the cohomology from just the cohomology in degree 0, namely from $$f$$.

We expect this action to preserve rational structures and since we understand that the action can be represented by an associated matrix called the stark regulator matrix $$R_f$$, our conjecture shall be that we can write down explcit linear combinations of cohomology classes over $$\mathbb{C}$$ which are asscoaited to $$f$$, which when scaleed by untis should land in $$H^i(X,\omega)_f\otimes E$$. In degree 1 for example, we expect $$R_f^{-1}\begin{bmatrix} \omega_1\\ \cdots \\ \omega_3  \end{bmatrix}\in H^1{X,\omega}\otimes E$$

Explicitly in te degree 3 conjecture we predict $$R_f^{-1}\begin{bmatrix} \omega_1\\ \omega_2\\ \omega_3  \end{bmatrix}\in H^1{X,\omega}\otimes E$$. This is very difficult in this generalized for so past work has focused on the case where $$f$$ is the base change of a classical modular form $$f_0$$ of weight 1 on $$SL_2$$. We will make the same assumption that our weight $$(1,1,1)$$ form arises from base change, which diagonalizes the matrix when F is galois and simplifies the conjecture to the following

$$\frac{\omega_1+\omega_2+\omega_3}{log|u_{f_0}|}, \frac{\omega_1+\zeta_3\omega_2+\zeta_3^2\omega_3}{log|u_{f_\chi}|}, \frac{\omega_1+\zeta_3^2\omega_2+\zeta_3\omega_3}{log|u_{f_{\chi^2}}|}\in H^1(X,\omega)\otimes E$$

And this is what I will try to prove. The first step should be to use starks conjecture to relate these units to L-values which should make the question purely automorphic. Then figure out how to test rationality of cohomology classes and analyze the explcit connection between $$f$$ and $$f_0$$ through base change, which we will note is exceptional and nonstandard in this case, to hopefully get somewhere.


Questions to have:
=========
How do we view $$f\in H^1(X,\omega)\otimes \mathcal{O}_E$$

How does the hecke algebra act on cohomology. In what general context can we think of a hecke action. I think the answer are most group schemes over $$\mathbb{Q}$$

Why is $$dim H^i(X,\omega)_f=\binom{d}{i}$$

Why does this regulator matrix show up, what are the entries

------
