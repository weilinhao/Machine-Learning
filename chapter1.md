# 线性回归 总结

# 1. 定义 Definition

在统计学中，线性回归是利用称为线性回归方程的最小二乘函数对一个或多个自变量和因变量之间关系进行建模的一种回归分析。

这种函数是一个或多个称为回归系数的模型参数的线性组合。

只有一个自变量的情况称为简单回归。

大于一个自变量的情况叫做多元回归。

# 2. 代价函数 Cost Function

假设函数 $$h_\theta(x)=\theta_0+\theta_1x$$

目标是选择出可以使得建模误差的平方和能够最小的模型参数。即使得**代价函数**

$$J ( \theta_0, \theta_1)=\frac{1}{2m}\sum_{i=1}^m\left( h_\theta(x^{(i)})-y^{(i)}\right)^2$$最小。

# 3. 梯度下降 Gradient Descent

## 3.1 Batch Gradient Descent

批量梯度下降算法公式为：

$$repeat \ until \ convergence \{ \\
 \theta_j := \theta_j -\alpha\frac{\partial}{\partial\theta_j}J(\theta_0,\theta_1) ~~ (for \ j=0 \ and \ j=1) \\

\}$$

其中$$\alpha$$是学习率（**learning rate**），它决定了我们沿着能让代价函数下降程度最大的方向向下迈出的步子有多大，在批量梯度下降中，我们每一次都同时让所有的参数减去学习速率乘以代价函数的导数。

需要注意的是，需要同时更新$$\theta_0$$和$$\theta_1$$。实现方法是：

应该计算公式右边的部分，通过那一部分计算出$$\theta
_0$$和$$\theta_1$$的值，然后同时更新$$\theta_0$$和$$\theta_1$$。

具体为：

$$

temp0:=\theta{\_0}

$$

## 3.2 SGD

