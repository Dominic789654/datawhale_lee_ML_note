[21版视频P5-9](https://www.bilibili.com/video/BV1JA411c7VT?p=5&vd_source=48793a38317f97a2e88a3bdf813932bf)
# 神经网络训练不起来怎么办
## 局部最小值(local minima)与鞍点(saddle point)
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h3bbt8fhc4j20zg0qkdjd.jpg)
梯度为0的点为critical point。
使用泰勒展开式可以判断当前critical point是local minima or saddle point.
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h3bc1rfo5gj20xb0mpwgq.jpg)
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h3bc2q85m6j20wc0hyadb.jpg)
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h3bc8l4fbyj20y70om774.jpg)
计算hessian matrix，可以判断critical point的情况。
## 批次(batch) 动量(momentum)
对每个batch求loss，1 epoch 计算所有batch。  
多batch可以有效避免梯度卡住和local minima的情况。  
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h3c8ud7z4tj20wy0lvtb9.jpg)
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h3c8vp5reoj20uc0fh0up.jpg)
## 自动调整学习率(learning rate)
**Root Mean Square** 
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h3cfsgtb6dj20xg0ndq51.jpg)
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h3cfswebvoj20v20kzwfx.jpg)
**RMSProp**
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h3cftwf099j20wf0mzwgf.jpg)
**Adam**
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h3cfvkriiij20wy0ni79p.jpg)
**Learning Rate Decay**
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h3cfz34wi8j20ww0bit9u.jpg)
**Warm up**
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h3cg2rdckvj20vc09kmxq.jpg)
在初始阶段，对error surface 有个探索。

![](https://tva1.sinaimg.cn/large/e6c9d24ely1h3cg4rdyycj20xk0nc0ul.jpg)
## 损失函数(loss function)
分类问题可以通过one-hot方法转换为矩阵。
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h3dmilptv5j20x10nh40h.jpg)
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h3dmjfyn7xj20x50mb765.jpg)
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h3dmmzb48aj20wf0mh40o.jpg)
PyTorch CE loss包含soft max  
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h3dxikea0nj20ye0lsgot.jpg)
MSE在较大loss的地方会卡住。  
Changing the loss function can change the difficulty of optimiztion.  
## batch normalization
把山铲平。
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h3ej1xmpf8j20yx0o5dj9.jpg)
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h3ej4aypcvj20xz0mu77g.jpg)
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h3ejjr5t41j20ys0ng41z.jpg)

## 总结
这几章主要讲了神经网络在训练中遇到的问题，以及对应的解决方法还有很多的优化方法。但是并没有太深刻理解，需要后面通过代码实践的方式来加深理解。