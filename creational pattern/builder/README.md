# 创建者模式

通常用于一个巨大的复杂对象的构建，避免了写无数个参数不同的构造函数

wiki

``
The intent of the Builder design pattern is to separate the construction of a complex object from its representation. By doing so, the same construction process can create different representations.
``

builder设计模式的目的是将复杂对象的构造与其表示分离。通过这样做，相同的构造过程可以创建不同的表示。


### 例子：

![builder](../../.img/builder.png?raw=true)

汽车是一个复杂的物体，可以用一百种不同的方式建造。我们没有用一个巨大的构造函数来膨胀Car类，而是将汽车装配代码提取到一个单独的car builder类中。这个类有一组用于配置汽车各个部件的方法。
客户端可以将程序集委托给director类，director类知道如何使用builder来构建几个最流行的汽车模型。

## 参考

[wiki](https://en.wikipedia.org/wiki/Builder_pattern)

[guru](https://refactoring.guru/design-patterns/builder)