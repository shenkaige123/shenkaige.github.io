---
layout: post
title: 老马学机器学习-14-最大熵原理 principle of maximum entropy
date:  2018-11-14 08:38:35 +0800
categories: [ML]
tags: [ML, ai, math, sh]
published: true
---

# 最大熵原理

最大熵原理是一种选择随机变量统计特性最符合客观情况的准则，也称为最大信息原理。

随机量的概率分布是很难测定的，一般只能测得其各种均值（如数学期望、方差等）或已知某些限定条件下的值（如峰值、取值个数等），符合测得这些值的分布可有多种、以至无穷多种，通常，其中有一种分布的熵最大。

选用这种具有最大熵的分布作为该随机变量的分布，是一种有效的处理方法和准则。

这种方法虽有一定的主观性，但可以认为是最符合客观情况的一种选择。

在数学上，这个原理称为**最大熵原理**。


# 直观理解

在求解概率模型时，当没有任何约束条件则只需找到熵最大的模型，比如预测一个骰子的点数，每个面为 1/6。

当模型有一些约束条件之后，首先要满足这些约束条件， 然后在满足约束的集合中寻找熵最大的模型，该模型对未知的情况不做任何假设，未知情况的分布是最均匀的。

举例来说对于随机变量 X ，其可能的取值为 {A,B,C} ，没有任何约束的情况下下，各个值等概率得到的 MaxEnt 模型为：

P(A)=P(B)=P(C)=1/3

当给定一个约束 P(A)=1/2 , 满足该约束条件下的 MaxEnt 模型是：

P(A)=1/2

P(B)=P(C)=1/4

# TODO...

# 小结

希望本文对你有所帮助，如果喜欢，欢迎点赞收藏转发一波。

我是老马，期待与你的下次相遇。

# 参考资料

[最大熵原理](https://baike.baidu.com/item/%E6%9C%80%E5%A4%A7%E7%86%B5%E5%8E%9F%E7%90%86/9938383?fr=aladdin)

[深入机器学习系列21-最大熵模型](https://zhuanlan.zhihu.com/p/29978153)

[最大熵模型 Maximum Entropy Model](https://www.cnblogs.com/ooon/p/5677098.html)

https://blog.csdn.net/yangziluomu/article/details/81986271

https://blog.csdn.net/june_young_fan/article/details/88698301

https://www.cnblogs.com/wxquare/p/5858008.html

https://spaces.ac.cn/archives/3534

https://www.52nlp.cn/category/maximum-entropy-model

* any list
{:toc}