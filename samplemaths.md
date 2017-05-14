---
layout: post
title: "Sample maths"
author: Sina Hazratpour
use_math: true
---

##Sample maths 
================
  

When $a \ne 0 $, there are two solutions to $$ax^2 + bx + c = 0$$ and they are
$$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$ 
      
\begin{align}
    |\psi_1\rangle = a|0\rangle + b|1\rangle \\\\
    |\psi_2\rangle = c|0\rangle + d|1\rangle
\end{align}

\begin{equation} %diagram 4
\begin{tikzcd}[column sep = large]
&& D \arrow[dddl, bend right= 15, swap, "x"] \arrow[dd, "y"] \arrow[dddr, bend left=15, "m"] \\ 
\\
&& g^*(E) \arrow[dl, near start, dotted, swap, "l(\alpha)"] \arrow[dr,"p^*g"] \arrow[dd]  \arrow[rd, phantom, bend right= 25, ""{name=qux}] \\
& f^* (E) \arrow[rr, crossing over, bend right=15, near end,swap, "p^*f"] \arrow[rr, bend left=1, phantom, ""{name=baz}] \arrow[dd, swap, "f^*p"] \arrow[dr, phantom, bend left= 5,""{name=waldo}] \arrow[dr, phantom, bend right= 55, ""{name=fred}] & & E  \arrow[dd, "p"]  \arrow[Rightarrow, from=baz, to=qux, swap, "\altil" ] \arrow[Rightarrow, from=fred, to=waldo, swap, "\iso" ] \\
&& A \arrow[dl, equal, ""{name=foo}] \arrow[rd, near start, "g"]\arrow[dl, phantom, bend left=25, ""{name=alex}] \arrow[dr, phantom, bend right=25, ""{name=bar}] & &  \\
& A \arrow[rr, swap, bend right=15,  "f", ""{name=alfred}] \arrow[rr, swap, bend left=1, phantom, ""{name=hoax}]   & & B \arrow[from=uu, crossing over] 
\arrow[Rightarrow, from=hoax, to=bar, swap, "\alpha"]\\
\end{tikzcd}
\end{equation}
