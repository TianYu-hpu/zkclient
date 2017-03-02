#ZooKeeper 开源客户端实现 ZkClient

ZkClient是Github上一个开源的ZooKeeper客户端。ZkClient在ZooKeeper原生API接口之上进行了包装，是一个更加易用的ZooKeeper客户端。同时，ZkClient在内部实现了诸如Session超时重连、Watcher反复注册等功能。

在编写完成的时候测试了一下
SubScribeDataChange 和 SubscribeStateChange 无法显现出效果，我分别创建节点、修改节点，然后连接其他服务，并close掉，均没有打印日志。    
------待修复------
