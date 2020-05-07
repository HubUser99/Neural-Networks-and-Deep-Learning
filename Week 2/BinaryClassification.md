# Binary Classification

![Example 1](images/Annotation%202020-05-07%20201302.png)

## Notation

$(x, y)$ - (feature, label)

$x \in \mathbb{R}^{n_x}$

$y \in \{0, 1\}$

$m$ training examples:
$(x^{(1)}, y^{(1)}), (x^{(2)}, y^{(2)}),\dots,(x^{(3)}, y^{(3)})$

$m = m_{train}$

$m_{test}$ = test example

$$
\begin{aligned}
    &X=\begin{bmatrix}
        | & | && |\\
        x^{(1)} & x^{(2)} & \dots & x^{(m)}\\
        | & | && |
    \end{bmatrix}
    \\\\
    &X \in \mathbb{R}^{n_x*m}
    \\\\
    &Y=[y^{(1)}, y^{(2)},\dots, y^{(m)}]\\\\
    &Y \in \mathbb{R}^{1*m}  
\end{aligned}
$$
