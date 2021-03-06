# 头文件

头文件的命名极其重要，因为它可以指出头文件包含的内容：

* 声明一个孤立的class或protocol

* * 将声明放入单独的文件
  * 使头文件名与声明的class/protocol相同
* ![1441510258390459](assets/1441510258390459.png)

* 声明关联的class或protocol

* * 将关联的声明（class/category/protocol）放入同一个头文件
  * 头文件名与主要的class/category/protocol相同
* ![1441510278719846](assets/1441510278719846.png)

* Framework头文件

* * 每个framework都应该有一个同名头文件
  * Include了框架内其他所有头文件
* ![1441510294801244](assets/1441510294801244.png)

* 添加API到另一个framework

* * 如果要在一个framework中为另一个framework的class catetgory添加方法，加上单词“Additions”

  * * 如Application Kit的NSBundleAdditions.h 文件
* 关联的函数、数据类型

* * 如果你有一组关联的函数、常量、结构体或其他数据类型，将它们放到一个名字合适的头文件中

  * * 如Application Kit的NSGraphics.h

{% include links.html %}
