# Logistic Regression Cost Function

Loss (error) function:

$$
    L(\hat{y}, y) = -(y\log(\hat{y}) + (1-y)\log(1 - \hat{y}))
$$

Cost function:

$$
    J(\omega, b) = \frac{1}{m}\sum\limits_{i = 1}^{m}
    L(\hat{y}^{(i)}, y^{(i)}) =
    -\frac{1}{m}\sum\limits_{i = 1}^{m}[y^{(i)}\log(\hat{y}^{(i)}) +
    (1-y^{(i)})\log(1 - \hat{y}^{(i)})]
$$
