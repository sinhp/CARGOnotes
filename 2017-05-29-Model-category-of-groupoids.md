---
layout: post
title: Model category of groupoids
author: Sina Hazratpour
category: Cargo notes
use_math: true
comments: true
---

{{ page.title }}
================


{% include macros %}



## The fundamental groupoid $2$-functor 

There is a strict $2$-fucntor $\Pi : \top \to \grpd$ which associates to every topological space its fundamental groupoid, to a continuous map of spaces, a functor of groupoids, and to a homotopy of maps, an iso natural transformation. Let's see how this works in more details: 

 
We recall from algebraic topology that a continuous map $p:E \to B$ is said to be a _covering map_ (or space $E$ a covering space over $B$) whenever for every $x \in B$ there is an open neighbourhood $U$ containing $x$ such that $p^{-1} (U) = \amalg_{i \in I} V_i$, a disjoint union of open sets $V_i$ in $E$ such that $ p|_{V_i}: V_i \cong U $. 
One handy example of a covering map is the quotient map $\bb{R}^2 \to \bb{T}$ where the torus $\bb{T}$ is obtained as the quotient space of $\bb{R}^2$ by identifying $(x,y) \sim (x+m, y+n)$ for every $m, n \in \bb{Z}$. Another well-known examples is the helix-shaped real line $\bb{R}$ over $1$-sphere $\bb{S}^{1}$.   

**Remark:**  If $f : A \to B$ is a map  whereby $A$ is path connected then the pullback of $p$ along $f$, that is $\str{f}p $ is
a covering map. 


There is fundamental lifting type theorem associated to covering maps; **the unique path lifting theorem**. You can find its proof in section 3.2. of Peter May's [A Concise Course in Algebraic Topology][1]. 

Lifting of paths and homotopies written in terms of $2$-functor $\Pi$ yields that $e/P: e/\Pi(E) \to p(e)/\Pi(B)$ is an isomorphism of groupoids and furthermore the functor $P: \Pi(E) \to \Pi(B)$ is surjective on objects. 





[1]: https://www.math.uchicago.edu/~may/CONCISE/ConciseRevised.pdf
