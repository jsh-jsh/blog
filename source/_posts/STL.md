---
title: STL
author: Jinshuhang
tags:
  - oi
categories: []
abbrlink: 9423
date: 2021-03-24 21:59:00
---
STL

<!-- more -->

首先，肯定是一些函数：
```cpp
make_heap(first_pointer,end_pointer,compare_function)  建堆(默认大根堆)
push_heap(first_pointer,end_pointer,compare_function) 添加元素到堆
pop_heap(first_pointer,end_pointer,compare_function) 取出堆顶元素
sort_heap() 排序堆（不推荐）
```
所有操作均为O($log_2$(n))。
建堆时，可以用定义数组，亦可以用vector。