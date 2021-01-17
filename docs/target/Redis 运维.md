# Redis 运维



```shell
# 注册服务 
redis-server.exe --service-install redis.windows.conf

# 删除服务 
redis-server --service-uninstall

# 开启服务 
redis-server --service-start

# 停止服务 
redis-server --service-stop
```



## 内部实现

Redis内部使用 redisObject 对象来表示所有的key 和 value。

type表示一个value对象是什么数据类型；

encoding表示对象在redis内部的存储方式；

<img src="..\md_resource\image-20200319085845183.png" alt="image-20200319085845183" style="zoom: 80%;" />



