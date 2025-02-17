# 高等数学A

----

## 1.1函数

### 一.函数的定义和基本特征

#### 定义：

​	设 $D$ 是一个实数集 $R$ 内的一个非空数集，从 $D$ 到 $R$ 的任意一个映射 $f$ 称为定义在 $D$ 上的一个`一元函数` 简称 `函数`$f$, 记作
$$
y = f(x), x \in D
$$
#### 基本元素定义：

* 设 $X$ 和 $Y$ 是两个非空集合，存在一个法则 $T$ ，使得 $X$ 中的每一个元素 $x$ 按照法则 $T$ 在 $Y$ 中有唯一的元素 $y$ 与之对应，那么称 $T$ 为从 $X$ 到 $Y$ 的`映射`
* $x$ 被称为`自变量`
* $y$ 称为函数的`因变量`
* $D$ 称为函数 $f$ 的`定义域`
* $f(D) = \{f(x)|x \in D\}$ 称为函数的`值域`
* 在平面 $R^2$ 中的点集 $\{(x,y)|y = f(x),x \in D\}$，称为函数 $y = f(x)$ 的`图像`

#### 自然定义域定义：

在数学中，不考虑函数的实际意义，只抽象研究数学表达式，且该函数的定义域就是使得算式有意义的一切实数组成的集合，则我们称函数的定义域为`自然定义域`

#### 分段函数定义：

在该函数的定义域内的不同部分，对应法则由不同的算式表达，这种函数被成为`分段函数`，$(-\infty, x_1]$ 被称为`分段区间`，$x1$ 被称为 `分段点`

#### 函数的基本性质：

* **有界性**：

  存在上下界就称函数有界

  设函数 $f(x)$ 的定义域为 $D$，有数集 $X \subset D$,如果存在正数 $M$，使得任意一数 $x \in X$, 都满足
  $$
  |f(x)| \leq M
  $$
  就称函数 $f$ 在 $X$ 上有上界，否则如果 $M$ 不存在就称 $f$ 在 $X$ 上无界

* **单调性**：

  设 $x_1$ 和 $x_2$ 在函数的定义域上，当
  $$
  x_1 < x_2
  $$
  

  总有
  $$
  f(x_1) < f(x_2)
  $$
  则称函数 $f$ 在该区间单调递增，

  反之当
  $$
  x_1 < x_2
  $$
  

  总有
  $$
  f(x_1) > f(x_2)
  $$
  则称函数 $f$ 在该区间单调递减

  单调增加或者减少的函数都叫做`单调函数`

* **奇偶性**：

  设函数 $f(x)$ 关于原点对称，即函数在定义域 $D$ 中 $x \in D$ 时必有 $-x \in D$，如果对于任意的 $x$,总有
  $$
  f(x) = f(-x)
  $$
  则称 $f(x)$ 是偶函数

  如果总有
  $$
  f(x) = -f(-x)
  $$
  则称 $f(x)$ 是奇函数

* **周期性**：

  设 $f(x)$ 的定义域为 $D$, 如果存在不为0的 $T$，使得对每一个 $x \in D$ ，有$x \pm T \in D$, 且总有 $f(x + T) = f(x)$, 就称 $f(x)$ 是`周期函数`，$T$ 称做 $f(x)$ 的周期， $T$ 为`最小正周期`



#### 小知识点:

* 任何一个函数都可以被分解为一个奇函数和一个偶函数的和， 证明见附录 [任何函数是奇偶函数和证明](#jump1)
* 狄利克雷函数(有理数为1，无理数为0)   函数图像见附录 [狄利克雷函数图像](#jump2)
* 函数和方程概念不同，$y = x^2$ 属于函数和方程， $x = y^2$ 就不属于函数但是属于方程，函数只能是一个 $y$ 对应多个 $x$

### 二.函数的运算以及初等函数

#### 四则运算：

设函数 $y = f(x)$ 和 $y = g(x)$ 的定义域分别是 $D_f$ 和 $D_g$ 若 $D_f \cap D_g \ne \oslash$ 可在 $D = D_f \cap D_g$ 上定义这两个函数的和，差，积，商

| 运算法则 | 式子                                              |
| -------- | ------------------------------------------------- |
| 和       | $(f+g)(x) = f(x) + g(x), x \in D$                 |
| 差       | $(f-g)(x) = f(x) - g(x), x \in D$                 |
| 积       | $(f \cdot g)(x) = f(x) \cdot g(x), x \in D$       |
| 商       | $为({f \over g})(x) = {f(x) \over g(x)}, x \in D$ |

#### 复合运算：

复合函数通常记为$(f \circ g)(x) = f[g(x)]$

#### 反函数：

设函数 $f$ 

满足条件：

*  $D \to R$ 为单射（即任意的 $x_1,x_2$ 都有 $f(x_1) \neq f(x_2)$）



反函数性质：

* 关于直线 $y = x$ 对称

* 单调函数一定存在反函数

  

通常称函数 $f$ 的反函数为 $f^{-1}$, 由对应关系可得
$$
x = f^{-1}(y)
$$
习惯上又把该式子记为
$$
y = f^{-1}(x)
$$
注意此处的 $y$ 和 $x$ 非前式子的 $y$ 和 $x$ 

以下有一些例子：

* $y = x^{3}$ 的反函数为 $x = y^{1 \over 3}, y \in R$, 常写为 $y = x^{1 \over 3}, x \in R$

* $\sin x$ 在其定义域上 $R$ 不存在反函数，但是定义在一定区间内如 $I = [-{\pi \over 2}, {\pi \over 2}]$ 上就是个单调函数，反函数记为 $y = \arcsin x$, 定义域为 $[-1, 1]$ ， 值域为 $[-{\pi \over 2}, {\pi \over 2}]$

  

#### 初等函数：

* **幂函数** $y = x^{\mu}$
* **指数函数** $y = a^x$, （$a$ 为正常数，且 $a \neq 1$）
* **对数函数** $y = \log_{a}{x}$ （$a$ 为正常数，且 $a \neq 1$）
* **三角函数** 正弦函数 $\sin x$ , 余弦函数 $\cos x$, 正切函数 $\tan x = {\sin x \over \cos x}$, 余切 $\cot x = {\cos x \over \sin x}$, 正割函数 $\sec x = {1 \over \cos x}$ , 余割函数 $\csc x = {1 \over \sin x}$
* **反三角函数** 反正弦函数 $\arcsin x$, 反余弦函数 $\arccos x$, 反正切函数 $\arctan x$, 反余切函数 $\newcommand{\arccot}{\mathrm{arccot}\,}\arccot x$



#### 小知识点：

* 典型代表的初等函数图像  函数图像见附录[初等函数图像集](#jump3) 

### 三.习题

​	

## 1.2 极限的定义

### 一. 数列极限的定义

### 二. 函数极限的定义

#### 定义：

​	设 $f(x)$ 在去心领域 $\mathring{U}(x_0, \delta_0)$ 内有定义，如果存在常数 $A$ 使得对任意给定的正数 $\varepsilon$ 总存在正数 $\delta(\delta < \delta_0)$ , 只要点 $x$ 满足不等式 $0 < |x - x_0| < \delta$， 对应的函数值 $f(x)$ 就满足
$$
|f(x) - A| < \varepsilon
$$
常数 $A$ 记作 $f(x)$ 当 $x \to x_0$ 的极限， 记为
$$
\lim\limits_{x \to x_0}f(x) = A
$$

## 1.3 极限的性质和运算法则

### 一.极限的性质



### 二.极限的运算法则

#### 小知识点：

* 在极限的式子中 $1^\infty \neq 1$, 在高等数学中 $1^\infty$ 是一个极限未定式，需要用 $u^v = e^{v \cdot \ln u}$ 公式来破解

### 三.习题

例题1. 函数 $f(x) = \lim\limits_{n\to \infty} {{x^{2 n}- 1} \over {x^{2 n} + 1}}$ 的间断点是 ?    [例题1答案](#1.3_problem1)

例题2. $x = 0$ 是函数 $\arctan{1 \over x}$ 的什么点 ?      [例题2答案](#1.3_problem2)

例题3. $\lim\limits_{n \to \infty} {3^n \sin{x \over 3^n}}$ 等于多少 ？              [例题3答案](#1.3_problem3)

例题4. $\lim\limits_{n \to \infty}{\sqrt{n}(\sqrt{n + 1} - \sqrt{n})}$              [例题4答案](#1.3_problem4)

例题5. $\lim\limits_{x \to \infty}({{x+a} \over {x-a}})^x = 9$, 请问 $a$ 等于多少 ？    [例题5答案](#1.3_problem5)  

例题6. $\lim\limits_{x \to 0}{{5x-\sin^2{x}-2x^3} \over {\tan x + 4x^2}}$ 等于多少 ？            [例题6答案](#1.3_problem6)

## 1.4 极限存在的准则与两个重要极限

### 一.两个准则和一个原理

#### 夹逼准则

#### 单调有界收敛准则

#### 柯西收敛原理

#### 小知识点

* 函数在某一点极限存在的充要条件： 函数左极限与函数右极限存在且相等

### 二.两个重要极限

由两个准则推导得出

* $\lim\limits_{x \to 0}{\sin x \over x} = 1$
* $\lim\limits_{x \to \infty}(1 + {1 \over x})^x = e$

## 1.5 无穷小以及无穷小的比较

### 一. 无穷小与无穷大

#### 定义：

* 无穷小：

​	当 $x \to x_0$ 时函数 $\alpha(x)$ 的极限为 $0$ 

### 二. 无穷小的比较

#### 条件：

* 非 $0$ 无穷小，即不包含常数 $0$

#### 比较：

设 $\alpha$ 和 $\beta$ 是 $x \to x_0$ 时的无穷小

![2023-02-26 19-37-32屏幕截图](https://s2.loli.net/2023/02/26/TnPuMrOZFEzYRpD.png)

## 1.6 函数的连续性和连续函数的运算

### 一.函数的连续性

#### 定义：

设函数 $f(x)$ 满足以下条件：

* $f(x)$ 在 $x_0$ 处有定义
* $\lim\limits_{x \to x_0}f(x)$ 极限存在
* $\lim\limits_{x \to x_0}f(x) = f(x_0)$

则称函数 $f(x)$ 在点 $x_0$ 处连续

### 二.函数的间断点

* 判断是否是间断点

  ![2023-02-15 20-11-24屏幕截图](https://s2.loli.net/2023/02/15/KRJjqx3lcomn2tQ.png)

* 判断间断点类型

  ![2023-02-15 20-29-23屏幕截图](https://s2.loli.net/2023/02/15/dshlbNM8wpEHVSu.png)

### 三. 连续函数的运算

### 四. 习题

例题1. 函数 $f(x) = \begin{cases} {{\sin 2x \over x},  x < 0 } \\ {x + 2}, x > 0 \end{cases}$ 在分段点 $0$ 处 ？         [例题1答案](#1.6_problem1)

## 2.1 导数的概念

### 一.导数定义

#### 导数定义式：

$$
f'(x) 
=
\lim\limits_{\Delta x \to 0}{{\Delta y} \over {\Delta x}}
= \lim\limits_{\Delta x \to 0}{{f(x+\Delta x) - f(x)} \over \Delta x}
$$

#### 函数在一点处的导数：

设自变量 $x$ 在 $x_0$ 处取得增量 $\Delta x$ ，有：
$$
f'(x_0) = \lim\limits_{\Delta x \to 0}{\Delta y \over \Delta x} = \lim\limits_{\Delta x \to 0}{{f(x_0 + \Delta x) - f(x_0) \over \Delta x}}
$$

#### 单侧导数：

分别为左，右导数，记为 $f'_{-}(x_0)$ 和 $f'_{+}(x_0)$
$$
f'_{-}(x_0) = \lim\limits_{\Delta x \to 0^-}{{f(x_0 + \Delta x) - f(x_0)} \over \Delta x} \\
f'_{+}(x_0) = \lim\limits_{\Delta x \to 0^+}{{f(x_0 + \Delta x) - f(x_0)} \over \Delta x}
$$

#### 导数不存在条件：

* 函数在该点不连续，且该点是函数的第二类间断点
* 函数在该点连续，但是该点的左右导数不相等

### 二.导数以及常见函数的求导


#### 常见函数导数：

![v2-4edc63dfc3551011cfaef8970ce95ae5_r](https://s2.loli.net/2023/02/13/nHpEgAywIB547eQ.jpg)

### 三.导数的几何意义

### 四.函数可导性和连续性

函数 $y = f(x)$ 在点 $x$ 处可导，即
$$
\lim\limits_{\Delta x \to 0}{\Delta y \over \Delta x} = f'(x)
$$

* 若 $y = f(x)$ 在点 $x$ 处可导，则函数在该点一定连续
* 若函数 $f(x)$ 在点 $x$ 处连续，但未必可导



## 2.2 求导法则

## 2.3 高阶导数

## 2.4 函数的微分

### 一.微分的定义:

设函数 $f(x)$ 在 $x_0$ 的某一个领域内有定义，当自变量 $x$ 取得增量 $\Delta x$ 时，相应的函数增量 $\Delta y = f(x_0 + \Delta x) - f(x_0)$ 可以表示为
$$
\Delta y = A\Delta x + o(\Delta x)
$$
称函数 $f(x)$ 在 $x_0$ 处`可微`. $A\Delta x$ 称为 $y = f(x)$ 在点 $x_0$ 相应于自变量增量 $\Delta x$ 的`微分`，记为 $dy$, 即：
$$
dy = A\Delta x
$$
也可以记为：
$$
df(x){\bigg|}_{x = x_0}
$$
由定义可知，函数微分 $dy$ 与增量 $\Delta y$ 仅相差了一个比 $\Delta x$ 高阶的无穷小, 可得：
$$
{\Delta y \over \Delta x} = A + {o(\Delta x) \over \Delta x} \\
\\
\lim\limits_{\Delta x \to 0} {\Delta y \over \Delta x} = \lim\limits_{\Delta x \to 0}(A + {o(\Delta x ) \over \Delta x}) = A \\
\\
f'(x) = A
\\
$$


即得：
$$
\lim\limits_{\Delta x \to 0}{\Delta y \over \Delta x} = f'(x) \\
\\
dy = f'(x)\Delta x
$$
通常把 $x$ 增量称为 `自变量的微分` 记为 $dx$, 即 $dx = \Delta x$， 有:
$$
{dy \over dx} = f'(x)
$$


### 二.基本初等函数微分运算和微分运算法则：

* 初等函数基本公式

  ![v2-4edc63dfc3551011cfaef8970ce95ae5_r1](https://s2.loli.net/2023/02/13/nHpEgAywIB547eQ.jpg)

* 函数四则运算的微分法则

  ![v2-b36b68abf0ca4769ae2cc84de45ef049_720w](https://s2.loli.net/2023/02/15/jOHSuMUbmsoRNnX.jpg)


* 复合函数的微分法则

$$
{dy \over dx} = f'[\varphi(x)] \cdot \varphi '(x)
$$



## 2.5 隐函数的导数和由参数方程所确定的函数的导数

### 一.计算隐函数的导数

![2023-02-15 22-12-23屏幕截图](https://s2.loli.net/2023/02/15/aGDSF1NtCoU2ieI.png)

### 二.计算参数方程的导数

我们假设参数方程:
$$
\begin{cases}
x = \alpha(x), \\
y = \beta(x)
\end{cases}
$$
假设 $x = \alpha(x)$ 在定义域上单调，可导且 $\alpha'(x) \neq 0$ ，则 $x = \alpha(x)$， 在该区间上的反函数 $\alpha^{-1}(x)$ 存在且
$$
{dt \over dx} = {1 \over \alpha'(x)}
$$
对于 $y = \beta(x)$ 同理，有：
$$
{dy \over dx} = {dy \over dt} \cdot {dt \over dx} = {\beta'(x) \over \alpha'(x)}
$$

### 三. 习题

例题1. 求方程 $y^7 + y - 2x^2 + 5 = 0$ 所确定的隐函数导数 $dy \over dx$                    [例题1答案](#2.5_problem1)

例题2. 求由方程 $xe^y - 2y + 6 = 0$ 所确定的隐函数 $y = y(x)$ 在 $x=0$ 处的微分   [例题2答案](#2.5_problem2)

例题3. 求双曲线 ${x^2 \over 4} - y^2 = 1$ 在点 $(8, \sqrt{15})$ 处的切线方程                       [例题3答案](#2.5_problem3)

例题4. 求 $y = {\sqrt{x + 1}(x + 3)^2 \over \sqrt[3]{x + 2}(x + 4)^3}$                                                  [例题4答案](#2.5_problem4)

例题5. 已知椭圆的参数方程 $\begin{cases} x = a \cos t \\ y = b \sin t \end{cases}$, 求椭圆在 $t = {\pi \over 4}$ 处的切线方程            [例题5答案](#2.5_problem5)



## 2.6 微分中值定理

### 一. 罗尔中值定理：

如果函数 $f(x)$ 在闭区间 $[a, b]$ 上连续，在开区间 $(a, b)$ 内可导，并且 $f(a) = f(b)$ 那么至少存在一点 $\varepsilon \in (a, b)$ 使得 $f'(\varepsilon) = 0$

![2023-02-19 16-37-04屏幕截图](https://s2.loli.net/2023/02/19/TGgeSRsh1OUY5dp.png)

### 二. 拉格朗日中值定理：

设函数 $f(x)$ 在闭区间 $[a, b]$ 上连续，在开区间 $(a, b)$ 内可导，那么至少存在一点 $\varepsilon \in (a, b)$ 使得：
$$
f(b) - f(a) = f'(\varepsilon)(b - a)
$$
使用条件：

* $(a, b)$ 上 $f(x)$ 可导
* 至少存在一点 $\varepsilon \in (a, b)$ 使得 $f'(x) = {f(b) - f(a) \over b - a}$

### 三. 柯西中值定理：

### 四. 小知识点：

* 通常称函数导数等于 $0$ 的点为函数的 `驻点`

## 2.7 泰勒公式

## 2.8 洛比达法则

## 3.1 不定积分的概念和基本性质

### 一. 原函数和不定积分的概念：

#### 不定积分定义：

函数 $f(x)$ 在区间 $I$ 内带有任意常数项的原函数称为 $f(x)$ 在区间 $I$ 内的不定积分，记为：
$$
\int f(x)dx
$$
等价于：
$$
F(x) + C
$$

* $f(x)$ 被称为 `被积函数`
* $f(x)dx$ 被称为 `被积表达式`
* $x$ 被称为 `被积变量`

#### 基本积分表

![v2-0855b8f2b620f94422d4e0c419cb0e58_720w](https://s2.loli.net/2023/02/19/x3oMhv9mrSE6GIl.webp)

#### 不定积分的基本性质

性质1.

* 若函数的不定积分存在，则
  $$
  {d \over dx}\bigg[\int f(x)dx\bigg] = f(x), (\forall x \in I)
  $$

* 若函数可导，则
  $$
  \int f'(x)dx = f(x) + C
  $$

* 不定积分提取常
  $$
  \int k \cdot f(x) dx = k \cdot \int f(x) dx
  $$
  

性质2.

* 若函数 $u(x)$ 和 $v(x)$ 的不定积分存在，则：
  $$
  \int \bigg[ \alpha u(x) + \beta v(x) \bigg]dx = \alpha \int u(x)dx + \beta \int v(x)dx
  $$

* 对上式结果求导可得：
  $$
  \bigg[ \alpha \int u(x) dx + \beta \int v(x) dx \bigg]' = \alpha \bigg[ \int u(x)dx \bigg]' + \beta \bigg[ \int v(x) dx \bigg]' = \alpha u(x) + \beta v(x)
  $$
  

### 三. 习题

例题1. 求 $\int {{x^2 - 2x + 3} \over \sqrt{x}}dx$                                      [例题1答案](#3.1_problem1)

例题2. 求 $\int {{2^{x+1} + 5^{x-1}} \over {10^x}}dx$                                     [例题2答案](#3.1_problem2)



## 3.2 不定积分的换元积分法

### 一. 不定积分第一类换元法（凑微分）：

设函数 $f(x)$ 在区间 $I$ 上连续，$u = \varphi(x)$ 具有连续的导数且 $\varphi(x)$ 的值域包含在 $I$ 中，则
$$
令u = \varphi(x)
\\
\int f[\varphi(x)]\varphi'(x)dx = \bigg[ \int f(u)du \bigg]
$$


### 二. 不定积分第二类换元法（变量代换）：

当式子中出现根号，平方等可通过第二类换元法得出答案



----



## 例题答案

### 1.1 函数

### 1.2 极限定义

### 1.3 极限的性质与运算法则

<span id='1.3_problem1'></span>

例题1.答案
$$
f(x) = \lim\limits_{n \to \infty} {{x ^ {2 n}} - 1 \over {x ^ {2 n}} + 1} = \lim\limits_{n \to \infty} ({1 - {2 \over x ^ {2 n} + 1}}) \\
\\
f(x) = \begin{cases}
 |x| > 1, & 1 \\
 |x| < 1, & -1 \\
 |x| = 1, & 0
\end{cases} \\
\\
在 |x| = 1 处,f(x)存在间隔点\\
\\
\lim\limits_{x \to 1^+}f(x) = 1 ,  \lim\limits_{x \to 1^-}f(x) = -1 \\
\lim\limits_{x \to -1^+}f(x) = -1, \lim\limits_{x \to -1^-}f(x) = 1 \\
\\
得出结论，f(x)的间断是1和-1, 且均为跳跃断点
$$
<span id='1.3_problem2'></span>

例题2.

![2023-02-09 22-10-37屏幕截图](https://s2.loli.net/2023/02/09/uIkhvP4gi8zsfBe.png)


$$
\lim\limits_{x \to 0^+}\arctan{1 \over x} = {\pi \over 2}\\
\lim\limits_{x \to 0^-}\arctan{1 \over x} = -{\pi \over 2}
$$

<span id='1.3_problem3'></span>

例题3.
$$
令 t = 3^n \\
\lim\limits_{n \to \infty}{3^n \sin{x \over 3^n}} = \lim\limits_{t \to \infty}{t \sin{x \over t}} = \lim\limits_{t \to \infty}{ \sin{x \over t} \over {1 \over t} } \\
由无穷小等价替换公式知， 结果为 {{x \over t} \over {1 \over t}} = x
$$


<span id='1.3_problem4'></span>

例题4.
$$
\lim\limits_{n \to \infty}{\sqrt{n}(\sqrt{n+1}-\sqrt{n})} 
= 
\lim\limits_{n \to \infty}{\sqrt{n}(\sqrt{n + 1} - \sqrt{n})(\sqrt{n+1} + \sqrt{n}) \over (\sqrt{n+1}+\sqrt{n})} 
= \\ 
\lim\limits_{n \to \infty}{\sqrt{n} \over \sqrt{n+1} + \sqrt{n}}
=
\lim\limits_{n \to \infty}{1 \over \sqrt{1 + {1 \over n}} + 1} = {1 \over 2}
$$
<span id='1.3_problem5'></span>

例题5.
$$
\lim\limits_{x \to \infty}({{x+a} \over {x-a}})^x
=
\lim\limits_{x \to \infty}(1 + {2a \over x - a})^x
=
e^{2ax \over x-a}
=
e^{2a \over {1-{a \over x}}}
=
e^{2a} 
= 
9 \\
({e^a})^2 = 9 \\
a = \ln3
$$

<span id='1.3_problem6'></span>

例题6.
$$
\lim\limits_{x \to 0}{({5x-\sin^2{x}-2x^3})' \over ({\tan x+4x^2})'}
=
\lim\limits_{x \to 0}{{5-2\sin x \cdot \cos x-6x^2} \over {{1 \over \cos^2 {x}} + 8x} }
=
{{5 - 0} \over 1}
=
5
$$


### 1.6 函数的连续性和连续函数的运算

<span id='1.6_problem1'></span>

例题1.
$$
\lim\limits_{x \to 0^+}{\sin 2x \over x} =  {2x \over x} = 2 \\
\lim\limits_{x \to 0^-}({x + 2}) = 2 \\
\\
左极限 = 右极限， 所以函数极限存在 \\
由原式知 \\
f(x) = \begin{cases}
		{\sin 2x \over x}, & x < 0 \\
		{x + 2}, & x > 0 \\
		\end{cases} 
\\
f(x) 没有在 x = 0 处有定义，所以函数不连续
$$

### 2.5 隐函数的导数和由参数方程所确定的函数的导数

<span id='2.5_problem1'></span>

例题1.
$$
(y^7 + y + 5)' = (2x^2)' 
\\
(y^7)' + y' = 4x
\\
{dy^7 \over dx} + {dy \over dx} = 4x = 7y^6{dy \over dx} + {dy \over dx}
\\
y' = {dy \over dx} = {4x \over 7y^6 + 1}
$$


<span id='2.5_problem2'></span>

例题2.
$$
(xe^y)' = (2y - 6)'
\\
e^y + xe^y \cdot y' = 2y'
\\
y' = {e^y \over 2 - xe^y}
\\
x = 0 \to y = 3
\\
y' = {e^3 \over 2}
\\
dy = {e^3 \over 2}dx
$$
<span id='2.5_problem3'></span>

例题3.
$$
({x^2 \over 4} - 1)' = (y^2)'
\\
{x \over 2} = 2y{dy \over dx}
\\
{dy \over dx} = {x \over 4y}
\\
x = 8, y = \sqrt{15}
\\
{dy \over dx} = k = {2\sqrt{15} \over 15}
\\
切线方程：y - \sqrt{15} = {2\sqrt{15} \over 15}(x - 8)
$$
<span id='2.5_problem4'></span>

例题4.
$$
利用对数求导法 
\\
\ln{y} = ln({\sqrt{x+1}(x+3)^2}) - \ln({\sqrt[3]{x+2}(x+4)^3})
\\
两边求导
\\
({1 \over y})y' = {(\sqrt{x + 1}(x+3)^2)' \over \sqrt{x + 1}(x+3)^2} - {(\sqrt[3]{x+2}(x+4)^3)' \over \sqrt[3]{x+2}(x+4)^3}
\\
y' = y[{1 \over 2(x+1)} + {2 \over (x+3)} - {1 \over 3(x+2)} - {3 \over (x+4)}]
\\
\\
y' = {\sqrt{x + 1}(x + 3)^2 \over \sqrt[3]{x + 2}(x + 4)^3}[{1 \over 2(x+1)} + {2 \over (x+3)} - {1 \over 3(x+2)} - {3 \over (x+4)}]
$$

<span id='2.5_problem5'></span>

例题5.
$$
设 M_0(x_0, y_0) 是 t = {\pi \over 4} 对应点的坐标\\
\begin{cases}
x_0 = a \cos{\pi \over 4} = {\sqrt{2} \over 2}a, \\ 
y_0 = b \sin{\pi \over 4} = {\sqrt{2} \over 2}b
\end{cases}
\\

{dy \over dx}{\bigg|}_{t = {\pi \over 4}} = {(b\sin t)' \over (a\cos t)'}{\bigg|}_{t = {\pi \over 4}} = {{b\cos t} \over {-a\sin t}}{\bigg|}_{t = {\pi \over 4}} = -{b \over a}
\\
切线方程：y - {\sqrt{2} \over 2}b = -{b \over a}(x - {\sqrt{2} \over 2}a)
$$



### 3.1 不定积分的概念和基本性质

<span id='3.1_problem1'></span>

例题1.
$$
\int {{x^2 - 2x + 3} \over \sqrt{x}}dx = \int ({x^{3 \over 2} - 2x^{1 \over 2} + 3x^{-{1 \over 2}}})dx
\\
= \int x^{3 \over 2}dx - 2\int x^{1 \over 2}dx + 3\int x^{-{1 \over 2}}dx
\\
= {2 \over 5}x^{5 \over 2} - {4 \over 3}x^{3 \over 2} + 6x^{1 \over 2} + C
$$
<span id='3.1_problem2'></span>

例题2.
$$
2\int {2^x \over 10^x}dx + {1 \over 5}\int {5^x \over 10^x}dx = 2\int ({1 \over 5})^xdx + {1 \over 5}\int ({1 \over 2})^xdx 
\\
= -{2 \over \ln5 \cdot 5^x} - {1 \over 5\ln2 \cdot 2^x} + C
$$


## 附  录

### 集合符号

符号小技巧：* 代表非0，即不含0， + 代表大于等于0， - 代表小于等于0

| 集合符号     | 符号意义                                             |
| ------------ | ---------------------------------------------------- |
| $N$          | 非负整数的集合或者自然数集合{0,1,2,3,4,5 ...}        |
| $N^*$或$N^+$ | 正整数集合{1,2,3,4,5 ...}                            |
| $Z$          | 整数集合{..., -1,0,1, ...}                           |
| $Q$          | 有理数集合                                           |
| $Q^+$        | 正有理数集合                                         |
| $Q^-$        | 负有理数集合                                         |
| $R$          | 实数集合（包括有理数和无理数）{1,2,0.333333..., ...} |
| $R^+$        | 正实数集合{0,1,2.3, ...}                             |
| $R^-$        | 负实数集合{0,-1,-2.3, ...}                           |
| $C$          | 复数集合{1 + i, 2 - 6i, ...}                         |
| $I$          | 虚数集合{$i^2$ = -1, $\sqrt{-9}$ = 3i, ...}          |
| $\oslash$    | 空集（不含有任何元素的集合）                         |

集合的关系图：

![2023-01-14 16-32-08屏幕截图](https://s2.loli.net/2023/01/14/GzJSV6CuZOXWArL.png)



### 对数运算

![img](https://s2.loli.net/2023/02/06/UmXcZbaEw4uLNAD.jpg)

![img](https://s2.loli.net/2023/02/06/NiG1dCyqDJxHFec.jpg)

![img](https://s2.loli.net/2023/02/06/Qo3vEMGb7NyZPJs.jpg)

![img](https://s2.loli.net/2023/02/06/aYbQrLVKgHUEZ8A.jpg)



<span id='jump3'></span>

### 初等函数图像集

* **幂函数**

  ![2023-01-24 15-15-49屏幕截图](https://s2.loli.net/2023/01/24/bUQugpFGVjkNCyl.png)

  交点坐标 $(1, 1)$ 和 $(-1,-1)$

  定义域：随 $\mu$, 但在 $(0, +\infty)$ 上总有定义

  值域：随 $\mu$

  主要性质：

  * 若 $\mu > 0$, $x^{\mu}$ 在 $[0, +\infty)$ 上单调增加
  * 若 $\mu < 0$, $x^{\mu}$ 在 $(0, +\infty)$ 上单调减少

  

* **指数函数**

  ![2023-01-24 15-35-22屏幕截图](https://s2.loli.net/2023/01/24/FyxIAUeszqTgbBE.png)

  交点坐标 $(0, 1)$

  定义域 $(-\infty, +\infty)$

  值域 $(0, +\infty)$

  主要性质 

  * $a^0 = 1$

  * 若 $a > 1$, $a^x$ 单调增加

  * 若 $0 < a < 1$, $a^x$ 单调减少

  * 直线 $y = 0 $ 为函数图形的水平渐近线

    

* **对数函数**

  ![2023-01-24 15-56-38屏幕截图](https://s2.loli.net/2023/01/24/wg5Y8qFBKrs9a2y.png)

  交点坐标 $(1, 0)$

  定义域 $(0, +\infty)$

  值域 $(-\infty,+\infty)$

  主要性质

  * $\log_{a}{1} = 0$

  * 若 $a > 1$， $\log_{a}{x}$ 单调增加

  * 若 $0 < a < 1$， $\log_{a}{x}$ 单调减少 

  * 直线 $x$ 是铅直渐近线

     

* 正弦函数（正/反）

  

* 余弦函数（正/反）

* 正切函数（正/反）

* 余切函数（正/反）

* 正割函数（正/反）

* 余割函数（正/反）

  



### 无穷小等价替换公式

使用条件： 

* 本质上是约分达到替换的效果，$\lim\limits_{x \to x_0}f(x) \cdot 1$（这个$1$是乘在整体上）, $1$ 可以被替换成两个等价的无穷小之比
* 只能用于乘除中，一般不能用在加减运算 

 ![dengjiatihuan](https://s2.loli.net/2023/02/06/UG9sKlLJjfapRPH.webp)

### 常见函数的导数和微分方程

![v2-4edc63dfc3551011cfaef8970ce95ae5_r](https://s2.loli.net/2023/02/13/W4pq7reV9viCJ82.jpg)



<span id='jump1'></span>

### 任何函数是奇偶函数和证明

设任意函数 $f(x)$:
$$
f(x) = {f(x)-f(-x) \over 2} + {f(x) + f(-x) \over 2}
$$
令 $g(x)$, $h(x)$:
$$
g(x) = {f(x) - f(-x) \over 2}, h(x) = {f(x) + f(-x) \over 2}
$$
有
$$
g(x) = -g(-x) = {f(x) - f(-x) \over 2} \\
h(x) = h(-x) = {f(x) + f(-x) \over 2}
$$
得 $g(x)$ 为奇函数，$h(x)$ 为偶函数，得证 $f(x)$ 是一个奇函数和一个偶函数的和



<span id='jump2'></span>

### 狄利克雷函数图像

函数原型：
$$
D(x) = \begin{cases} 
		1, x \in Q, \\
		0, x \in Q^c
	   \end{cases}
$$
函数图像(大概非真实图像)：

![pc3ba4sb](https://s2.loli.net/2023/01/14/pMButz85TOkvJi3.gif)

无理数的数量比有理数多，但有理数分布相对稠密，所以函数图像视觉上看上去像是 $y = 1$ 和 $y = 0$ 函数的合体，但是狄利克雷函数有理数点不连续，无理数点连续
