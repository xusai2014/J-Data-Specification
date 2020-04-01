# J-Data-Specification
💜Clietn-side 数据处理草案，缓存数据、持久化数据，前后端数据转化，封装统一的JS端数据增删改查。


## Client-side 数据痛点

客户端数据包括:
- 服务端提供数据(接口数据)
- 用户行为产生的状态数据（程序内存数据）
- 应用本身携带的基础数据。（本地持久化数据）

数据在时间和空间上的分布是无规则的，比如：
- 远程数据、本地数据、缓存数据、用户交互数据有异步和同步之分。
- 远程数据的更新、本地数据的更新需要同步保证一致。
- 多数据源数据增删改回滚

对客户端而言，数据又分为：
- 视图展示数据
- 业务逻辑数据

如果把数据看作资源，远程资源和本地资源两类又存在较大区别：
- 远程资源存在可用性问题，同时需要客户端提供身份凭证获取。
- 本地资源读取过程可靠性远高于远程资源，存在空间的限制。

**因此前端数据的结构化很重要，可以提高数据复用性、降低使用复杂性**


