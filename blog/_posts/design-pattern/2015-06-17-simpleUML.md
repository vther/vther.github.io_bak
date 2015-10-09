---
layout: post
title: UML 类图简介
---

UML 类图简介
==========

## 泛化(generalization)
泛化关系是一个类（称为子类、子接口）继承另外的一个类（称为父类、父接口）的功能，并可以增加它自己的新功能的能力，继承是类与类或者接口与接口之间最常见的关系(extends)
   
  ![generalization](/images/design-pattern/extends.jpg)

## 实现(realization)
  实现关系指的是一个class类实现interface接口（可以是多个）的功能；实现是类与接口之间最常见的关系(implements)
   
  ![realization](/images/design-pattern/implements.jpg)
  
## 依赖关系(dependency)
  依赖关系: 也是类与类之间的连接. 表示一个类依赖于另一个类的定义. 依赖关系总是单向的 。可以简单的理解，就是一个类A使用到了另一个类B，而这种使用关系是具有偶然性的、、临时性的、非常弱的，但是B类的变化会影响到A；比如某人要过河，需要借用一条船，此时人与船之间的关系就是依赖
  
  ![dependency](/images/design-pattern/dependency.jpg)

## 关联关系(association)
  关联(association)关系: 表示类与类之间的联接, 它使一个类知道另一个类的属性和方法. 
  关联可以使用单箭头表示单向关联, 使用双箭头或不使用箭头表示双向关联, 不建议使用双向关联. 关联有两个端点, 在每个端点可以有一个基数, 表示这个关联的类可以有几个实例. 
  
  ![generalization](/images/design-pattern/association.jpg)
   
常见的基数及含义: 
0..1:0 或1 个实例. 
0..*: 对实例的数目没有限制. 
1: 只能有一个实例. 
1..*: 至少有一个实例. 

## 聚合关系(aggregation)
  聚合关系: 关联关系的一种特例, 是强的关联关系. 聚合是整体和个体之间的关系,即has-a的关系，此时整体与部分之间是可分离的，他们可以具有各自的生命周期，部分可以属于多个整体对象，也可以为多个整体对象共享；比如计算机与CPU、公司与员工的关系等；表现在代码层面，和关联关系是一致的，只能从语义级别来区分。
   
  ![aggregation](/images/design-pattern/aggregation.jpg)

## 组合(合成)关系(composition)
  组合/合成关系: 也是关联关系的一种特例，他体现的是一种contains-a的关系，这种关系比聚合更强，也称为强聚合；他同样体现整体与部分间的关系，但此时整体与部分是不可分的，整体的生命周期结束也就意味着部分的生命周期结束；比如你和你的大脑；合成关系不能共享. 。表现在代码层面，和关联关系是一致的，只能从语义级别来区分。组合跟聚合几乎相同，唯一的区别就是“部分”不能脱离“整体”单独存在，就是说， “部分”的生命期不能比“整体”还要长。
  ![composition](/images/design-pattern/composition.jpg)
   
  关系所表现的强弱程度依次为：组合>聚合>关联>依赖

[参考](http://justsee.iteye.com/blog/808799)