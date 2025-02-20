# ReXNet 系列
---
## 目录

* [1. 概述](#1)
* [2. 精度、FLOPS 和参数量](#2)

<a name='1'></a>

## 1. 概述

ReXNet 是 NAVER 集团 ClovaAI 研发中心基于一种网络架构设计新范式而构建的网络。针对现有网络中存在的 `Representational Bottleneck` 问题，作者提出了一组新的设计原则。作者认为传统的网络架构设计范式会产生表达瓶颈，进而影响模型的性能。为研究此问题，作者研究了上万个随机网络生成特征的 `matric rank`，同时进一步研究了网络层中通道配置方案。基于此，作者提出了一组简单而有效的设计原则，以消除表达瓶颈问题。[论文地址](https://arxiv.org/pdf/2007.00992.pdf)

<a name='2'></a>


## 2. 精度、FLOPS 和参数量

| Models | Top1 | Top5 | Reference<br>top1| FLOPS<br/>(G) | Params<br/>(M) |
|:--:|:--:|:--:|:--:|:--:|----|
| ReXNet_1_0 | 77.46 | 93.70 |       77.9        | 0.415 | 4.838 |
| ReXNet_1_3 | 79.13 | 94.64 |       79.5        | 0.683 | 7.611 |
| ReXNet_1_5 | 80.06 | 95.12 |       80.3        | 0.900 | 9.791 |
| ReXNet_2_0 | 81.22 | 95.36 |       81.6        | 1.561 | 16.449 |
| ReXNet_3_0 | 82.09 | 96.12 |       82.8        | 3.445 | 34.833 |

关于 Inference speed 等信息，敬请期待。
