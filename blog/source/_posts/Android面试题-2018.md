---
title: Android面试题(2018)
date: 2018-07-15 21:02:30
tags:Android面试
category: Android
toc: true
---

### 一、Java知识

1、Java特性，多态，封装，继承。
2、Java集合框架Collection：

- ArrayList 数组非同步
- Vector 同步
- LinkedList 链表非同步
- HashMap 数组+链表，jdk1.8之后链表长度超8时变成红黑树。非同步
- HashTable 同步
- LinkedHashMap 双向链表+HashMap
- ConcurrentHashMap

3、多线程，并发及线程基础。
多线程安全问题，不加锁怎么保证安全性？
加锁的机制是什么，monitor相关知识点。
有哪些锁？
手写一个死锁的例子，线程运行顺序等。
线程池，同步处理，锁。synchronize自动释放，性能低，lock手动释放。
4、jvm虚拟机，垃圾回收（GC），内存模型。
GCRoots：

- 虚拟机栈(栈桢中的本地变量表)中的引用的对象
- 方法区中的类静态属性引用的对象
- 方法区中的常量引用的对象
- 本地方法栈中JNI的引用的对象

5、设计模式。平常使用的设计模式。23种设计模式。
6、抽象类与接口。
7、Java IO 与 NIO。
8、Java数据结构和算法。
9、基础类型。
10、Serializable和Parcelable。
11、sleep和wait的区别，sleep不释放锁，wait释放锁。
12、SpareArray
13、生产者和消费者模式,使用不同的锁实现，wait()和notify(),ReentrantLock,Condition
14、SingleTon的饿汉和懒汉
**饿汉：**
```
private SingleTon(){

}
//性能高点，适合很多地方使用时初始化
private static final INSTANCE = new SingleTon();

public SingleTon getSingleTon(){
	return INSTANCE;
}
```
**懒汉：**
```
private SingleTon(){

}
private static INSTANCE = null

public SingleTon getSingleTon(){
	if(INSTANCE == null){
    	synchronized (SingleTon.class){
        	if(INSTANCE == null){
            	INSTANCE = new SingleTon();
            }
        }
    }
}


```

### 二、Android相关知识
1、四大组件。
2、IntenService工作原理。
3、Hadnler原理，消息机制。
4、View绘制流程，ViewGroup。
5、事件分发机制。
6、app启动过程，桌面启动，普通启动。
7、binder 和 aidl。
数据拷贝只需要一次，
8、Fragment。
9、AsyncTask。
10、动画帧动画，补间动画，属性动画。
11、Context。
12、线程和线程池。
13、postInvalidate，可用于线程刷新UI。
14、OOM，ANR的问题。主线程5s，广播10s，服务20s。
15、内存泄漏。

- 非静态内部类的静态对象
- 单例导致，单例使用非ApplicationContext
- Handler和主线程Looper还有MessageQueue关联
- 广播注册后没有反注册
- 文件，corsor等没有关闭
- WebView

16、LruCache原理
17、ListView和RecyclerView的差别
18、子线程为什么不能更新UI，到处都去更新，引起絮乱咋办。
19、进程保活。
20、开源库

- Retrofit 动态代理
- OkHttp
- Volley
- RxJava 观察者模式
- EventBus 反射和注解
- Fresco
- Picasso
- Glide

21、性能优化

- SysTrace 网页查看，耗时的地方，onLayout，onDraw等
- TraceView 方法占用CPU和调用次数
- HoerarchyViewer 查看布局层级
- Leakcanary 内存泄漏
- StrictMode 主线程IO，网络，读写DB，没有关闭file，cursor等
- GPU／CPU／Memory Monitor 查看对应资源的使用情况
- MAT（Memory Analyzer Tool）生成hprof，查看GCRoot引用链，查看内存泄漏问题

22、ActivityManagerService，PackageManagerService，WindowManagerService。
23、MVC，MVP，MVVM。
24、图片加载和处理。
25、int和Integer的区别
Integer里-128～127会进行缓存，所以如果用==比较，部分情况会不期效果。
26、插件化，热更新。
27、ByBrid开发，weex,react native,flutter
28、Kotlin,Dart
29、TCP，UDP的区别，三次握手，四次握手。
30、网络模块，自己实现一个网络请求框架。长链接。


### 三、数据结构和算法
至少需要会手写这些：
1、快速排序
2、冒泡排序
3、插入排序
4、二分查找

### 四、app开发的架构
1、通过需求分析，分析业务逻辑确定app框架。搭建框架目的是为了解耦，代码复用性和阅读效果，利于协助开发，稳定性和利于维护以及扩展，目前流行的框架MVP，MVVM，MVC都是经过长时间的市场考验，很值得借鉴。是否需要考虑跨平台。
2、UI架构的搭建，功能模块的划分，注册登录模块，用户模块，消息通知，设置等。
3、数据交互和API接口的定义，数据库的设计。
4、第三方库的引入，网路请求，异步同步处理，图片加载以及缓存等。
5、推送功能模块。
6、数据统计。
7、云通讯，地图定位。
8、开发过程把与业务无关的工具库独立出来。
9、性能测试，压力测试等。
10、Logger模块。
