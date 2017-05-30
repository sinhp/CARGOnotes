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

Lifting of paths and homotopies written in terms of $2$-functor $\Pi$ yields that $e/P: e/\Pi(E) \to p(e)/\Pi(B)$ is an isomorphism of groupoids for any point $e \in E$, and furthermore the functor $\Pi(p): \Pi(E) \to \Pi(B)$ is surjective on objects. 

This motivates us to define the notion of _Covering functors_ of groupoids: For groupoids $\cat{E}$ and $\cat{B}$, a functor $P: \cat{E} \to \cat{B}$ is a covering functor if 
  1. it is surjective on objects 
  2. $e/\cat{E} \to P(e)/\cat{B}$ is  isomorphism of categories. 
  
**Remark**: For any groupoid $\cat{E}$, there is only a unique morphism between any two objects of $e/\cat{E}$. So, isomorphism of such coslice categories means  isomorphism of their object sets. 

**Remark**: If the groupoid $\cat{E}$ is connected then it is sufficient to check the second condition of covering only for a single object $e$ of $\cat{E}$.  

<div style="text-align:center"><img src="{{ site.baseurl }}/assets/2017-05-29/Grpd-conj.JPG" alt="Groupoid conjugation" > </div>






[1]: https://www.math.uchicago.edu/~may/CONCISE/ConciseRevised.pdf
