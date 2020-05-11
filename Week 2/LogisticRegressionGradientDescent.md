# Logistic Regression Gradient Descent

![Variable notation](images/Annotation%202020-05-09%20181025.png)

![Computation graph](images/Annotation%202020-05-09%20181224.png)

$$
\begin{aligned}
    &"da" = \frac{\delta L(a, y)}{\delta a} = -\frac{y}{a} + \frac{1 - y}{1 - a}
    \\\\
    &"dz" = \frac{\delta L(a, y)}{\delta z} = a - y
    \\\\
    &"dw_1" = \frac{\delta L(a, y)}{\delta \omega_1} = x_1 dz
    \\\\
    &"dw_2" = \frac{\delta L(a, y)}{\delta \omega_2} = x_2 dz
    \\\\
    &"db" = \frac{\delta L(a, y)}{\delta b} = dz
\end{aligned}
$$

`Repeat {`

$\omega_1 \coloneqq \omega_1 - \alpha \times d\omega_1$

$\omega_2 \coloneqq \omega_2 - \alpha \times d\omega_2$

$b \coloneqq b - \alpha \times db$

`}`
