# Experiment 01 房价预测


# 实验目标：
验证线性回归模型是否能根据面积和卧室数预测房价
（模型是否收敛，lr效果

Features:Area、Bedroom

Label: Price (Price = w1​×Area + w2​×Bedroom + b)

Model: Linear Regression

Loss: MSE Loss

Optimizer: SGD

Evaluation: Training Loss、Prediction Result



# 实验数据
1. Exp001
lr = 0.000001
epoch 10000, loss 2930.382080
预测房价: 223.35757446289062
Conclusion: 训练失败，模型收敛有限

2. Exp002
lr = 0.0001
epoch 10000, loss 221.008347
预测房价: 261.1086730957031

3. Exp003
lr = 0.001
epoch 10000, loss 47.547890
预测房价: 272.535400390625

4. Exp004
lr = 0.01
epoch 10000, loss 12.363211
预测房价: 283.00872802734375

5. Exp005
lr = 0.05
epoch 10000, loss 138.827927
预测房价: 274.09814453125

6. Exp006
lr = 0.005
epoch 10000, loss 12.429413
预测房价: 282.7335205078125



# 结论：
1. 学习率过小收敛速度极慢。
2. 学习率过大会导致训练不稳定。
3. 在本实验中，0.01效果最佳。
4. 线性回归能够有效学习面积、卧室数与房价之间的线性关系。