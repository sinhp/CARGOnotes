---
layout: default
title: The 2-category of toposes
author: Sina Hazratpour
category: research
tags: 
use_math: true
---

{{ page.title }}
================


Toposes, geometric morphisms, and natural transforamtions form a 2-category denoted by $\mathfrak{Top}$. Note that for each pair of toposes $D$, and $E$, $\mathbf{Geom}(D,E)$ is a large though locally small category. 

###Example: 
Suppose $X$ is a (non-T_1) topological space  We define the following (non-trivial) _partial_ order on points of $X$. 
$$ x \leq x' iff every neighbourhood of x contains x'$$. 

We can extend this order to all maps between topological spaces. Suppose $f,g: X \ensuremath{\rightrightarrows} Y$ are (continuous) maps. Define 

$$ f \leq g iff f(x) \leq g(x) for every x \in X $$ 

A ramification of above defintion, which is straightforward to see, is that $f \leq g$ if and only if $f^{-1} (V) \subseteq g^{-1}(V)$ for evey open set $V$ of $Y$.  





