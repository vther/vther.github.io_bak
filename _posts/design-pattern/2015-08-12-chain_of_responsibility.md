---
layout: post
title: 责任链模式
---

责任链模式(Chain of Responsibility)
================================
  
  在责任链模式里，很多对象由每一个对象对其下家的引用而连接起来形成一条链。请求在这个链上传递，直到链上的某一个对象决定处理此请求。发出这个请求的客户端并不知道链上的哪一个对象最终处理这个请求，这使得系统可以在不影响客户端的情况下动态地重新组织和分配责任。
 
![Chain of Responsibility1](/images/design-pattern/Chain of Responsibility1.png)
   
  直观的看是这个样子的：
   
![Chain of Responsibility2](/images/design-pattern/Chain of Responsibility2.png)
   
