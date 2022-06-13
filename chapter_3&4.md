# 第三章 回归
Regressio就是找到一个函数function， 通过输入特征x，输出一个数值Scalar。  
**模型步骤**  
- step1：模型假设，选择模型框架（线性模型）  
- step2：模型评估，如何判断众多模型的好坏（损失函数）  
- step3：模型优化，如何筛选最优的模型（梯度下降）  
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h36sbeql3jj20iq0d1dhh.jpg)
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h36scbscxej20m10h776e.jpg)

**步骤优化**
- step1: 模型融合；  
- step2: 模型拥有更多参数，数据包含更多特征；  
- step3: 加入正则化，防止过拟合。  
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h36sgrg16uj20l10ggaci.jpg)