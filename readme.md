# 工具箱的深度學習記事簿

## 这是什么

这个仓库包含了或即将包含深度学习相关基础知识和仅仅比基础高级一点的知识。每篇的内容将会包含：

- 这个知识有什么用
- 这个知识如何使用或如何实现

__在仓库中，会有一些基于框架的代码实现，大部分情况下会使用[tensorflow](https://www.tensorflow.org/)，或使用[MX-Net](http://mxnet.apache.org/)。__部分代码使用了其他框架会在代码上方注明。`实际上，使用何种框架与学习相关知识的关系没有想象中的那么大`。

__还有一件事，这个仓库的部分文稿包含了LaTex公式。__ 在网页上，这些公式可能不能被正确地显示出来。如果真的希望阅读本仓库，请将仓库克隆到本地。

---

## But why ?

> 理解机器学习和深度学习的最佳方法是学以致用。

众所周知，工具箱的深度学习基础是整个F4是稳稳垫底的水准。工具箱在补习基础知识的过程中，作为笔记形成了本仓库。这个仓库不一定有非常好的借鉴作用，但是工具箱尽量让它对自己很有用。

---

## 目录

目录的使用方法：**点击就可以跳转到相关页面**。其中前面打了对勾的是已经可供阅读的部分，未打勾的是还没有写或正在写的部分。本仓库在宣布`archive`之前会保持更新。

如果你在阅读的过程中遇到了不明白的名词，为了防止出现递归式学习，可以参照[附录-常见词汇](./appendix/similar-vocabularies.md)了解相关词汇的释义。

### 第零章：预备知识

- [x] [使用 conda 创建一个环境...?](./ch0/create-new-environment-using-conda.md)
- [x] [要配置GPU？](./ch0/configure-gpu.md)
- [x] [试着对数据进行操作](./ch0/operate-on-data.md)
- [x] [自动求梯度](./ch0/automatic-gradient.md)

### 第一章：深度學習基礎

- [x] [机器学习的HelloWorld：线性回归](./ch1/linear-regression.md) | [线性回归的代码实现](./ch1/linear-regression-code.md)
- [x] [softmax 回归](./ch1/softmax-regression.md) | [代码实现](./ch1/softmax-regression-code.md)
- [ ] [多层感知机]() | [代码实现]()
- [ ] [模型的选择，欠拟合和过拟合]()
- [ ] [权重衰减]()
- [ ] [丢...丢弃法?]()
- [ ] [正向传播和反向传播]()

### 第二章：深度學習計算

- [ ] [模型构造]()
- [ ] [模型哪来的参数？]()
- [ ] [模型参数的访问、初始化和共享]()
- [ ] [模型参数延后初始化]()
- [ ] [自定义网络层]()
- [ ] [储存和读取模型]()
- [ ] [使用GPU运算]()

### 第三章：卷积神经网络

- [ ] [二维卷积层]()
- [ ] [填充和步幅]()
- [ ] [多输入通道和多输出通道]()
- [ ] [池化层]()
- [ ] [使用框架实现卷积！实战cifar10！]()
- [ ] [卷积神经网络！(LeNet)]()
- [ ] [深度卷积的神经网络！(AlexNet)]()
- [ ] [使用重复元素(?)的网络(VGG)]()
- [ ] [套娃！网络中的网络。(NiN)]()
- [ ] [含有并行连接的网络]()
- [ ] [批量归一化]()
- [ ] [残差网络(ResNet)]()
- [ ] [稠密链接网络(DenseNet)]()

### 第四章：循环神经网络

- [ ] [呃，语言模型是啥]()
- [ ] [循环神经网络！]() | [代码实现]()
- [ ] [一个语言模型的数据集（歌词）]()
- [ ] [通过时间反向传播]()
- [ ] [门控制循环单元(GRU)]()
- [ ] [长短期记忆(LSTM)]()
- [ ] [深度循环神经网络]()
- [ ] [双向循环神经网络]()

### 第五章：计算机视觉

- [ ] [图像增广]()
- [ ] [微调]()
- [ ] [目标检测和边界框]()
- [ ] [锚框]()
- [ ] [多尺度目标检测]()
- [ ] [目标检测数据集（皮卡丘）]()
- [ ] [单发( 这是啥鬼翻译)多框检测(SSD)]()
- [ ] [区域卷积神经网络(R-CNN)系列]()
- [ ] [语义分割和数据集]()
- [ ] [全卷积网络(FCN)]()
- [ ] [样式迁移]()
- [ ] [实战 Sifar-10]() | [实战 ImageNet-Dogs]()

### 附录

- [x] [常见的词汇](./appendix/similar-vocabularies.md)
- [ ] 常见的包

