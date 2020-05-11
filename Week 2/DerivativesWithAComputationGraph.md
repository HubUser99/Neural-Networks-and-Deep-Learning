# Derivatives with a computation graph

Let function $J(a, b, c)$ be:

$$
    J(a,b,c) = 3(a + bc)
$$

then we can denote variables $u, v, J$ as:

$$
\begin{aligned}
    &u = bc\\
    &v = a + u\\
    &J = 3v
\end{aligned}
$$

![Computation graph](images/Annotation%202020-05-09%20173308.png)

---

Let's calculate $\frac{\delta J}{\delta v}$:

$J = 3v$

$v = 11 \leadsto 11.001$

$J = 33 \leadsto 33.003$

$\rArr \frac{\delta J}{\delta v}$ = 3

Similarly we can compute $\frac{\delta J}{\delta a}$:

$a = 5 \leadsto 5.001$

$v = 11 \leadsto 11.001$

$J = 33 \leadsto 33.003$

$\rArr \frac{\delta J}{\delta a}$ = 3

---

Chain rule:

$\frac{\delta J}{\delta a} = \frac{\delta J}{\delta v} \frac{\delta v}{\delta a}$

$\frac{\delta J}{\delta v} = 3$

$\frac{\delta v}{\delta a} = 1$

$\rArr \frac{\delta J}{\delta a} = 3 \times 1$ = 3

---

Let's calculate derivative $\frac{\delta J}{\delta u}$:

$u = 6 \leadsto 6.001$

$v = 11 \leadsto 11.001$

$J = 33 \leadsto 33.003$

$\rArr \frac{\delta J}{\delta u}$ = 3

Let's calculate last derivative $\frac{\delta J}{\delta b}$:

$b = 3 \leadsto 3.001$

$u = b \times c = 6 \leadsto 6.002$

$\frac{\delta J}{\delta u} = 3$

$\rArr \frac{\delta J}{\delta b} = \frac{\delta J}{\delta u} \frac{\delta u}{\delta b} = 6$
