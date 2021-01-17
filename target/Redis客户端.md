# Redis客户端

​	Redis支持几十种编程语言的客户端操作，如 C、C++、C#、Java、Python、Go、Objective-C 等等；其中支持的Java语言客户端就有多种，下面三个是比较主流的客户端程序：

- Jedis
- Lettuce
- Redisson 



Jedis、Lettuce、Redisson 



## Jedis

一个比较轻巧的Redis Java客户端。



## Lettuce

​	高级Redis客户端，用于线程安全的同步，异步和反应式使用。 支持集群，前哨，流水线和编解码器。是SpringBoot 2.x 中默认使用的Redis Java客户端。



## Redisson 

用于构建分布式的Java客户端



项目地址：https://github.com/redisson/redisson 



## SpringBoot 中使用Redis



**RedisTemplate** 

Spring Data 项目提供了 RedisTemplate 模板，它封装了redis 连接池管理的逻辑。

SpringBoot 整合 Redis

 Redis





@Cacheable

@CachePut

@CacheEvict	根据条件对缓存清空



