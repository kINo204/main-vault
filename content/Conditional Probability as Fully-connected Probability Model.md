---
date: 2026-07-02
tags:
  - math
  - bayes
  - probability
---

$$
p(X|Y), ~ X\cap Y=\emptyset
$$

Atomic operations:
- Marginalization, $p(\alpha,\beta|\gamma)\to p(\alpha|\gamma)$
    - $\#(X+Y)\downarrow, ~ \#X\downarrow,~ \#Y-$
    - The conditional context doesn't change
- Conditionalization, $p(\alpha,\beta|\gamma) = p(\alpha|\beta,\gamma)\cdot p(\beta|\gamma)$
    - $\#(X+Y)-, ~ \#X\downarrow,~ \#Y\uparrow$
    - $\beta$ is added to the conditional context

We have the following observations:
- $\#X$ and the total $\#(X+Y)$ always drops; $\#Y$ always rises.
- Each random variable can only cross from left to right, for once.

**T** (representation). Given the total joint distribution $p(\Omega)$, any $p(X|Y)$ can be represented.

**P.** Conditionalize $Y$, leave alone $X$, and marginalize the rest:

$$
\begin{align}
&p(\Omega) \xrightarrow{M} p(X,Y)\\
&p(\Omega) \xrightarrow{M} p(Y) \\
&p(X,Y) \xlongequal{C} p(X|Y)\cdot p(Y)
\end{align}
$$

**T** (representation under conditional context). Given a conditional context $\Theta$ and its total joint distribution $p(\Omega|\Theta)$, distribution $p$ can be represented iff. in the form $p(X|Y,\Theta)$ .

**P.** Conditionalize $Y$, leave alone $X$, and marginalize the rest:

$$
\begin{align}
&p(\Omega|\Theta) \xrightarrow{M} p(X,Y|\Theta)\\
&p(\Omega|\Theta) \xrightarrow{M} p(Y|\Theta) \\
&p(X,Y|\Theta) \xlongequal{C} p(X|Y,\Theta)\cdot p(Y|\Theta)
\end{align}
$$

Additionally, none of the basic operations could eliminate elements in conditional context. Thus only probability with the original condition $\Theta$ in context, i.e. in the form of $p(X|Y,\Theta)$, could be represented.

As is illustrated by the representation theorem, **the Bayesian Probability can be seen as a fully connected probability model**, where any *connection* $p(X|Y)$ is accessible as long as provided with enough information, e.g. from $p(\Omega)$.