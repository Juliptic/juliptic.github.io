---
title: 'Notions of smoothness'
date: 2026-8-16
permalink: /posts/2026/08/smoothness/
tags:
  - algebraic geometry
---

I am writing down the basic theory of smoothness to have an easy refrence. This will mostly just be a summary of vakil chapter 13, but mostly just the results.

Regular at a point p means equality of $$dim A_p=m_p/m_p^2$$

By 13.2.E if $$k$$ is algebraically closed then p is regular iff the jacobian critereon holds.

Regularity is harder to check for no algebraically closed fields, so we make a definition thats consistent in the algebraically closed case, and which is easier to check in the other cases.

Smooth over k (for k any field) means locally finite type and with cover by $$k[x_1,\cdots x_n]/(f_1,\cdots f_r)$$ such that the jacobian criteron holds for all points. 
(It is unclear how we consider the corank for non closed points if we have torsion but I guess it's ok).

By 13.2.H since it is clear that the rank/corank should not change by tensoring up to a field of the same characteristic smoothness can be checked after base change.

Thus $$X_k$$ is smooth iff $$X_{\bar{k}}$$ is smooth. 

By 13.2.I Since the locus where the jacobian matrix is not corank d is an explcit closed subscheme since its the vanishing locus of explicit polynomials coming from determinants of minors, then if we are smooth at all closed points then since closed points are dense we must be closed at all points.

By 13.2.J $$X$$ over k algebraically closed is regular at closed points iff smooth. The argument as we've already seen is that smoothness can be checked at closed points and when our field is algebraically closed the condition for smoothness, which is always just the jacobian critereon, implies regularity. 

So to summarize, smoothness can be checked at closed points and after base change if we care for that.

------
