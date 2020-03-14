# Metapath2vec
使用DGL实现metapath2vec
## 数据
数据使用的是JDATA竞赛的user-item数据
## 模型
使用DGL构造异构网络，然后对异构网络进行基于metapath的采样，得到若干个序列。
对这些序列采用基于负采样的skipgram，得到每个node的embedding
## 结果
对于这些user和item产生的embedding，因为是在同一个空间下，所以可以直接用户推荐。

# 后续
paper中几乎都是使用link prediction任务来判断embedding生成的好坏。
后续更新这种方法判断代码。
