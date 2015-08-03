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

## 里氏代换原则(Liskov Substitution Principle，LSP)

## 依赖倒转原则(Dependency Inversion Principle，DIP)

## 接口隔离原则(Interface Segregation Principle，ISP)

## 合成/聚合复用原则(Composite/Aggregate Reuse Principle，CARP)

## 最小知识原则(Principle of Least Knowledge，PLK，也叫迪米特法则)
  
----------

# 常用模式

  常用的设计模式可分为三种类型，分别为创建型模式、结构型模式和行为型模式。
   
## 建型模式
* [单例模式](/2015/06/18/singleton.html)
* [抽象工厂模式](/2015/06/20/factory.html)
* [建造者模式](/2015/07/29/builder.html)
* [工厂模式](/2015/06/20/factory.html)
* 原型模式
   
## 结构型模式
* 适配器模式
* 桥接模式
* 装饰模式
* [组合模式](/2015/07/23/composite.html)
* [外观模式](/2015/07/19/facade.html)
* 享元模式
* 代理模式
 
## 行为型模式
* 模版方法模式
* 命令模式
* 迭代器模式
* 观察者模式 
* 中介者模式
* 备忘录模式
* 解释器模式
* 状态模式
* 策略模式
* 职责链模式
* [访问者模式](/2015/07/24/visitor.html)

----------
  
# 各模式之间的关系下图

![relationship](/images/design-pattern/relationship.png)
   
# 参考
[百度百科](http://baike.baidu.com/link?url=8HuuLmplQp0-iBZRDMyq8C7TCAHDRB0wNGMCVOjTe362nO9qqcKmZnSpm9c5xk5IsugUPBe_Zd-jVcj6ogiUwa)
<http://blog.csdn.net/longronglin/article/details/1454315>