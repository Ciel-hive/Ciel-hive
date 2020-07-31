---
title: "JVM参数"
date: 2020-06-28
category: Java
tags: [JVM]
excerpt: JVM参数说明
---

| JVM参数                         | 说明                                                         |
| :------------------------------ | ------------------------------------------------------------ |
| -Xms20m                         | 堆最小内存                                                   |
| -Xmx20m                         | 堆最大内存                                                   |
| -XX:+HeapDumpOnOutOfMemoryError | 让虚拟机在内存溢出是Dump当前内存堆转储快照                   |
| -Xoss                           | 设置本地方法栈的大小，但实际上是无效的（通过-Xss参数设置）   |
| -Xss                            | 设置每个线程的堆栈大小                                       |
| -XX:PermSize                    | 表示非堆区初始内存分配大小，其缩写为permanent size（持久化内存） |
| -XX:MaxPermSize                 | 表示对非堆区分配的内存的最大上限                             |
| -XX:MaxDirectMemorySize         |                                                              |

