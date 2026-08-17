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

Smooth of dim d over k (for k any field) means locally finite type and with cover by $$k[x_1,\cdots x_n]/(f_1,\cdots f_r)$$ such that the jacobian is corank d for all points. 
(It is unclear how we consider the corank for non closed points if we have torsion but I guess it's ok).

By 13.2.H since it is clear that the rank/corank should not change by tensoring up to a field of the same characteristic smoothness can be checked after base change.

Thus $$X_k$$ is smooth iff $$X_{\bar{k}}$$ is smooth. 

By 13.2.I Since the locus where the jacobian matrix is not corank d is an explcit closed subscheme since its the vanishing locus of explicit polynomials coming from determinants of minors, then if we are smooth at all closed points then since closed points are dense we must be closed at all points.

By 13.2.J $$X$$ over k algebraically closed is regular at closed points iff smooth. The argument as we've already seen is that smoothness can be checked at closed points and when our field is algebraically closed the condition for smoothness, which is always just the jacobian critereon, implies regularity. 

So to summarize, smoothness can be checked at closed points and after base change if we care for that.

Next we define a smooth morphism of relative dim d. A map $$f\colon X\to Y $$ is smooth if there exists a cover by affines $$U_i$$ and $$V_i$$ such that $$f(U_i)\subset V_i$$ with $$V_i=Spec B$$
and $$U_i$$ being the open subscheme of some $$Spec B[x_1\cdots x_{d+r}]/(f_1,\cdots f_r)$$ given by the determinant of the jacobian matrix of the first r variables being invertible.

As a remark we note that the whole jacobian matrix is d+r by r, thus at most is rank r and our condition exactly forces it to be rank r. Thus corank d.

Thus it is clear, up to some arguments about dimension, that a smooth morphism to $$Spec k$$ is equivalent to our previous notion of smoothness.

One can then check that this notion of smooth morphism forms a reasonable class (In fact I should do this here)


We would like to give equivalent conditions to a morphism being smooth, namely some fiberwise criteria. To do this we need flatness

A map $$f\colon X \to Y$$ is flat if $$\mathcal{O}_{X,x}$$ is a flat module over $$\mathcal{O}_{Y,f(x)}$$ for all points $$x\in X$$.

We note that if X and Y are affine then because one can check flatness locally at all points then our map is flat iff the map on global rings is flat. Thus if we have an affine morphism flatness can be checked on a cover and its imeeditaley true for all covers. 

We note that free modules are flat and that locally,  free is equivalent to projective which is equivalent to flat.  

Thus we note flatness for a coherent sheaf is equivalent to being locally free.

So if we have a cover such that each map $$Spec A\to Spec B$$ is free, or really just flat, then our map is flat.

The result above should prove that smooth maps are flat, as locally they look like $$W\to Spec B$$ where W (I think) should be a free module.

Now we note that smoothness is equivalent to the relative sheaf of differentials being locally free, which gives use the leverage to get a local condition. 

If a map is smooth then its clear the fibers are all smooth by the fact the localization of the sheaf of kahler differentials will be free, and by the above smooth implies flat.

Thus smooth implies smooth fibers and flat, 24.8 in Vakil proves that this condition is sufficient as well.

Now we get to the question of how to check smoothness locally. Because we are working over a residue field we can just use the jacobian criteron and classic understanding and be fine.

We also need to check the map is flat. (Write down how to do that)

------