## 1 常用等价无穷小

当 $ x \rightarrow 0 $ 时，
##### (1)

$$ x \sim \sin{x} \sim \tan{x} \sim \arctan{x} \sim \arcsin{x} \sim \ln{(1+x)} \sim \mathrm{e}^x -1 $$

##### (2)
$$ (1+x)^\alpha -1 \sim \alpha x，1 - \cos{x} \sim \frac{1}{2}x^2，a^x - 1 \sim x \ln{a} $$

##### (3)
$$ x - \sin{x} \sim \frac{x^3}{6}，\arctan{x} - x \sim \frac{x^3}{6}，\tan{x} - x \sim \frac{x^3}{3}，x - \arctan{x} \sim \frac{x^3}{3}，x - \ln{(1+x)} \sim \frac{x^2}{2} $$

##### (4)
若 $ \alpha{x} \rightarrow 0 $，$ \alpha(x) \beta(x) \rightarrow 0 $，则
$$ [1 + \alpha(x)]^{\beta(x)} - 1 \sim \alpha(x) \beta(x) $$

## 2 泰勒公式

#### 2.1 泰勒定理
设 $n$ 是一个正整数，若一个定义域包含 $a$ 的函数 $f(x)$ 在 $a$ 点处 $n+1$ 次可导，那么对于定义域上的任意 $x$，都有：
$$ f(x) = f(a) + \frac{f'(a)}{1!} (x-a) + \frac{f^{(2)}(a)}{2!} (x-a)^2 + \cdots + \frac{f^{(n)}(a)}{n!} (x-a)^n + R_n(x) $$

#### 余项
##### 皮亚诺余项
$$ R_n(x) = o[(x-a)^n] $$

##### 拉格朗日余项
$$ R_n(x) = \frac{f^{(n+1)}(\theta)}{(n+1)!} (x-a)^{(n+1)}，\theta \in (a, x)$$

#### 2.2 常用泰勒公式
皮亚诺余项，且 $ x_0 = 0 $

##### (1)
$$ \mathrm{e}^x=1+x+\frac{x^2}{2!}+\cdots+\frac{x^n}{n!}+o(x^n) $$
$$ \sin{x} = x - \frac{x^3}{3!} + \cdots + (-1)^{n-1} \frac{x^{2n-1}}{(2n-1)!} + o(x^{2n-1}) $$
$$ \cos{x} = 1 - \frac{x^2}{2!} + \cdots + (-1)^n \frac{x^{2n}}{(2n)!} + o(x^{2n}) $$
$$ \ln{(1+x)} = x - \frac{x^2}{2} + \cdots + (-1)^{n-1} \frac{x^n}{n} +o(x^n) $$
$$ (1+x)^\alpha = 1 + \alpha x + \alpha (\alpha - 1) \frac{x^2}{2!} + \cdots + [\alpha (\alpha-1) \cdots (\alpha-n-1)] \frac{x^n}{n!} + o(x^n) $$

##### (2)
$$ \tan{x} = x + \frac{x^3}{3} + o(x^3) $$
$$ \arcsin{x} = x + \frac{x^3}{6} + o(x^3) $$
$$ \arctan{x} = x - \frac{x^3}{6} + o(x^3) $$

## 3 求导公式
|$ C' = 0 $|$ (x^\alpha)' = \alpha x^{\alpha-1} $|$ (a^x)' = a^x \ln{(a)} $|$ (e^x)' = e^x $|
|:-:|:-:|:-:|:-:|
|$ (\log_a{x})' = \frac{1}{x} \cdot \frac{1}{\ln{a}} $|$ (\ln{\lvert x\rvert})' = \frac{1}{x} $|$ (sin{x})' = cos{x} $|$ (cos{x})' = -sin{x} $|
|$ (\tan{x})' = \sec^2{x} = \frac{1}{\cos^2{x}} $|$ (\cot{x})' = -\csc^2{x} = - \frac{1}{\sin^2{x}} $|$ (\sec{x})' = \sec{x} \tan{x} = \frac{\sin{x}}{\cos^2{x}} $|$ (\csc{x})' = -\csc{x} \cot{x} = \frac{\cos{x}}{\sin^2{x}} $|
|$ (\arcsin{x})' = \frac{1}{\sqrt{1 - x^2}} $|$ (\arccos{x})' = 1 - \frac{1}{\sqrt{1-x^2}} $|$ (\arctan{x})' = \frac{1}{1 + x^2} $|$ (\mathrm{arccot}x)' = - \frac{1}{1 + x^2} $|

## 4 部分基本积分公式

$$ \int \sec^2{x} \mathrm{d} x = \int \frac{1}{\cos^2{x}} \mathrm{d}x = \tan{x}+C $$
$$ \int \csc^2{x} \mathrm{d} x = \int \frac{1}{\sin^2{x}} \mathrm{d}x = -\cot{x}+C $$
$$ \int \sec{x} \tan{x} \mathrm{d} x = \int \frac{\sin{x}}{\cos^2{x}} \mathrm{d}x = \sec{x}+C = \frac{1}{\cos{x}}+C $$
$$ \int \csc{x} \cot{x} \mathrm{d} x = \int \frac{\cos{x}}{\sin^2{x}} \mathrm{d}x = -\csc{x}+C = \frac{1}{\sin{x}}+C $$
$$ \int \sec{x} \mathrm{d} x = \int \frac{1}{\cos{x}} \mathrm{d} x = \ln{\lvert \sec{x} + \tan{x} \rvert} + C = \ln{\lvert \frac{1+\sin{x}}{\cos{x}} \rvert} + C $$
$$ \int \csc{x} \mathrm{d} x = \int \frac{1}{\sin{x}} \mathrm{d} x = -\ln{\lvert \csc{x} + \cot{x} \rvert} + C = -\ln{\lvert \frac{1+\cos{x}}{\sin{x}} \rvert} + C $$
$$ \int \frac{\mathrm{d}x}{a^2+x^2} = \frac{1}{a} \arctan{\frac{x}{a}} +C $$
$$ \int \frac{\mathrm{d}x}{a^2-x^2} = \frac{1}{2a} \ln{\lvert \frac{a+x}{a-x} \rvert} +C $$
$$ \int \frac{\mathrm{d}x}{\sqrt{a^2+x^2}} = \arcsin{\frac{x}{a}} +C $$
$$ \int \frac{\mathrm{d}x}{\sqrt{x^2+a^2}} = \ln{\lvert x + \sqrt{x^2+a^2} \rvert} +C $$
$$ \int \frac{\mathrm{d}x}{\sqrt{x^2-a^2}} = \ln{\lvert x + \sqrt{x^2-a^2} \rvert} +C $$

