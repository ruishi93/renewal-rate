# renewal-rate

##### 1.FA & LR：基于sara抽取的指标做了因子分析&逻辑回归

[结果](./markdown/FA_LR.md)

**2.cart：用几个类别变量做了cart**（par_days, n_ex, level, visa_typ_cd）

**3.partFeatures & allFeatures：续费率与作业因素分析的阶段终版**

[结果](./markdown/final.md)

**4.tf_wide_contrib & tf_wide_core:** 探索使用wide&deep进行续费率的分析，预测的F1 score为0.937，相比LR预测准确率0.6639有很大提升，但是没有解释性，适用于单纯做预测。

**5.FM:** 探索FM(factorization machines)做续费率分析，FM中引入了交叉特征（二个特征相乘，“且”的关系），相比LR能够得到更丰富的解释性。例如，套餐为6个月且A套餐的学生，续费率更有可能续费；套餐为6个月且为湖州的学生，续费率不高。