# Classification、Regression、Clustering 对比

| | Classification（分类） | Regression（回归） | Clustering（聚类） |
|---|---|---|---|
| 学习类型 | 监督学习 | 监督学习 | 无监督学习 |
| 训练数据 | 有标签 | 有标签 | 无标签 |
| 输出 | 离散类别 | 连续数值 | 算法发现的分组 |
| 目标 | 判断新样本属于哪一类 | 预测新样本的数值 | 发现数据的内在结构 |
| 例子 | 垃圾邮件识别 | 房价预测 | 用户分群 |
| 常见算法 | 逻辑回归、决策树、SVM | 线性回归、随机森林 | K-means、层次聚类、DBSCAN |
| 评估指标 | 准确率、F1 | MSE、MAE、R² | 轮廓系数 |

无监督学习的主要三大类：clustering，dimensionality reduction，generative models


# 无监督学习
├── 聚类（clustering）：找分组
│   ├── 基于中心：K-means
│   ├── 基于层次：层次聚类
│   ├── 基于密度：DBSCAN
│   └── 基于概率模型：高斯混合模型（GMM）
├── 降维（dimensionality reduction）：找主要变化方向
│   ├── 线性：PCA
│   └── 非线性：t-SNE、UMAP
├── 异常检测（anomaly detection）：找离群点
│   └── Isolation Forest、One-Class SVM
├── 关联规则挖掘（association rules）：找共现关系
│   └── Apriori、FP-Growth
└── 密度估计与生成模型：学习数据的分布
    ├── 密度估计：KDE、GMM
    └── 生成模型：自编码器、VAE、GAN