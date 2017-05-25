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
### What are Kan extensions?

Suppose for a $2$-category $\frk{M}$, $1$-cells $F$ and $G$ are given as follows.  
<div style="text-align:center"><img src="{{ site.baseurl }}/assets/2017-05-22/LiftingMonads-1.JPG" alt="right Kan extension-1" > </div>

**The question:** _Is there any $1$-cell $K$ such that $K \oo F =G$ ?_ 

The answer to this depends on the structure of $2$-category $\frk{M}$. But, generically the answer is no. Take the mother $2$-category $\Cat$ of categories. Take two distinct morphisms $g$ and $h$ in $A$ in such a way that $F(g)= F(h)$ but $G(g) \neq G(h)$. Any other functor $K$ will preserve the equality of $F(g)$ and $F(h)$. On the other hand, $G$, which preserve ditinction of $g$ and $h$, cannot be written as composition of functors $F$ and $K$. 


Okay, the first attempt to find a solution $K$ for filling the diagram above has failed. But, do not worry! We can use the $2$-cells in our $2$-category $\frk{M}$ to find the best possible approximation to such a solution. This approximation can be achieved from two different directions; left and right. And this is the basic idea of Kan extension. 


A _right Kan extension of $F$ along $G$_ is the following data: 
  1. a $1$-cell $K: B \to E$
  2. a $2$-cell $\ep: KF \To G$ 
   
 univeral among such data. 
   
<div style="text-align:center"><img src="{{ site.baseurl }}/assets/2017-05-22/LiftingMonads-2.JPG" alt="right Kan extension-2" > </div>

Note that such a $1$-cell $K$ must be unique up to unique isomorphism. Hence we denote it by $Ran_{F} G$ 

#### Note: 

In the case that the $2$-category $\frk{M}$ is poset-enriched we get familiar cancellation rule corresponding to the right Kan extension:

$$\Updownarrow \frac{KF \leq G}{K \leq Ran_{F} G}$$

And for the left Kan extension, we get: 

$$\Updownarrow \frac{G \leq KF}{Lan_{F} G \leq K}$$


##### Remark: 
Limit of a diagram $G: \cat{A} \to \cat{E}$ is obtained as the right extension of $G$ along the unique functor $!: \cat{A} \to 1$. Similarly, colimit of a diagram $G: \cat{A} \to \cat{E}$ is obtained as the left extension of $G$ along the unique functor $!: \cat{A} \to 1$.  

##### Remark: 
$\lang Lan_{F} G, \eta \rang$ is the initial object in the comma category $G/\str{F}$, and  $\lang Ran_{F} G, \eta \rang$ is the terminal object in the comma category $\str{F}/G$ 





**************************************************************



Let $F: \cat{A} \to \cat{B}$ be a functor. For any other category $\cat{E}$, define the functor
$F^{\ast}:  \fun(\cat{B}, \cat{E}) \to \fun(\cat{A}, \cat{E})$ by precomposition with $F$. 


#### Proposition:

$F^{\ast}$ has a right adjoint if and only if the right extensions of functors $G: \cat{A} \to \cat{E}$ along $F$ exists for all $G$.   
Moreover, the evaluation of this right adjoint at $G: \cat{A} \to \cat{B}$ yields $Ran_{F} G$. 

Similarly, $F^{\ast}$ has a left adjoint if and only if the left extensions of functors $G: \cat{A} \to \cat{E}$ along $F$ exists for all $G$. Moreover, the evaluation of this left adjoint at $G: \cat{A} \to \cat{B}$ yields $Lan_{F} G$. 




*****************************************************************


Suppose $P$ is a presheaf on a ctaegory $\cat{C}$. We would like to compute the left extension of $P$ along $F$ (given above).  


div style="text-align:center"><img src="{{ site.baseurl }}/assets/2017-05-22/Left-ext-presheaf.JPG" alt="Left-ext-presheaf" > </div>















[1]: assets/2017-05-22/kan-ext-notes-2017-04-12.pdf
