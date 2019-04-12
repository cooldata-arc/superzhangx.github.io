---
layout: post
date:   2019-04-09 16:15:00
title:  "Generalized Linear Models"
categories: machine learning
tags:  machine learning algorithm generalized linear models
mathjax: true
---

* content
{:toc}
广义线性模型 - Generalized Linear Models






---------

# 目录
- 1.监督学习
	- 1.1.广义线性模型
	- 1.2.线性和二次判别分析
	- 1.3.内核岭回归
	- 1.4.支持向量机
	- 1.5.随机梯度下降
	- 1.6.最近邻
	- 1.7.高斯过程
	- 1.8.交叉分解
	- 1.9.朴素贝叶斯
	- 1.9.决策树
	- 1.10.集成方法
	- 1.11.多类和多标签算法
	- 1.12.特征选择
	- 1.13.半监督学习
	- 1.14.等式回归
	- 1.15.概率校准
	- 1.16.神经网络模型(有监督)
- 2.无监督学习
	- 2.1.高斯混合模型
	- 2.2.流形学习
	- 2.3.聚类
	- 2.4.双聚类
	- 2.5.分解成分中的信号(矩阵分解问题)
	- 2.6.协方差估计
	- 2.7.经验协方差
	- 2.8.收敛协方差
	- 2.9.稀疏逆协方差
	- 2.10.Robust协方差估计
	- 2.11.新奇和异常值检测
	- 2.12.密度估计
	- 2.13.神经网络模型(无监督)
- 3.模型选择和评估
	- 3.1.交叉验证(评估估算器的表现)
	- 3.2.调整估计器的超参数
	- 3.3.模型评估(量化预测的质量)
	- 3.4.模型持久化
	- 3.5.验证曲线(绘制分数以评估模型)

---------

# 1.1.广义线性模型(Generalized Linear Models)
下面是一组用于回归的方法，其中目标值预期为输入变量的线性组合。在数学概念中，如果$\tilde{y}$是预测值，公式如下：<br>

$$\tilde{y} (w,x) = w_{0} + w_{1}x_{1} +...+w_{p}x_{p}$$

在整个模块中，我们指定向量$w=(w_{1},...,w_{p})$作为系数，$w_{0}$ 作为截距。

## 1.1.1. 普通最小二乘法

最小二乘法（又称最小平方法）是一种数学优化技术。它通过最小化误差的平方和寻找数据的最佳函数匹配。利用最小二乘法可以简便的求得未知的数据，并使这些求得的数据与实际数据之间误差的平方和最小。最小二乘法还可以用于曲线拟合。其他一些优化问题也可通过最小化能量或最大化熵用最小二乘法来表达。其矩阵表达形式为：

$$\min_{w}\parallel Xw-y\parallel_{2}^{2} \qquad w=(w_{1},...,w_{p})$$

### 1.1.1.1. 算法思想
\[
e ^ {i}
\]
### 1.1.1.2. 算法详解

### 1.1.1.3. 算法实现

### 1.1.1.4. sklearn中的应用