---
layout: post
title: 委托模式
---

委托模式(delegation)
==================
  
  被委托者(delegate)被赋予执行委托者(delegator)任务的权限。这里面存在着责任反转(Inversion of Responsibility)，一般情况下是主对象调用其他协助对象(helper object)，然后由主对象来执行任务，而在委托模式中则是主对象将任务委托给协助对象，由协助对象来执行任务。
  和代理(proxy)模式是委托模式的一种特殊形式，代理模式是代理同种类型的对象，在类型上有点限制，而委托模式可以委托其他类型的的对象，更广泛。
   委托模式是很多其他模式的基础，如组合(聚合)，混合(mixins)和切面(aspects)。








# 参考
<https://en.wikipedia.org/wiki/Delegation_pattern>