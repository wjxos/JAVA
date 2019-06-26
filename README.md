# JAVA
## java基础

### Java 集合

*  **List：** 可以有对个元素是相同的对象，list是有序的。
*  **Set：** 每个对象是都是唯一的，无序的。
*  **Map：** key value的形式存在，不同的key可以有相同的对象，常见的key是String， 也可以是一个对象。

* **ArrayList与LinkedList的区别**
ArrayList  是Object数组，是有序的，连续的，查询效率高，由于删除和插入要移动内存，所以删除和插入的速度慢，适合频繁的读操作
LinkedList是双向链表结构，查询时需要从头部一个个查找，查询效率低，插入和删除只需改变引用即可，所以插入和删除的效率高，适用于查询比较少，插入和删除操作比较多的情况；
ArrayList和LinkedList都是非线程安全的；

* **HashMap与HashTable的区别**
HashMap允许key和value为null值，是线程不安全的，操作比较快。
HashTable是线程安全的，不允许NULL为key和value，操作比较慢。
concurrentHashMap 结合了两者的优缺点；


* **Runnable与CallAble的区别**
Runnable 没有返回值 void 方法，异常只能在内部处理。
Callable 返回当前线程的执行结果，可以抛出异常。

* **有了基本类型，为什么还要包装类型**
```
每个基本类型都会有一个包装类型；
装箱： 将基本类型转换为包装类型
拆箱： 将包装类型转换为基本类型
java 是面向对象的，而基本类型不具备对象的特征。
```

* **== 和 equals 的区别**
```
== 在基本类型中，判断两个变量的值是否相等；
应用类型比较对应的首地址。
equals 用来比较两个对象的特征是否一样，
```

* **String StringBuilder 和 StringBuffer 的区别**
```
String是被final修饰过的一个类，是一个不可变的字符数字。
StringBuilder和StringBuffer是可变的字符数组，在拼接字符串时,效率高于String。
StringBuilder是非线程安全的，效率高。
StringBuffer是线程安全的，效率低。
```

* **String StringBuilder 和 StringBuffer 的区别**
```
String是被final修饰过的一个类，是一个不可变的字符数字。
StringBuilder和StringBuffer是可变的字符数组，在拼接字符串时,效率高于String。
StringBuilder是非线程安全的，效率高。
StringBuffer是线程安全的，效率低。
```

