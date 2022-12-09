## 0 复数
### 0.0 复数

设复数 $ z = a + jb $，其幅角 $ \theta = \arctan{\frac{a}{b}} $，则有 $ z = \lvert z \rvert \mathrm{e}^{j\theta} $

### 0.1 欧拉公式

$$ \mathrm{e}^{jx} = \cos{x} + j \sin{x} $$

则有
$$ \cos{x} = \frac{\mathrm{e}^{jx} + \mathrm{e}^{-jx}}{2} ， \sin{x} = \frac{\mathrm{e}^{jx} - \mathrm{e}^{-jx}}{2j} $$

## 1 信号
### 1.1 单位冲激信号

$$ \delta(at - t_0) = \frac{1}{\lvert a \rvert} \delta(t - \frac{t_0}{a}) $$
$$ x^{(k)}(t - t_0) = x(t) * \delta^{(k)}(t - t_0) $$
$$ x(t) \delta(t - t_0) = x(t_0) \delta(t - t_0) $$
$$ \int^{+ \infty}_{- \infty} \varphi(t) \delta^{(n)}(t - t_0) = (-1)^n \varphi^{(n)} (t_0) $$
$$ f(t) \delta'(t - t_0) = f(t_0) \delta'(t - t_0) - f'(t_0) \delta(t - t_0) $$
$$ \delta^{(n)}(-t) = (-1)^n \delta^{(n)}(t) $$


