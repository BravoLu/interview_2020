# 贝叶斯估计

* reference:  [http://noahsnail.com/2018/05/17/2018-05-17-%E8%B4%9D%E5%8F%B6%E6%96%AF%E4%BC%B0%E8%AE%A1%E3%80%81%E6%9C%80%E5%A4%A7%E4%BC%BC%E7%84%B6%E4%BC%B0%E8%AE%A1%E3%80%81%E6%9C%80%E5%A4%A7%E5%90%8E%E9%AA%8C%E6%A6%82%E7%8E%87%E4%BC%B0%E8%AE%A1/](http://noahsnail.com/2018/05/17/2018-05-17-贝叶斯估计、最大似然估计、最大后验概率估计/) 

## 最大似然估计

$P(x|\theta) = \frac{P(\theta|x)P(x)}{P(\theta)}$

## 最大后验估计（MAP）

* 公式：$P(\theta|x)=\frac{P(x|\theta)P(\theta)}{P(x)} = P(x|\theta)P(\theta)$ ($P(x)$是常数) 

* 与最大似然估计的区别：最大似然估计认为使似然函数$P(X|\theta)$最大参数的$\theta$即为最好的$\theta$, 此时最大似然估计是将$\theta$看作固定的值，只是其值未知；最大后验概率分布认为$\theta$是一个随机变量，即$\theta$具有某种先验分布，求解时除了要考虑似然函数$P(X|\theta)$，还要考虑$P(\theta)$。最大后验概率估计可以看作是正则化的最大似然估计。在最大似然估计中，由于认为$\theta$是固定的，因此$P(\theta)=1$.
## 贝叶斯估计

* 贝叶斯估计是最大后验估计的进一步扩展，贝叶斯估计同样假定$\theta$是一个随机变量，但贝叶斯估计并不是直接估计出$\theta$的某个特定值，而是估计$\theta$的分布。