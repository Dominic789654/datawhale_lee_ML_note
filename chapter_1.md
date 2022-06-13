# 第一章 机器学习介绍
## 过去 
**hand-crafted rules**  
基于规则判断的程序，使用成千上万的规则来模拟人的思维。  
可能会很有效，但注定永远无法超越创造者，并且成本非常高。
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h36ghz6lr9j20gb0e676h.jpg)
## 现在
**机器学习**  
使用一个内部包含大量函数(function)的模型(model)，在数据上进行学习，让模型自己去学到函数以及函数的参数，这就是机器学习。机器学习的范围非常广。  
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h36gtcsc8rj20i10agwfd.jpg)
其中使用模型在有标注的数据进行训练，称为监督学习(supervised learning).  
机器学习有举一反三的能力，这也是ML的重要问题，如何提高模型在没有见过的数据上的效果。  
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h36h4h0hjfj20mn0dgac6.jpg)
## 机器学习相关技术
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h36h6flug7j20lx0f0jt9.jpg)
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h36hty2iijj20me05mmyq.jpg)
### 监督学习(Supervised Learning)
主要分为回归问题(Regression)和分类问题(classification)。  
**回归问题**： 模型预测的结果是连续的，线性的。  
**分类问题**： 模型预测的结果是N分类中的一个，N选一。
监督学习需要大量的训练数据，并且在训练数据中还需要准确的标注出输入和输出之间的关系，需要人工为每个数据打上标签(label)。  
#### 结构化学习(Structured Learning)
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h36hok8luyj20ne0l078a.jpg)
### 半监督学习(Sem-supervised Learning)
半监督学习的方法可以减少人工标注label的数量。
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h36hfszq7lj20m10bxmyq.jpg)
### 迁移学习(Transfer Learning)
使用大量相同任务，但内容不相干的数据来帮助提高当前模型的效果的方法。  
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h36hih2v3bj20m90e5mzm.jpg)
### 无监督学习(Unsupervised Learning)
模型可以在没有标注的数据上达到无师自通，看模型在大量没有label的数据上可以学到什么。  
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h36hmro3bmj20mp0dzjts.jpg)
### 强化学习(Reinforcement Learning)
![](https://tva1.sinaimg.cn/large/e6c9d24ely1h36hrto5loj20mg05zdhk.jpg)
2022/06/13