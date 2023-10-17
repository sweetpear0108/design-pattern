# 状态模式

状态是一种行为设计模式，当对象的内部状态发生变化时，它可以改变对象的行为。看起来好像对象更改了类。

状态模式用于分离状态和行为。

![state](../../.img/state.png?raw=true)

与策略模式比较类似，只不过状态模式类似于有限状态机`Finite-State Machine`,他涉及状态的转换，由某一个状态
自己进行切换操作，改变context中的state，而策略模式则是使用者对策略进行选择