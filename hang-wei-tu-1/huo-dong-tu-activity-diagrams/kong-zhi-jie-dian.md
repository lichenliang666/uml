---
description: 下面的都是活动图中的使用的控制节点。
---

# 控制节点 Control Nodes

## 初始节点 Initial

这是个控制节点，活动将从这里开始。每个活动图中只能有一个初始。初始节点显示为**实心圆。**

![&#x6D3B;&#x52A8;&#x521D;&#x59CB;](../../.gitbook/assets/image%20%2822%29.png)

## 决策节点 Decision

决策节点接受一或两个输入，并从一或多个边到输出，

决策节点使活动图中的流程具有了条件的支持。

![&#x4E24;&#x4E2A;&#x6761;&#x4EF6;](../../.gitbook/assets/image%20%2827%29.png)

![&#x904D;&#x5386;&#x6761;&#x4EF6;&#x9884;&#x5B9A;&#x4E49;&#x4E2A;&#x5176;&#x4ED6;&#x6761;&#x4EF6;](../../.gitbook/assets/image%20%2826%29.png)

## 合并节点 Merge

合并节点是一个控制节点，它将传入的备用流汇集在一起已接受单个输出流。没有加入令牌。不应该使用合并节点来同步并发流。

例如，如果在fork之后使用决策节点，那么从决策节点出来的两个流程需要连接之前合并为一个；否则，连接将等待两个流，其中只有一个流将到达。

进出合并节点的所有边必须是**对象流**或是**控制流**。

合并节点的表示法是一个菱形符号，有两个或多个边进入它，一个活动边留下它。

![&#x5408;&#x5E76;&#x5177;&#x6709;&#x4E09;&#x4E2A;&#x4F20;&#x5165;&#x8FB9;&#x548C;&#x4E00;&#x4E2A;&#x4F20;&#x51FA;&#x8FB9;&#x7684; &#x8282;&#x70B9;](../../.gitbook/assets/image%20%2816%29.png)

可以通过使用相同的节点符号来组合合并节点和决策节点 的功能，如下所示。此案例映射到包含合并节点的模型，该合并节点包含图中显示的所有传入边，并且一个传出边指向具有图中所示的所有传出边的决策节点。

![&#x5408;&#x5E76;&#x8282;&#x70B9;&#x548C;&#x51B3;&#x7B56;&#x8282;&#x70B9;&#x4F7F;&#x7528;&#x76F8;&#x540C;&#x7684;&#x7B26;&#x53F7;&#x7EC4;&#x5408;](../../.gitbook/assets/image%20%2819%29.png)

## 同步节点 Synch

常用在状态机中，这里不进行太多结束，同步节点显示为圆圈中放个米字。

![&#x540C;&#x6B65;&#x8282;&#x70B9;](../../.gitbook/assets/image%20%2811%29.png)

## 分叉节点 Fork

同样是个控制节点，具有一个输入边界和多个输出边界，用于将传入的流分割为多个并发流。分叉节点支持并行的活动，与UML1.5相比，UML2.0活动图的分叉模型将不受并行性的限制。

![&#x4E00;&#x4E2A;&#x8F93;&#x5165;&#x662F;&#x4E09;&#x4E2A;&#x8F93;&#x51FA;](../../.gitbook/assets/image%20%283%29.png)

## 合并节点 Join

这也是一个控制节点，具有多个传入和一个传出，用于同步传入的并发流程。此节点用来支持活动图中的并行特性。它表示为一个线段，其中有几个活动输入，并且只有一个离开。

![&#x4E09;&#x4E2A;&#x6D3B;&#x52A8;&#x8F93;&#x5165;&#x4E00;&#x4E2A;&#x8F93;&#x51FA;](../../.gitbook/assets/image%20%2818%29.png)

![&#x7ED3;&#x5408;&#x5408;&#x5E76;&#x4E0E;&#x5206;&#x53C9;](../../.gitbook/assets/image%20%2824%29.png)

![&#x5408;&#x5E76;&#x89C4;&#x8303;&#x4F7F;&#x7528;&#x5927;&#x62EC;&#x53F7;&#x663E;&#x793A;](../../.gitbook/assets/image%20%2823%29.png)

## 流程结束 Flow Final

流程结束节点用来结束活动中的某个流程，但整个活动中的其他流程不受此控制。一个流程图中可以有多个流程结束节点。

![&#x6D41;&#x7A0B;&#x7ED3;&#x675F;&#x8282;&#x70B9;](../../.gitbook/assets/image%20%2817%29.png)

## 结束节点 Final

活动结束节点用于停止活动中的所有流程。一个活动中可以有多个结束节点。

![&#x6D3B;&#x52A8;&#x7ED3;&#x675F;&#x8282;&#x70B9;](../../.gitbook/assets/image%20%284%29.png)



