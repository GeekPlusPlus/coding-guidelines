# 类与协议的命名

## 类

* class的名称应该包含一个名词，用以表明这个类是什么（或者做了什么），并拥有合适的前缀
* 如NSString、NSDate、NSScanner、UIApplication、UIButton

### 不关联class的protocol

* 大多数protocol聚集了一堆相关方法，并不关联class

* 这种protocol使用ing形式以和class区分开来

  ​

  ![1441510247983445](assets/1441510247983445.png)

### 关联class的protocol

* 一些protoco聚集了一堆无关方法，并试图与某个class关联在一起，由这个class来主导

* * 这种protocol与class同名

  * * 如NSObject protocol



{% include links.html %}
