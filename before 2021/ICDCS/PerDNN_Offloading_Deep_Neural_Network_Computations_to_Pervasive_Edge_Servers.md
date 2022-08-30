# Title

PerDNN_Offloading_Deep_Neural_Network_Computations_to_Pervasive_Edge_Servers

## Website
<!-- 网址，有DOI的建议用DOI地址-->

## Citing

<!-- 引用格式，建议使用latex格式-->

## Brief Introduction

<!-- 通过三五句话描述这篇文章，包括 1. 论文的应用场景；2. 论文克服已有方法的局限性；3. 论文主要的技术手段； 4. 论文的预期结果 -->

## Key Methodology
- 基于 GPU 的 DNN 时延预测（边服务器）
    - 考虑 GPU 挤占（congestion of GPU），即多个推理任务共享同一 GPU。这里基于 GPU 信息去估算资源争用时延。
        - 基于 GPU 统计和层超参数估算层执行时间。GPU 统计包括核/内存利用率、内存占用、温度等。
        - 具体的估计基于离线的黑盒训练，具体数据是在进行多客户端推理时的一个 DNN 层推理时间。
    - 基于图的分割方案
        - 数据流有端和边服务器两条路线，边服务器通过第一条进行估计，端执行时间使用 profile，传输时间通过将输入/输出数据量除以运行时网速得到。
<!-- 分点写，论述论文中主要技术手段的实施过程 -->


## Data sets & Experimental Design

<!-- 撰写实验环境的设置，实验的对象，实验的比较方面，以及实验的结果（不要列举数据，要概括谈） -->


## Conclusion And Future Work

<!-- 作者或者阅读者对本文工作的总结，以及未来可能的改进方向 -->
