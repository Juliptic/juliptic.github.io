---
title: 'Why Schemes'
date: 2026-09-23
permalink: /posts/2026/09/why-schemes/
tags:
  - Algebraic Geometry
---

Here's a fact I didn't believe when I first read it. The category of rings is complete. 

If you've done a decent amount of algebraic geometry, you should be able to easily remember/guess what a product, coproduct and fibered coproduct in the category of Rings should be, but the notion of a fibered product was never introduced to me on my first pass and so I assumed it didn't exist. It lets you tell a convenient (but horribly incorrect) story about why you need schemes. If you say "Well we have this category of affine schemes but we're missing some colimits"(the objects that should come from gluing affine schemes)" then lets just formally complete the category by introducing these objects" and if you did you would've created the category of schemes. This, as we have just seen is a lie. Instead, let me offer one perspective.

Imagine we have a colimit diagram in the category AffSch. If we want to compute the new affine scheme we should get we could go to the category of rings, compute the limit there and then go back. If we consider the example of maps $$k[y]\to k[x,x^{-1}]$$ and $$k[z]\to k[x,x^{-1}]$$ sending $$y\to x$$ and $$z\to x^{-1}$$ then the limit of these rings should just be $$k$$ and so the colimit in affine schemes should just be a point, but this feels wrong. In AffSch we have two line which we are saying should agree on a big subset each excluding one point from each line, but we are seemingly getting that gluing these together should just be a point. 

The problem here is that if we took a forgetful functor $$AffSch\to Top$$ and then computed the colimit there, we would get a different topological space that what we computed in our first attempt. So to fix this incongruence, we created schemes, which have the topological space we expect.


------
