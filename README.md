# STA326-project
## 岩石图像分类项目
本项目旨在基于深度学习方法实现岩石图像的多类别分类，使用了 **EfficientNet-B3** 模型并结合 **Mixup 数据增强** 和 **迁移学习策略**等方法，在实际应用中具有较强的鲁棒性和可扩展性。

## 项目结构

```
├── dataset/                  # 解压后的岩石图像数据集  
├── best_model.pth           # 训练得到的最佳模型权重文件  
├── dataset.zip              # 压缩格式的数据集  
├── dataset.py               # 数据集加载与预处理脚本  
├── train_best_model.ipynb   # 主训练脚本  
├── test_predictions.csv     # 模型在测试集上的预测结果  
├── project_introduction.pdf # 项目介绍文档  
├── requirements.txt         # 安装依赖  
```


## 运行步骤

1. **安装依赖**

建议使用 Python 3.8+ 和 pip 虚拟环境进行安装。
```bash
pip install -r requirements.txt
```
2. **解压数据集**

将 dataset.zip 解压至当前目录：
unzip dataset.zip

4. **运行训练代码**

打开并运行 train_best_model.ipynb 文件，即可开始训练与验证，测试集预测csv文件和最终模型均会保存在该目录下

## 实验结果

- 最佳验证集准确率：76.19%
- 最佳验证集 F1 分数：0.7628
- kaggle测试集准确率：75.90%

## 创新点与应用价值

- 本项目结合了迁移学习（EfficientNet-B3）与 mixup 数据增强，提升了模型的泛化能力
- 适用于岩石类型识别、地质勘探、矿产资源分析等领域，可为无人化地质巡检系统提供基础

## 作者

宋子墨，姜博宇（SUSTech 统计与数据科学系）  
邮箱：12212119@mail.sustech.edu.cn

