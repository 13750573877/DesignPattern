# 外观模式
外观模式属于结构型模式，它隐藏了系统的复杂性，并向客户端提供了一个客户端可以访问系统的接口。  
为子系统中的一组接口提供了一个统一的访问接口，这个接口使得子系统更容易被访问或者使用。  

应用场景：  
1. 开发阶段，子系统越来越复杂，增加外观模式提供一个简单的调用接口。  
2. 维护一个大型遗留系统的时候，可能这个系统已经非常难以维护和扩展，但又包含非常重要的功能，为其开发一个外观类，以便新系统与其交互。  

优点：  
1. 实现了子系统与客户端之间的松耦合关系。  
2. 客户端屏蔽了子系统组件，减少了客户端所需处理的对象数目，并使得子系统使用起来更加容易。  

缺点：  
1. 不符合开闭原则，如果要修改某一个子系统的功能，通常外观类也要一起修改。  
2. 没有办法直接阻止外部不通过外观类访问子系统的功能，因为子系统类中的功能必须是公开的（根据需要决定是否使用internal访问级别可解决这个缺点，但外观类需要和子系统类在同一个程序集内）。