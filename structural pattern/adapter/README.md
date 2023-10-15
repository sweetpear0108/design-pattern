# 适配器模式

Adapter是一个既能处理客户端又能处理服务的类：它实现客户端接口，同时包装服务对象。适配器通过客户端接口接收来自客户端的调用，并将它们转换为能够被封装服务对象所理解的格式的调用。

简而言之，adapter通过extend服务的类和implement客户端接口实现了对于调用格式的统一

btw：适配器模式在可以多继承的语言中还有一种名为 `class adapter`（类适配器）的模式，他是同时继承了客户端接口和服务接口。上边说的这类模式则为 `object adapter` （对象适配器）


实际使用中 `Adaptee` 一般为接口，并且使用工厂函数生成实例。

在 `Adapter` 中匿名组合 `Adaptee` 接口，所以 `Adapter` 类也拥有 `SpecificRequest` 实例方法，又因为 `Go` 语言中非入侵式接口特征，其实 `Adapter` 也适配 `Adaptee`
接口。

## object adapter

![object](../../.img/structure-object-adapter.png)

## class adapter

![class](../../.img/structure-class-adapter.png)