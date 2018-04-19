Mybatis缓存
=

缓存分类
-
+ 一级缓存(会话级别,SqlSession级别) 
+ 二级缓存(多个Session之间)



缓存流程
-

![一级缓存执行流程](https://github.com/tinyshuang/Note/blob/master/image/article/mybatis-1.jpg)
![一级缓存执行流程](https://pic3.zhimg.com/80/v2-65b50fa087add440f70e29ce85aa624b_hd.jpg)



注意事项
-
>一级缓存是session级别的,在多个session间或分布式环境容易出现脏数据,可设定缓存级别为Statement(默认为SESSION)

>二级缓存是跟namespace走的,多表关联时维护缓存比较麻烦,以及会造成效率比较低
 
 
总结
-
*生产环境不要用Mybatis缓存,直接使用redis等分布式缓存*

参考链接
https://zhuanlan.zhihu.com/p/33179093?utm_medium=social&utm_source=qq
