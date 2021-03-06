
# 24. Advertising

## 24.1 Overview

#### Article

**计算广告CTR预估系列 1-9 from公众号：机器学习荐货情报局**:

- [计算广告CTR预估系列(一)--DeepFM理论](https://mp.weixin.qq.com/s?__biz=MzU0NDgwNzIwMQ==&mid=2247483673&idx=1&sn=256e57219c8d577c61f25221c346053c)

- [计算广告CTR预估系列(二)--DeepFM实践](https://mp.weixin.qq.com/s?__biz=MzU0NDgwNzIwMQ==&mid=2247483677&idx=1&sn=5bf0ac27124f57553cc8c17aa48664c7)

- [计算广告CTR预估系列(三)--FFM理论与实践](https://mp.weixin.qq.com/s?__biz=MzU0NDgwNzIwMQ==&mid=2247483685&idx=1&sn=36de5b8814c7a1ca5d5a19315b3f1ed1)

- [计算广告CTR预估系列(四)--Wide&Deep理论与实践](https://mp.weixin.qq.com/s?__biz=MzU0NDgwNzIwMQ==&mid=2247483689&idx=1&sn=c6e55677fe4ee1983e8f51fb61dffab5)

- [计算广告CTR预估系列(五)--阿里Deep Interest Network理论](https://mp.weixin.qq.com/s?__biz=MzU0NDgwNzIwMQ==&mid=2247483704&idx=1&sn=2b80e3def93056e4afb39cc1e744d18a)

- [计算广告CTR预估系列(六)--阿里Mixed Logistic Regression](https://mp.weixin.qq.com/s?__biz=MzU0NDgwNzIwMQ==&mid=2247483707&idx=1&sn=5810c525e2880edb795543d5b8bd4aa2)

- [计算广告CTR预估系列(七)--Facebook经典模型LR+GBDT理论与实践](https://mp.weixin.qq.com/s?__biz=MzU0NDgwNzIwMQ==&mid=2247483711&idx=1&sn=14e8d906d84de78b249510b33d423b89)

- [计算广告CTR预估系列(八)--PNN模型理论与实践](https://mp.weixin.qq.com/s?__biz=MzU0NDgwNzIwMQ==&mid=2247483719&idx=1&sn=ab9b912145c94ef299bc8484372794e9)

- [计算广告CTR预估系列(九)--NFM模型理论与实践](https://mp.weixin.qq.com/s?__biz=MzU0NDgwNzIwMQ==&mid=2247483738&idx=1&sn=61334a86c12f027cf6964196b62b3e7e)

#### Library

- <https://github.com/guoday/ctrNet-tool> (Tensorflow)

    This's the tool for CTR, including FM, FFM, NFFM and so on.

- <https://github.com/shenweichen/DeepCTR>

    Easy-to-use, Modular and Extendible package of deep-learning based CTR models. 包含很多主流的模型，如FM, PNN, Wide&Deep, DeepFM, xDeepFM, AFM, NFM, DIEN, NFFM, FGCNN, DSIN, FiBiNET

#### Competition

**2019腾讯广告算法大赛**

- <https://github.com/guoday/tencent2019_preliminary_rank1st>

    The code for 2019 Tencent College Algorithm Contest, and the online result ranks 1st in the preliminary.

    **Article**: 【Great】[2019腾讯广告算法大赛-冠军之路](https://zhuanlan.zhihu.com/p/72762888)

    **Article**: [一文梳理2019年腾讯广告算法大赛冠军方案](https://mp.weixin.qq.com/s?__biz=MzI3MTA0MTk1MA==&mid=2652054840&idx=4&sn=90bd20b8bf39d401be58ce72b44b0d8c)


**2018腾讯广告算法大赛**

- <https://github.com/wangle1218/Advertising-algorithm-competition>

    IJCAI 阿里妈妈搜索广告转化预测竞赛/讯飞广告营销算法/OGeek，模型有：LightGBM, LR, DeepFFM

- <https://github.com/DiligentPanda/Tencent_Ads_Algo_2018> (PyTorch)

    Tencent advertisement algorithm competition 2018. Rank 3 in the final round.

- <https://github.com/ColaDrill/tx_competition>

    Top3, Top12, Top15 总结分享

- <https://github.com/BladeCoda/Tencent2017_Final_Coda_Allegro>

    腾讯2017社交广告源码（决赛排名第23位），模型有：LightGBM, XGBoost


**阿里妈妈2018 IJCAI CTR预估**

- <https://github.com/plantsgo/ijcai-2018>

    Top1 Solution

- <https://github.com/YouChouNoBB/ijcai-18-top2-single-mole-solution>

    Top2 单模型方案，没有特征选择没有调参LGB单模型857个特征

- <https://github.com/luoda888/2018-IJCAI-top3>

    Top3 Code  3/5204， 模型有：LightGBM, XGBoost, CatBoost, GBDT+LR, DeepFFM, DeepFM, FNN


- <https://github.com/classtag/ijcai18-mama-ads-competition> 

    IJCAI-19 阿里妈妈搜索广告转化预测初赛方案，模型有：LightGBM, CatBoost

- <https://github.com/ShawnyXiao/2018-Kaggle-AdTrackingFraud>

    2018 - Kaggle - TalkingData AdTracking Fraud Detection Challenge: Silver medal (银牌), 模型是LightGBM


## 24.2 Classic

### 24.2.1 [Practical Lessons from Predicting Clicks on Ads at Facebook - Facebook2014](http://quinonero.net/Publications/predicting-clicks-facebook.pdf)

**Keywords**: LR + GBDT

**Key Points**: 利用树模型(GBDT)组合特征的能力自动做特征组合，作为新的特征叠加到LR模型里再训练一个LR模型。

#### Code

- <https://github.com/neal668/LightGBM-GBDT-LR>

#### Article

- [Practical Lessons from Predicting Clicks on Ads at Facebook](http://www.bubuko.com/infodetail-1902390.html)


### 24.2.2 Mixed LR - [Learning Piece-wise Linear Models from Large Scale Data for Ad Click Prediction - Ali2017](https://arxiv.org/abs/1704.05194)

**Keywords**: Mixed LR

**Key Points**: 基于Mixed LR的CTR模型，核心思想是聚类LR

#### Article

- [计算广告CTR预估系列(六)–阿里Mixed Logistic Regression](https://blog.csdn.net/u010352603/article/details/80681239)


### 24.2.3 FTRL - [Ad Click Prediction - A View From the Trenches - Google2013](http://static.googleusercontent.com/media/research.google.com/en/us/pubs/archive/41159.pdf)

**Keywords**: Online Advertising; Data Mining; Large-scale Learning

**Key Points**: FTRL，一种大规模在线学习算法

#### Article

- [各大公司广泛使用的在线学习算法FTRL详解](http://www.cnblogs.com/EE-NovRain/p/3810737.html)


## 24.3 Deep Learning

### 24.3.1 Overview


### 24.3.2 [Audience Expansion for Online Social Network Advertising - LinkedIn2016](https://www.kdd.org/kdd2016/papers/files/adf0483-liuA.pdf)

**Keywords**: Online Advertising; Audience Expansion; Lookalike Modeling

**Key Points**: 


### 24.3.3 DIN - [Deep Interest Network for Click-Through Rate Prediction - Ali2018](https://arxiv.org/abs/1706.06978)

**Keywords**: CTR Prediction; Display Advertising; E-commerce; DIN; Attention Mechanism

**Key Points**: 引入了Attention Mechanism

#### Article

- [推荐系统中的注意力机制——阿里深度兴趣网络(DIN)](https://zhuanlan.zhihu.com/p/51623339)

- [计算广告CTR预估系列(五)--阿里Deep Interest Network理论](https://blog.csdn.net/u010352603/article/details/80590152)

