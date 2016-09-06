# 线性回归 总结

# 1. 定义 Definition

在统计学中，线性回归是利用称为线性回归方程的最小二乘函数对一个或多个自变量和因变量之间关系进行建模的一种回归分析。

这种函数是一个或多个称为回归系数的模型参数的线性组合。

只有一个自变量的情况称为简单回归。

大于一个自变量的情况叫做多元回归。

# 2. 代价函数 Cost Function

假设函数 $$h_\theta(x)=\theta_0+\theta_1x$$

目标是选择出可以使得建模误差的平方和能够最小的模型参数。即使得代价函数

$$J ( \theta_0, \theta_1)=\frac{1}{2m}\sum_{i=1}^m\left( h_\theta(x^{(i)})-y^{(i)}\right)^2$$

最小。

# 3. 梯度下降 Gradient Descent

## 3.1 Batch Gradient Descent

$$repeat until convergence{

}$$

## 3.2 SGD

