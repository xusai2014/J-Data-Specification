# J-Data-Specification
💜Clietn-side 数据处理草案，缓存数据、持久化数据，前后端数据转化，封装统一的JS端数据增删改查。



## Client-side 数据痛点

1.数据结构
客户端数据包括，服务端提供数据、用户行为产生的状态数据、应用本身携带的基础数据。
数据在时间和空间上的无规则分布，比如远程数据、本地数据、缓存数据、用户交互数据有异步和同步之分。
又比如远程数据的更新、本地数据的更新需要同步保证一致。
