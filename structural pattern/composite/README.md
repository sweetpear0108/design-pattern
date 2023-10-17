# 组合模式

组合模式统一对象和对象集，使得使用相同接口使用对象和对象集。

组合模式常用于树状结构，用于统一叶子节点和树节点的访问，并且可以用于应用某一操作到所有子节点。

Decorator类似于Composite，但只有一个子组件。还有另一个显著的区别：Decorator为被包装的对象添加了额外的责任，而Composite只是“总结”了其子对象的结果。
然而，模式也可以协作：您可以使用Decorator来扩展Composite树中特定对象的行为。