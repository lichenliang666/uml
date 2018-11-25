# 动作 action

为了与 activity（活动）进行区分，这里的 action 都称为“动作”。

## 变量动作 Variable Action

变量 action 包含变量的读取、写入、添加、移除、清理操作。

![&#x53D8;&#x91CF; action &#x6982;&#x8981;&#x56FE;](../../.gitbook/assets/image%20%282%29.png)

## 调用动作 Invocation Action

调用动作中有多种操作，包括信号发送、广播、发送对象。

![&#x8C03;&#x7528;&#x884C;&#x4E3A;&#x6982;&#x8981;&#x56FE;](../../.gitbook/assets/image%20%2825%29.png)

这个地方是粒度很小很具体的表示，先不介绍了，想了解的话点[这里](https://www.uml-diagrams.org/activity-diagrams-actions.html#invocation-action)。

## 时间事件动作 Accept time event action

如果某个行为**由时间来触发**，那么这个行为就是**时间事件行为。**有时也被非正式的称为“等待时间辛未”。用沙漏图形来表示⌛。

下图，每个小时执行一次。此时间事件操作没有传入边缘，因此只要启用 了包含活动或结构化节点，就会启用它。

![](../../.gitbook/assets/image%20%287%29.png)

