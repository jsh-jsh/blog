---
title: 一个简单数学问题的证明
date: 2022-8-7
tags: 随笔
categories: 随笔
---
以下中 (a,b) 表示组合数，从 a 中选取 b 个

在一个圆上的一般位置上取n个点，把每个点连接起来，然后找到(n+3,6)+(n+1,5)+(n,5)  
这将产生一个序列。

该公式的证明需要4个步骤

圆上有3个角的三角形的数量是(n,3)

证实。任何三个角都可以定义这样一个三角形，反之亦然。

圆上正好有两个角的三角形的数量是4(n,4)

证明。对于任何4个角的选择，有4个这样的三角形

圆上正好有一个角的三角形的数量是5(n,5)。

证明。对于任何5个角的选择，都有5个这样的三角形

圆上没有角的三角形的数量是(n,6)。

证明。对于任何6个角的选择，正好有一个这样的三角形

三角形的总数为
(n,6)+5(n,5)+4(n,4)+(n,3)

=(n+3,6)+(n+1,5)+(n,5)证明。

有定理：(n+1,m)=(n,m)+(n,m-1)

原式子= (n,6)+(n,5)+4(n,5)+4(n,4)+(n,3)

            =(n+1,6)+4(n+1,5)+(n,3)

            =(n+2,6)+3(n+1,5)+(n,3)

            =(n+2,6)+2(n+1,5)+(n,5)+(n,4)+(n,3)

            =(n+2,6)+2(n+1,5)+(n,5)+(n+1,4)

            =(n+2,6)+(n+1,5)+(n+1,4)+(n+1,5)+(n,5)

            =(n+3,6)+(n+1,5)+(n,5)
