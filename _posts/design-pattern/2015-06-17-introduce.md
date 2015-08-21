---
layout: post
title: 设计模式简介
---

设计模式简介
=========
   
  设计模式（Design pattern）是一套被反复使用、多数人知晓的、经过分类编目的、代码设计经验的总结。使用设计模式是为了可重用代码、让代码更容易被他人理解、保证代码可靠性。 设计模式使代码编制真正工程化。设计模式提供了一套术语方便开发人员之间的交流，但是不能滥用设计模式，导致设计过度。

----------

# 设计原则
  
  面向对象开发设计需要遵循一下的原则：
  
## 开闭原则(Open Closed Principle，OCP)

  软件应当对扩展开放，对修改关闭。
* 对于扩展是开放的(Open for extension)，这意味着模块的行为是可以扩展的。当应用的需求改变时，我们可以对模块进行扩展，使其具有满足那些改变的新行为。也就是说，我们可以改变模块的功能。
* 对于修改是关闭的(Closed for modification)，对模块行为进行扩展时，不必改动模块的源代码或者二进制代码。类的修改只应该因错误而修改。
## 里氏代换原则(Liskov Substitution Principle，LSP)
  
## 依赖倒转原则(Dependency Inversion Principle，DIP)

1. 高层次的模块不应该依赖于低层次的模块，他们都应该依赖于抽象。
2. 抽象不应该依赖于具体，具体应该依赖于抽象。 
  
 这个原则反转两个字需要从设计的角度去理解，很多时候接口的抽象都依赖于具体的应用，导致增加一个具体应用就增加一个接口，这其实是不符合依赖倒转原则的。 
  依赖倒转原则的重要应用就是控制反转(Inversion of Control, IoC)一般分为两种类型，依赖注入(Dependency Injection, DI)和依赖查找(Dependency Lookup)。
  
## 接口隔离原则(Interface Segregation Principle，ISP)
  
  一个类对另外一个类的依赖性应当是建立在最小的接口上。使用多个专门的接口比使用单一的总接口要好。
  
## 合成/聚合复用原则(Composite/Aggregate Reuse Principle，CARP)
  
  合成复用原则是指尽量使用合成/聚合，而不是使用继承。首先要区分区分Has-A和Is-A的关系，然后当满足以下的条件时，才使用继承关系。
  
1. 子类具有扩展超类的责任，而不是具有置换掉或注销掉超类的责任。
2. 不会出现需要将子类换成另外一个类的子类的情况。
  
## 最小知识原则(Principle of Least Knowledge，PLK，也叫迪米特法则Law of Demeter)
   
  每一个软件单位对其他的单位都只有最少的知识，而且局限于那些与本单位密切相关的软件单位。迪米特法则的初衷在于降低类之间的耦合。由于每个类尽量减少对其他类的依赖，因此，很容易使得系统的功能模块功能独立，相互之间不存在（或很少有）依赖关系。

----------

# 常用模式

  常用的设计模式可分为三种类型，分别为创建型模式、结构型模式和行为型模式。
   
## 建型模式
  
* [单例模式](/2015/06/18/singleton.html)
* [工厂模式](/2015/06/20/factory.html)
* [抽象工厂模式](/2015/06/20/factory.html)
* [建造者模式](/2015/07/29/builder.html)
* [原型模式](/2015/06/21/prototype.html)
   
## 结构型模式
  
* [适配器模式](/2015/06/27/adapter.html)
* [桥接模式](/2015/08/10/bridge.html)
* [装饰模式](/2015/06/24/decorator.html)
* [组合模式](/2015/07/23/composite.html)
* [外观模式](/2015/07/19/facade.html)
* [享元模式](/2015/06/26/flyweight.html)
* [代理模式](/2015/08/11/proxy.html)
  
## 行为型模式
  
* [模版方法模式](/2015/06/22/template.html)
* [命令模式](/2015/08/13/command.html)
* [迭代器模式](/2015/08/12/iterator.html)
* [观察者模式 ](/2015/08/04/observer.html)
* [中介者模式](/2015/08/04/mediator.html)
* [备忘录模式](/2015/08/14/memento.html)
* [解释器模式](/2015/08/17/interpreter.html)
* [状态模式](/2015/06/25/state.html)
* [策略模式](/2015/06/23/strategy.html)
* [责任链模式](/2015/08/12/chain_of_responsibility.html)
* [访问者模式](/2015/07/24/visitor.html)
   
----------
  
# 各模式之间的关系下图

![relationship](/images/design-pattern/relationship.png)
   
# 参考
[百度百科](http://baike.baidu.com/link?url=8HuuLmplQp0-iBZRDMyq8C7TCAHDRB0wNGMCVOjTe362nO9qqcKmZnSpm9c5xk5IsugUPBe_Zd-jVcj6ogiUwa)
<http://blog.csdn.net/longronglin/article/details/1454315>