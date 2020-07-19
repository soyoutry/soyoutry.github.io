---
title: Java中的内存
date: 2020-07-19 16:00:03
tags: java
categories: java
cover: false
---


Java的内存分为5个部分：

- 栈(Stack)：存放方法中的局部变量

- 堆(Heap)：对象都在堆中存放

  - 堆中的内容中都有一个16进制的地址值

    | 类型     | 默认值   |
    | -------- | -------- |
    | 整数     | 0        |
    | 浮点数   | 0.0      |
    | 字符     | ‘\u0000’ |
    | 布尔     | false    |
    | 引用类型 | null     |

- 方法区(Method Area)：存储.class相关信息，包含方法的信息。
- 本地方法栈(Native Method Stack)：操作系统相关。
- 寄存器(PC Register)：CPU相关。

