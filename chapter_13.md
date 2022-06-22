# 第十三章 深度学习的发展趋势
1. 神经网络
2. 模型评估
3. 选择最优函数

不论是做回归模型（linear model）还是逻辑回归（logistics regression）都是定义了一个函数集（function set）。我们可以给上面的结构的参数设置为不同的数，就是不同的函数（function）。这些可能的函数（function）结合起来就是一个函数集（function set）。这个时候你的函数集（function set）是比较大的，是以前的回归模型（linear model）等没有办法包含的函数（function），所以说深度学习（Deep Learning）能表达出以前所不能表达的情况。
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h3a4oqfsrqj20hw0igmyo.jpg)
## 思考
隐藏层越多越好？
一层多神经单元 or 深层神经网络？

## 总结
学习了深度学习与机器学习的不同点，对神经网络有了大概的了解。学习了隐藏层，激活函数在神经网络中的作用，知道了GPU对深度学习带来的帮助。深度学习的模型评估与梯度下降过程与机器学习相似，在参数量上有很大的不同。深度学习不会刻意的挑选function，让模型自己去学习function以及function的参数，这是和机器学习比较不同的一点。并且深度学习的神经网络结构之间也有很大的差异，不同的结构之间的效果也有很大的不同。