## EventBus

- [观察者模式 : 一支穿云箭，千军万马来相见](http://blog.csdn.net/u011240877/article/details/52683558)
 
   关键点：
   1. 一对多关系模式
   2. 一切始于被观察者（Observable）
   3. 被观察者（Observable）通过一个开关命令触发具体的动作，且会调用观察者（Observer）中的某个方法
   4. 观察者（Observer）内早就准备好了触发后方法的具体实现
   

- [EventBus 3.0 的特点与如何使用](http://blog.csdn.net/u011240877/article/details/73015939)
 
   关键点:
   1. 谁用谁注册和注销
   2. 注册和注销要成对出现
   3. 4种线程模式
   4. 只有在同一线程中的订阅者优先级才有作用
   5. 只有 ThreadMode 为 POSTING 的订阅方法可以拦截消息，这通过调用 cancelEventDelivery(event) 方法
   6. 通过 EventBus.builder()配置
   7. 异步线程池 AsyncExecutor


- [源码分析 EventBus 3.0 如何实现事件总线](http://blog.csdn.net/u011240877/article/details/73196808)
 
   关键点：
   1. 
   
   
- [从 EventBus 中学到的精华](http://blog.csdn.net/u011240877/article/details/74599216)
 
 
---
 
 **原作者：shixinzhang**

_原文链接_：

1. [http://blog.csdn.net/u011240877/article/details/52683558](http://blog.csdn.net/u011240877/article/details/52683558)
2. [http://blog.csdn.net/u011240877/article/details/73196808](http://blog.csdn.net/u011240877/article/details/73196808)
3. [http://blog.csdn.net/u011240877/article/details/73015939](http://blog.csdn.net/u011240877/article/details/73015939)
4. [http://blog.csdn.net/u011240877/article/details/74599216](http://blog.csdn.net/u011240877/article/details/74599216)