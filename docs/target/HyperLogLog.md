# HyperLogLog

HyperLogLog，它是 LogLog 算法的升级版，作用是能够**在大数据中做高效率的基数统计**（去重计数）。

有如下特点：

- 能够使用极少的内存统计海量数据，在Redis中实现的 HyperLogLog ，只需要12K 内存就可以统计2^64个数据。
- 基数统计存在一定误差，标准误差率低于1%（0.81％）。
- 误差可以通过 辅助计算因子进行降低。



## LogLog 算法

​	基数估计算法（LogLogCounting）是基于概率论与数理统计所设计的概率统计算法，用于在大数据中进行不完全精确的基数统计。

​	为什么叫LogLog 算法呢？因为这种算法的**空间复杂度是O(log(log(Nmax)))**，可以通过KB级内存估计数亿级别的基数。



有一个网站，可以动态地让你观察到 HyperLogLog 的算法到底是怎么执行的：

http://content.research.neustar.biz/blog/hll.html

<img src="..\md_resource\image-20200315092007865.png" alt="image-20200315092007865" style="zoom:80%;" />







