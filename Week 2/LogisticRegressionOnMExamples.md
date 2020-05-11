# Logistic regression on m examples

`#Initialize variables`

$J = 0$

$d\omega_1 = 0$

$d\omega_2 = 0$

$db = 0$

`for i = 0 to m {`

$z^{(i)} = \omega^Tx^{(i)} + b$

$a^{(i)} = \sigma(z^{(i)})$

$J += -[y^{(i)}\log a^{(i)} + (1 - y^{(i)})\log(1 - a^{(i)})]$

$dz^{(i)} = a^{(i)} - y^{(i)}$

$d\omega_1 += x_1^{(i)} dz^{(i)}$

$d\omega_2 += x_2^{(i)} dz^{(i)}$

...

$db += dz^{(i)}$

`}`

$J /= m$

$d\omega_1 /= m$

$d\omega_2 /= m$

$db /= m$

$\omega_1 = \omega_1 - \alpha \times d\omega_1$

$\omega_2 = \omega_2 - \alpha \times d\omega_2$

$b = b - \alpha \times db$
