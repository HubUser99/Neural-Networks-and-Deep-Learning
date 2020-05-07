# Logistic Regression

Given $x$, we want:

$\hat{y} = P(y = 1 | x)$, $(0 \le \hat{y} \le 1)$

$x \in \mathbb{R}^{n_x}$

Parameters:

$\omega \in \mathbb{R}^{n_x}$

$b \in \mathbb{R}$

Output:

$\hat{y} = \sigma(\omega^Tx + b)$

![Sigmoid function](images/Annotation%202020-05-08%20000125.png)

$G(z) = \frac{1}{1 + e^{-z}}$

If $z$ is a large number, then:

$G(z) \approx \frac{1}{1 + 0} \approx 1$

If $z$ is a large negative number, then:

$G(z) \approx \frac{1}{1 + e^{-\infty}} \approx 0$
