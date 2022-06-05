# Jittor 计图挑战赛热身赛

![主要结果](./result.png)

## 简介

本项目包含了第二届计图挑战赛计图 - 热身赛的代码实现。

## 安装 

#### 运行环境
- ubuntu 18.04 LTS
- python >= 3.7
- jittor >= 1.3.0

#### 安装依赖
执行以下命令安装 python 依赖
```
pip install -r requirements.txt
```

#### 预训练模型
预训练模型模型下载地址为https://pan.baidu.com/s/1HaU8PuPnxSmY_-1bjo_Spw?pwd=h7w9，提取码: h7w9，下载后放入目录 `<root>/` 下。

## 训练

将`discriminator_last.pkl`和`generator_last.pkl`移除出当前文件夹后，单卡训练可运行以下命令：
```
python CGAN.py
```

## 推理

生成测试集上的结果可以将`discriminator_last.pkl`和`generator_last.pkl`放在当前文件夹下运行以下命令：

```
python CGAN.py
```

## 致谢

此项目基于论文 *Conditional Generative Adversarial Nets* 实现，部分代码参考了 [jittor-gan](https://github.com/Jittor/gan-jittor)。
