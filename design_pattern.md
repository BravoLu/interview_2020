# 设计模式

1. 单例模式

   1. 私有化构造函数
   2. 使用类的私有静态指针变量指向类的唯一实现
   3. 使用一个公有的静态方法获取实例

   * 懒汉式（线程不安全，用锁解决）

   * 饿汉式（线程安全，效率低）

     

![pic](images/singlemode.jpg)

2. 工厂模式
   * 简单工厂模式
   * 抽象工厂模式
   * 工厂方法模式