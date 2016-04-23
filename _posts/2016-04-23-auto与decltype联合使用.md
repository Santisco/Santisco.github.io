---
layout: post
title: 将auto与decltype联合使用
---
这种效果爽的飞起而且装逼属性满满，当我使出这个的时候以我身边那些渣渣的水平一定看不懂的。原理有点类似于动态语言根据decltype确定前面auto的类型<br>

<code>
template<class T><br>
auto getSize(T data) -> decltype( data.size() ){<br>
return data.size();<br>
}<br>
vector<int> x;<br>
cout << getSize(x) << endl;<br>
<code>

<a href="http://blog.csdn.net/yshe_xun/article/details/7315135">auto&decltype</a>
<a href="https://www.quora.com/Why-is-C++-so-hard">decltype</a>


