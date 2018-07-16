---
title: 一些面试记录
date: 2018-06-29 00:18:14
tags: Android面试
category: Android
toc: true
---

#### 1、魅族
毕业那时候面试的，忘记了。

#### 2、金山
1、问做过的Android项目，当时让我实现一个undo 和 redo 的功能，设计好数据结构和处理逻辑。
2、Retrofit2的实现方式。
3、HashMap的原理。
4、ArrayList原理
5、加载大图的处理方式，防止OOM，例如加载清明上河图。可以使用原生的BitmapRegionDecoder。
6、无限滑动的列表，怎么处理加载的数据？
7、线程和线程池，并发的安全性。
8、各种设计模式。
9、虚拟机GC过程和算法。
10、Android事件分发。
11、如何处理性能问题，具体例子。

#### 3、oppo

**电话面**
1、问项目

**现场面**
1、主要是项目上的东西，问得很仔细。

#### 4、百度
**电话面**
1、虚拟机GC过程和算法，GCRoot是哪些。
2、事件分发。
3、handler机制。
4、还接触了那些其他新技术。
5、性能优化，具体的优化过程。

#### 5、今日头条
1、进程间通讯。
2、性能优化。
3、ListView的CardView解耦方式。
4、SurfaceView和TextureView的区别
5、序列化的方式。
6、wait和sleep为什么要在同步块里。
7、onNewIntent什么时候执行，getIntent的数据。

#### 6、中软国际
其实是华为外包，第一面是中软国际的一个小哥，第二面去华为那边另一个小哥面。
1、项目上的一些东西。
2、对称加密和非对称加密，使用场景。
3、Handler机制。

华为那边：
1、介绍一下四大组件。
2、内存泄漏和OOM的情况和原因，怎么处理。
3、Activity的生命周期。
4、Handler机制。
5、自定 view，view的绘制流程。
6、性能优化，具体的优化过程。具体例子。

#### 7、BiGo
一面：
1、static代码块，什么时候初始化。类被载入的时候有且只有一次初始化。
2、JVM的内存模型。
3、多线程使用，4种线程池。等待多个线程完成后再处理的问题。Join（）。
4、各种锁，各种锁的效率。
5、HashMap里面的hashCode和数组index的转换。HashMap是不是保持顺序的。
6、LinkedHashMap结构和使用，和HashMap的差异。
7、一个数字char转化成int数字。减去char '0'，char占几个字节。
8、Activity启动流程，App启动流程，Zygote怎么知道要启动那个程序，AMS如何管理Activity的。
9、内存泄漏，OOM的处理。
10、OkHttp和EventBus。
11、做过哪些比较难的东西？
12、设置一个死锁的情况，平常有没有遇到死锁的问题。死锁导致ANR问题。
13、private 方法能否被调用，反射调用单例里面的private static 初始化类会不会创建多个对象。
14、long转int会越界／OOM吗？
15、ArrayList，HashMap扩容。

二面：
1、算法题，敲代码。链表反转，K个链表合并。
2、Retrofit2，OkHttp3 的设计模式。责任链模式和策略模式的区别。
3、框架MVP，MVVM，MVC的差异，还有没有其他框架，框架的目的和作用是什么？没答好。
4、动态代理的必要条件，interface，抽象类可以实现动态代理吗？代理的是什么？没答好。
5、android动画和OpenGL动画的差别，性能。GPU和CPU计算的差别。
6、app的启动流程，Activity的启动流程。
7、Fragment的实现原理。没答好。
8、个人职业规划什么的。
9、React native，weex，flutter等差异。
10、做的最有成就感的东西。
11、性能优化具体例子，怎么解决。
12、系统添加新的apk资源包，因为简历写了，所以问，具体修改了什么。aapt，mk，assetmanager，resourceTable，ResourceTpye等。
13、问了做过的东西的难点是什么。自定义View遇到的问题，SDK开发遇到的问题，原生控件添加功能遇到的问题。


#### 8、菜鸟网络
电话面：
1、简历上的项目。
2、插件化热修复。
3、虚拟机GC相关东西。
4、Activity生命周期，启动流程，App启动和Activity启动。
5、有没有开发过一个完整的SDK，不是在别人的基础上修改的。
6、性能优化，具体的优化过程。具体例子。
