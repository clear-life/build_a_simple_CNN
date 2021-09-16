# 从零搭建卷积神经网络

## 声明

项目代码参考该书

[深度学习入门 基于 python 的理论与实现](https://www.ituring.com.cn/book/1921)

该项目的目的是**用 numpy 实现一个简单卷积神经网络**

其他内容有**写注释和重构文件结构**(项目只有 17 个文件, 且在同一文件夹下)

## 总览

### 目标

**只用 `numpy` 库**搭建起一个简单的**卷积神经网络**,

并在 **MNIST 数据集**上进行训练

### 结果

在遍历 20 遍数据集后, 即 epochs 为 20 时,

训练出来的神经网络在测试数据集的**准确率达到 98.8 %** 左右

### 项目结构

只有一个文件夹, 该文件夹下只有 17 个文件

17 个文件分别是 10 个 .py 代码文件, 4 个 mnist 数据集文件, 2 个保存数据集和神经网络参数的 .pkl 文件, 1 个 readme 文件

* 中文命名的都是代码文件

| 文件名                      | 说明                                                         |
| --------------------------- | ------------------------------------------------------------ |
| 开始训练.py                 | 运行代码的 main 函数所在文件                                 |
| 训练器.py                   | 实现整个**训练过程的类**的文件                               |
| 神经网络.py                 | 实现**简单卷积神经网络类**的文件                             |
| 各层单独实现.py             | 每一层都是一个类, 实现**所有层的类**的文件                   |
| 优化器.py                   | 实现**优化方法的类**的文件                                   |
| 激活函数.py                 | 实现**激活函数**的文件                                       |
| 梯度计算.py                 | 实现**梯度计算函数**的文件                                   |
| 损失函数.py                 | 实现**损失函数**的文件                                       |
| 函数工具.py                 | 只有两个函数: im2col 和 col2im 函数<br />实现多维数据与二维数据的相互转换 |
| 加载数据集.py               | **加载 mnist 数据集相关函数**的文件                          |
| train-images-idx3-ubyte.gz  | mnist 训练集中的 输入数据(x_train) 文件                      |
| train-labels-idx1 -ubyte.gz | mnist 训练集中的 标签数据(t_train) 文件                      |
| t10k-images-idx3-ubyte.gz   | mnist 测试集中的 输入数据(x_train) 文件                      |
| t10k-labels-idx1-ubyte.gz   | mnist 测试集中的 标签数据(t_train) 文件                      |
| mnist.pkl                   | **保存 minst 数据集**的文件(np 数组格式)                     |
| params.pkl                  | **保存**训练好的**参数**的文件                               |
| readme.md                   | readme 文件                                                  |

