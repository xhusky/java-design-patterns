---
layout: pattern
title: Visitor
folder: visitor
permalink: /patterns/visitor/
pumlid: DSR14OGm20NGLhG0mtsxmSWeJa8oyD7sTo_xJczLgoqFIM_B1Spu43c_vLHSkMU8rs4GGwcZaxPy6UnqyyFR8Q6dRPC1SGlg7B_Gew4OJeBwVqdlPMPlNm00
categories: Behavioral
tags:
 - Java
 - Difficulty-Intermediate
 - Gang Of Four
---

## 意图

表示对对象结构中元素的操作。访问者使你可以在不改变各元素的类的前提下定义对这些元素的新操作。

![alt text](./etc/visitor_1.png "Visitor")

## 适用性

以下情况使用访问者模式（Visitor pattern）

* 对象结构包含许多具有不同接口的对象类，并且你希望对这些依赖于具体类的对象执行操作
* 需要对对象结构中的对象执行许多不同且不相关的操作，并且你希望避免使用这些操作“污染”他们的类。 访问者可以通过在一个类中定义相关操作来保持相关的操作。当对象结构由许多应用程序共享时，使用Visitor将操作放在需要它们的应用程序中
* 定义对象结构的类很少更改，但是您经常希望在结构上定义新的操作。 更改对象结构类需要重新定义所有访问者的接口，这可能是昂贵的。 如果对象结构类经常发生变化，那么最好在这些类中定义操作

## 真实世界的例子 

* [Apache Wicket](https://github.com/apache/wicket) component tree, see [MarkupContainer](https://github.com/apache/wicket/blob/b60ec64d0b50a611a9549809c9ab216f0ffa3ae3/wicket-core/src/main/java/org/apache/wicket/MarkupContainer.java)
* [javax.lang.model.element.AnnotationValue](http://docs.oracle.com/javase/8/docs/api/javax/lang/model/element/AnnotationValue.html) and [AnnotationValueVisitor](http://docs.oracle.com/javase/8/docs/api/javax/lang/model/element/AnnotationValueVisitor.html)
* [javax.lang.model.element.Element](http://docs.oracle.com/javase/8/docs/api/javax/lang/model/element/Element.html) and [Element Visitor](http://docs.oracle.com/javase/8/docs/api/javax/lang/model/element/ElementVisitor.html)
* [java.nio.file.FileVisitor](http://docs.oracle.com/javase/8/docs/api/java/nio/file/FileVisitor.html)

## 感谢

* [Design Patterns: Elements of Reusable Object-Oriented Software](http://www.amazon.com/Design-Patterns-Elements-Reusable-Object-Oriented/dp/0201633612)
