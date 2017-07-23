---
layout: pattern
title: Strategy
folder: strategy
permalink: /patterns/strategy/
pumlid: FSV13OCm30NGLM00udktCS4AGOaJsTz5tRwSkBstLiqj3WbhombC_n0PtwbKdB67Y-MX44NAerDjSJFOwE8lRuTuBRfD1iJKgRC_88SnfFn8aD-ai9vczFO7
categories: Behavioral
tags:
 - Java
 - Difficulty-Beginner
 - Gang Of Four
---

## 也被称为
Policy

## 意图
定义一系列算法，将每个算法封装起来，并让他们可以相互替换。策略模式让算法独立于使用它的客户端而变化。

![alt text](./etc/strategy_1.png "Strategy")

## 适用性

以下情况使用策略模式

* 许多相关的类仅在其行为上有所不同。策略模式提供了一种方式，可以将类配置为许多行为之一
* 你需要一个算法的不同变体。例如，您可以定义反映不同空间/时间权衡的算法。当这些变体被实现为算法的类层次结构时，可以使用策略模式
* 一个算法使用了客户端不应该知道的数据。 使用策略模式避免暴露复杂的、特定算法的数据结构
* 一个类定义了许多行为，并且它们在其操作中显示为多个条件语句。 取代多条件，将相关的条件分支移动到自己的Strategy类中

## 感谢

* [Design Patterns: Elements of Reusable Object-Oriented Software](http://www.amazon.com/Design-Patterns-Elements-Reusable-Object-Oriented/dp/0201633612)
* [Functional Programming in Java: Harnessing the Power of Java 8 Lambda Expressions](http://www.amazon.com/Functional-Programming-Java-Harnessing-Expressions/dp/1937785467/ref=sr_1_1)
