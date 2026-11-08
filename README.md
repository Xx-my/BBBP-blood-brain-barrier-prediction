# BBBP 血脑屏障通透性预测

大二自学 AIDD 时做的第一个练习：预测一个分子能不能穿透血脑屏障（二分类任务）。

**做法**：Morgan 指纹 → scaffold split（按骨架分组切分，避免相似分子泄漏）→ 随机森林

**结果**：测试集 ROC-AUC 0.9189，准确率 0.8850

## 怎么跑

1. 安装依赖：`pip install pandas numpy rdkit scikit-learn`
2. 打开 `BBBP-血脑屏障预测.ipynb`，从头按顺序运行

## 数据

`BBBP.csv`，来自 MoleculeNet / BBBP 公开数据集（2,039 个化合物）。

参考：[yxl768/BBBP](https://github.com/yxl768/BBBP)
