### Java程序执行流程

![Java程序执行流程](/assets/WechatIMG297.jpeg)

1. 所有的程序都要求运行在JVM上，是因为考虑到了可移植性问题，可是如果要想真正的去执行程序，绝对不可能离开操作系统的支持
2. 在Java中可以使用native实现本地C函数的调用，但是这些都属于程序运行的辅助手段，而真正程序的运行都在运行时数据区中

### Java运行时数据区

![Java运行时数据区](/assets/2981516982268_.pic_hd.jpg)

3. 在整个的运行时数据区中分为如下几块内存空间：
 - 堆内存：保存所有引用数据类型的真实信息
 - 栈内存：基本类型、运算、指向堆内存的指针
 - 方法取：所有定义方法的信息都保存在方法区当中，此区属于共享区
 - 程序计数器： （有异常之后的代码定位行数）是一个非常小的内存空间，小到可以忽略
 - 本地方法栈： 每一次执行递归的方法处理的时候，都会将上一个方法入栈
 
### 本地方法栈
 
![本地方法栈](/assets/2991516983030_.pic_hd.jpg)

![栈帧](/assets/3001516983140_.pic_hd.jpg)