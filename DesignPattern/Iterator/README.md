# 迭代器模式
提供一种方法访问一个聚合对象中的各个元素，而又不暴露其内部的表示。  
迭代器模式就是抽象一个迭代器类来分离了集合对象的遍历行为，这样既可以做到不暴露集合的内部结构，又可让外部代码透明地访问集合内部的数据。  

* 应用场景
  > 支持对聚合对象的多种遍历。  

  > 为遍历不同的聚合结构提供一个统一的接口（即支持多态迭代）。  

* 优点
  > 迭代器模式使得访问一个聚合对象的内容而无需暴露它的内部表示，即迭代抽象。  

  > 迭代器模式为遍历不同的集合结构提供了一个统一的接口，从而支持同样的算法在不同的集合结构上进行操作。  

* 缺点
  > 迭代器模式在遍历的同时更改迭代器所在的集合结构会导致出现异常。所以使用foreach语句只能在对集合进行遍历，不能在遍历的同时更改集合中的元素。  

* .Net中迭代器模式的应用
  > 在mscorlib程序集里有这样一个命名空间：System.Collections，在该命名空间里面早已有了迭代器模式的实现。其中IEnumerator扮演的就是迭代器的角色，IEnumerable则扮演的就是抽象聚集的角色。  