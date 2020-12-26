API GateWay



#### API网关的核心特性

| **Features**         | key tech point | 对应的开源组件/库 |
| -------------------- | -------------- | ----------------- |
| **Dynamic upstream** | 动态的服务发现 | etcd              |
| **Dynamic router**   | ？？？         | ？？？            |
| **Health check**     |                |                   |
| **Dynamic SSL**      |                |                   |
| **L4 and L7 proxy**  |                |                   |
| **Opentracing**      |                |                   |
| **Custom plugin**    |                |                   |
| **REST API**         |                |                   |
| **CLI**              |                |                   |

本文记录的重点内容如何实现动态的路由：

1. 动态修改添加路由信息
2. 不同的url对应不同的处理模块
   1. test1 需要调用模块A、B、C
   2. test2 需要调用模块A、C、D
   3. 模块ABCD，如何管理？
   4. 功能调用的模块如何管理？