---
layout: post
title: Lifting of monads to Grothendieck toposes
author: Sina Hazratpour
category: Cargo notes
use_math: true
comments: true
---

{{ page.title }}
================


{% include macros %}



Suppose $T: \cat{C} \to  \cat{C}$ is a monad on $\cat{C}$. We are intereted in answering the question that under which conditions on $\cat{C}$ it is possible to lift $T$ to $\psh{C}$ and to $\sh{C}$. In order to answer this question, in this post I am going to highlight some of relevant defintions and results that are elaborated in my [notes][1]. 

----------------------------------------------------------   
### Basic definitions and results

Suppose for a $2$-category $\frk{M}$, $1$-cells $F$ and $G$ are given as follows.  
<div style="text-align:center"><img src="{{ site.baseurl }}/assets/2017-05-22/LiftingMonads-1.JPG" alt="right Kan extension" > </div>

**The question:** _Is there any $1$-cell $K$ such that $K \oo F =G$ ?_ 

The answer to this depends on the structure of $2$-category $\frk{M}$. But, generically the answer is no. Take the mother $2$-category $\Cat$ of categories. Take two distinct morphisms $g$ and $h$ in $A$ in such a way that $F(g)= F(h)$ but $G(g) \neq G(h)$. Any other functor $K$ will preserve the equality of $F(g)$ and $F(h)$. On the other hand, $G$, which preserve ditinction of $g$ and $h$, cannot be written as composition of functors $F$ and $K$. 


Okay, the first attempt to find a solution $K$ for filling the diagram above has failed. But, do not worry! We can use the $2$-cells in our $2$-category $\frk{M}$ to find the best possible approximation to such a solution. This approximation can be achieved from two different directions; left and right. And this is the basic idea of Kan extension. 


A _right Kan extension of $F$ along $G$_ is the following data: 

   -a $1$-cell $K: B \to E$
   -a $2$-cell $\delta: KF \To G$ 
   
 univeral among such data. 
   
<div style="text-align:center"><img src="{{ site.baseurl }}/assets/2017-05-22/LiftingMonads-2.JPG" alt="right Kan extension" > </div>

Note that such a $1-cell $K$ must be unique up to unique isomorphism. Hence we denote it by $Ran_{F} G$ 


**************************************************************




[1]: assets/2017-05-22/kan-ext-notes-2017-04-12.pdf
