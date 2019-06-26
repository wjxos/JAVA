volatile 是java虚拟机提供的轻量级同步机制。
1. 保证可见性：当线程A将物理内存中的共享变量从自己的内存中改变并刷新到物理内存时，对其他线程是可见的。
2. 不保证原子性：在刷回内存之前，有线程在修改主内存的数据，此时该线程会被挂起，当前一个线程执行完修改还未通知其他你线程之前，该线程继续修改主内存数据。使用atomic将能保证原子性，例如：AtomicInteger atomicInteger = new AtomicInteger();
3. 禁止指令重排:volatile 关键字禁止指令重排。

[](https://github.com/wangjianxiongwjx/JAVA/tree/master/img/volatile.png)


[](https://github.com/wangjianxiongwjx/JAVA/tree/master/img/atomicInteger.jpg)
