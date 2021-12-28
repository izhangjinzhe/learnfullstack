##### 特点

- 高性能，持久化
- key-value,支持多种数据类型
- 支持事务,原子性

##### 应用场景

- 缓存(读写性能优异)
- 计数&消息(高并发,阻塞队列)
- 分布式回话session&分布式锁(秒杀)

##### 使用

[http://doc.redisfans.com/](http://doc.redisfans.com/)

- `redis` 进入命令行
- `auth ![username] [password]` 登录
- `echo` 打印
- `ping` 心跳
- `quit` 退出
- `select [index]` 选择数据库
- `type [key]` 检查类型
- `move [key] [db]` 移动
- `ttl [key]` 生命周期(秒)
- `pttl [key]` 生命周期(毫秒)
- `expire [key] [time]` 设置生命周期(秒)
- `pexpire [key] [time]` 设置生命周期(毫秒)
- `persist [key]` 设置永不过期
- `rename [key] [newkey]` 更改键名

###### 字符串

- `set [key] [value]` 设置
- `get [key] [value]` 获取
- `mset ...[key] [value]` 批量添加
- `mget ...[key]` 批量获取
- `strlen [key]` 获取长度
- `append [key] [value]` 追加内容
- `getrange [key] [start] [end]` 获取内容
- `incr [key]` 自增
- `decr [key]` 自减
- `keys [pattern]` 过滤
- `exists ...keys` 判断是否存在
- `del ..keys` 删除

###### hash

- `hset [key] [field] [value]` 设置
- `hget [key] [field]` 获取
- `hgetall [key]` 获取全部
- `hmset [key] ...[field] [value]` 设置多个
- `hmget [key] ...[field]` 获取多个
- `hkeys [key]` 获取所有keys
- `hvals [key]` 获取所有value
- `hexists [key] [field]` 判断字段存在
- `hlen [key]` 获取字段数量
- `hincrby [key] [field] [number]` 字段的增\减
- `hdel [key] ...[field]` 删除字段

###### list

- `lpush [key] ...[value]` 左增
- `rpush [key] ...[value]` 右增
- `lrange [key] [start] [stop]` 获取
- `lpop [key] [count]` 左减
- `rpop [key] [count]` 右减

###### 发布/订阅

- `subscribe ...[channel]` 订阅
- `publish [channel] [message]` 发布

###### 删除

- `flushdb` 删除当前db
- `flushall` 删除全部db

###### 备份

- `save`
