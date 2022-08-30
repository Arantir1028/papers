# Title

Context-Aware_Deep_Model_Compression_for_Edge_Cloud_Computing

## Website
<!-- 网址，有DOI的建议用DOI地址-->

## Citing

<!-- 引用格式，建议使用latex格式-->

## Brief Introduction

<!-- 通过三五句话描述这篇文章，包括 1. 论文的应用场景；2. 论文克服已有方法的局限性；3. 论文主要的技术手段； 4. 论文的预期结果 -->

## Key Methodology
- 边端
    - MACC（multiply-accumulate operations），即点乘运算，是全连接层和卷积层的典型运算，是计算量的一种表示方法，大约是FLOPs的一半（因为包含一次加法和一次乘法）。
    - 对于卷积层，MACC表示为 卷积核面积 * 输出面积 * 输入通道数 * 输出通道数。
    - 对于全连接层，MACC表示为 输入通道数 * 输出通道数。
    - 时延和 MACC 呈线性关系，全连接层的系数在相同设备上固定，卷积层的系数和卷积核大小有关。
    - 这种线性关系在 CPU 上显著，在 GPU 上因为存在并行因此线性关系不显著。不精确，但是文章没详细讨论。
- 传输
    - 基于 pipeline 的文件传输协议，所以可以分成两阶段：第一个文件的传输时延（propagation delay）和后续文件的传输时延（transmission delay），如果第一个文件体积不那么大，总传输时延可以近似视为和文件大小呈线性关系。基于实验建立了线性模型。
- 云端
<!-- 分点写，论述论文中主要技术手段的实施过程 -->


## Data sets & Experimental Design

<!-- 撰写实验环境的设置，实验的对象，实验的比较方面，以及实验的结果（不要列举数据，要概括谈） -->


## Conclusion And Future Work

<!-- 作者或者阅读者对本文工作的总结，以及未来可能的改进方向 -->
