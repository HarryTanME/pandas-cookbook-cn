Pandas 手册
===============

[pandas](http://pandas.pydata.org/) 是一个用于数据分析的Python库，它能让你快速处理一些探索性的工作。

本手册的目的通过一些实际的例子来让你开始使用pandas。
Pandas 的[帮助文档](http://pandas.pydata.org/pandas-docs/stable/)已经相当全面了。不过，经常会有人询问
应该怎样上手。接下来我讲讲如何用pandas来处理一些真实世界中的数据，如你所料，这些数据包含各种bug和异常值。

接下来我会使用以下3个数据

* 311 calls in New York
* How many people were on Montréal's bike paths in 2012
* Montreal's weather for 2012, hourly

这些数据已经包含在本目录下。

目录
=================


* [简单介绍下Ipython Nodebook](http://nbviewer.ipython.org/github/jvns/pandas-cookbook/blob/master/cookbook/A%20quick%20tour%20of%20IPython%20Notebook.ipynb)
  <br> 展示了如何使用IPython的tab自动补齐和魔法函数
* [Chapter 1: 从CSV文件中读取数据](http://nbviewer.ipython.org/github/jvns/pandas-cookbook/blob/master/cookbook/Chapter%201%20-%20Reading%20from%20a%20CSV.ipynb)
  <br> 将数据导入到pandas是相当容易的一件事，即使有编码错误也不是问题！
* [Chapter 2: 选择和查找数据](http://nbviewer.ipython.org/github/jvns/pandas-cookbook/blob/master/cookbook/Chapter%202%20-%20Selecting%20data%20&%20finding%20the%20most%20common%20complaint%20type.ipynb)
  <br>从pandas的DataFrame中选择数据有时候显得不那么直观,在这一部分我将解释一些基本的东西（比如怎么做切片操作，选取指定列）
* [Chapter 3: “哪个区抱怨噪声的人最多？”(查找数据进阶)](http://nbviewer.ipython.org/github/jvns/pandas-cookbook/blob/master/cookbook/Chapter%203%20-%20Which%20borough%20has%20the%20most%20noise%20complaints%20%28or%2C%20more%20selecting%20data%29.ipynb)
  <br>这部分将继续介绍如何对数据切片、切块以及过滤处理。
* [Chapter 4: 用groupby和agg操作来查找人们骑自行车最多的一天是星期几](http://nbviewer.ipython.org/github/jvns/pandas-cookbook/blob/master/cookbook/Chapter%204%20-%20Find%20out%20on%20which%20weekday%20people%20bike%20the%20most%20with%20groupby%20and%20aggregate.ipynb)
  <br> groupby/aggregate操作 是我最喜欢pandas的地方，我几乎无时不刻都在用它。这部分必读！
* [Chapter 5: 融合DataFrame并抓取加拿大气候数据](http://nbviewer.ipython.org/github/jvns/pandas-cookbook/blob/master/cookbook/Chapter%205%20-%20Combining%20dataframes%20and%20scraping%20Canadian%20weather%20data.ipynb)
  <br>Here you get to find out if it's cold in Montreal in the winter (spoiler: yes). Web scraping with pandas is fun!
  <br>这部分将会探索Montreal的冬天冷不冷（答案：冷！），用pandas来做网页抓取相当有意思。
* [Chapter 6: String操作：哪个月下雪最多？](http://nbviewer.ipython.org/github/jvns/pandas-cookbook/blob/master/cookbook/Chapter%206%20-%20String%20Operations-%20Which%20month%20was%20the%20snowiest.ipynb)
  <br> Strings with pandas are great. It has all these vectorized string operations and they're the best. We will turn a bunch of strings containing "Snow" into vectors of numbers in a trice.
  <br> pandas对string的操作非常好，它包含所有向量化的string操作。这部分内容将一系列包含Snow的字符串转换成向量化的数值来表示。
* [Chapter 7: 处理脏数据](http://nbviewer.ipython.org/github/jvns/pandas-cookbook/blob/master/cookbook/Chapter%207%20-%20Cleaning%20up%20messy%20data.ipynb)
  <br> 处理脏数据可不轻松，不过对于pandas来说，那就是另外一回事了～
* [Chapter 8: 解析Unix下的时间戳](http://nbviewer.ipython.org/github/jvns/pandas-cookbook/blob/master/cookbook/Chapter%208%20-%20How%20to%20deal%20with%20timestamps.ipynb)
  <br> 这个小技巧花了我两天才弄明白。。。
* [Chapter 9 - 从SQL数据库中导入数据](http://nbviewer.ipython.org/github/jvns/pandas-cookbook/blob/master/cookbook/Chapter%209%20-%20Loading%20data%20from%20SQL%20databases.ipynb)
  <br> 本部分将介绍如何从 SQLite3, PostgreSQL及MySQL中导入数据到pandas

怎么使用Panda手册
========================

首先，你需要更新下IPython Notebook(&gt;= 3.0) 以及 pandas(&gt;=0.13)

用pip可以完成以上操作：

```
pip install ipython pandas numpy tornado pyzmq jinja2 matplotlib
```

编译和配置这些有时候挺繁琐的，我自己是用的
[Anaconda](https://store.continuum.io/),这个软件把几乎所有你能想到的库都包含了，并且是免费和开源的。

安装好IPython和pandas后就可以开始啦～

```
git clone https://github.com/jvns/pandas-cookbook.git
cd pandas-cookbook/cookbook
ipython notebook
```

执行完以上命令后，你的浏览器会自动打开一个地址为 `http://localhost:8888`的页面。

尽情享受吧～

Contribute!
===========

如果你发现某些地方有错误，或者是你想学习一些我在这里没有讲到的东西，
又或者是你想分享些东西，赶紧发个issue，或者发邮件，pull request都行！


TODO
====

* join 操作
* 使用 stack/unstack
* ???


License
=======

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="http://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/)
