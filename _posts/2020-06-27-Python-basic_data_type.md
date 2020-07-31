---
title: "Python数据类型"
date: 2020-06-27
category: Python
tags: [Basics]
excerpt: 本文主要介绍Python的数据类型(Number、String、List、Tuple、Dictionary、Set)以及类型之间的转换
---

# 标准数据类型([类型转换](#TypeChange))
 > - [Numbers(数字)](#Number) 
 > - [String(字符串)](#String)
 > - [List(列表)](#List)
 > - [Tuple(元组)](#Tuple)
 > - [Dictionary(字典)](#Dictionary)
 > - [Set(集合)](#Set)

 

<h3 id='Number'>1. Number(数字)<sup><a href="#Top">Top</a></sup></h3>
 > - 当指定值时,Number被创建

    var1 = 1
 > - 删除对象引用

    del var
    del var_a, var_b
 > - 支持四种数字类型：
	 - int(整数),如1,只有一种整数类型int,表示长整型,没有			python2中的Long
	 - bool(布尔),如True
	 - float(浮点数),如1.23、3E-2
	 - complex(复数),如1 + 2j、1.1 + 2.2j
 > - 内置type()函数查询变量所指的对象类型

```
 a, b, c, d = 1, 1.0, 'gool', True
 print(type(a), type(b), type(c), type(d))
```
 > 输出:  

```
 <class 'int'> <class 'float'> <class 'str'> <class 'bool'>
```
 - 还可以使用isinstance来判断

```
 a = 11.0
 print(isinstance(a, float))
```
 > 输出:

```
 True
```

 > - isinstance和type的区别:
	- type()不会认为子类是一种父类类型
	- isinstance()会认为子类是一种父类类型

<h3 id="String">2. String(字符串)<sup><a href="#Top">Top</a></sup></h3>
 > - python中的单引号和双引号使用完全相同;
 > - 使用三引号('''或""")可以指定一个多行字符串;
 > - 转义符'\\'
 > - 反斜杠可以用来转义,使用r可以让反斜杠不发生转义.

```
 print(r'This is string \n')
```

 > 输出:

```
 This is string \n
```

 > - 按字面意思级联字符串,如"this""is""string"会被自动转换成thisisstring
 > - 字符串可以用+运算符连接在一起,用*运算符重复
 > - Python中的字符串有两种索引方式,从左往右以0开始,从右往左以-1开始
 > - Python中的字符串不能改变
 > - Python没有独立的字符类型,一个字符就是长度为1的字符串
 > - 字符串截取语法:`变量[头下标:尾下标:步长]`

<h3 id="List">3. List(列表)<sup><a href="#Top">Top</a></sup></h3>
 > - 支持字符,数字,字符串或者列表;
 > - 用`[ ]`标识
 > - 使用`[头下标:尾下标]`切割,操作与字符串截取相同。

<h3 id="Tuple">4. Tuple(元组)<sup><a href="#Top">Top</a></sup></h3>
    - 类似于List
    - 使用`()`标识,内部元素用逗号隔开
    - 元组不能二次赋值,相当于只读列表
<h3 id="Dictionary">5. Dictionary(字典)<sup><a href="#Top">Top</a></sup></h3>
 > - 列表是有序对象的集合,字典是无序对象的集合
 > - 字典由索引(key)和它对应的值value组成,通过键来取值
 > - 字典使用`{}`标识

```
a = dict()
b = {}
a['name'] = 'jick'
b['name'] = 'gool'
print(a['name'])
print(b['name'])
```

<h3 id="Set">6. Set(集合)<sup><a href="#Top">Top</a></sup></h3>
 > - 可以使用`{ }`或者`set()`函数创建集合
 > - 创建空集合必须使用`set()`而不能使用`{ }`,因为`{ }`是用来创建空字典的

<h3 id="TypeChange">7. Python数据类型转换<sup><a href="#Top">Top</a></sup></h3>

函数 | 描述
:---|:---
int(x[,base]) | 将x转换为一个整数
long(x[,base]) | 将x转换为一个长整数
float(x) | 将x转换到一个浮点数
complex(real[,imag]) | 创建一个复数
str(x) | 将对象 x 转换为字符串
repr(x) | 将对象 x 转换为表达式字符串
eval(str) | 用来计算在字符串中的有效Python表达式,并返回一个对象
tuple(s) | 将序列 s 转换为一个元组
list(s) | 将序列 s 转换为一个列表
set(s) | 转换为可变集合
dict(d) | 创建一个字典。d 必须是一个序列 (key,value)元组。
frozenset(s) | 转换为不可变集合
chr(x) | 将一个整数转换为字符
unichr(x) | 将一个整数转换为Unicode字符
ord(x) | 将一个字符转换为它的整数值
hex(x) | 将一个整数转换为一个十六进制字符串
oct(x) | 将一个整数转换为一个八进制字符串

