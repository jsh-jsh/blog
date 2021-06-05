---
title: CF195A-Let's Watch Football
author: Jinshuhang
tags:
  - oi
categories: 题解
abbrlink: 13193
date: 2021-03-24 22:00:00
---
这题不难，运用乘法分配律可以解出。

题目中给出了方程：$tb+cb=ac$，根据乘法分配律可以把这个式子变成如下：$(t+c)b=ac$，接下来解方程就可以了。

注意：向上取整使用函数 ceil，在 cmath 库里。
 
代码： 
```cpp
#include<bits/stdc++.h>//万能头
#define ll long long
using namespace std;
ll a,b,c;
int main(){
	cin>>a>>b>>c;
	ll ac=a*c;
	ac=ceil(ac*1.0/b);//向上取整
	ac-=c;//减去c得到t
	cout<<ac;
	return 0;
}
```
