---
title: "Python基础语法"
date: 2020-06-27 17:32:23 +0800
category: Python
tags: [Basics]
excerpt: 本文主要介绍Python的基础语法
---


 > - [1.Python标识符](#Identifier)
 > - [2.Python保留字符](#Keyword)
 > - [3.行和缩进](#Indent)
 > - [4.Python引号](#Marks)
 > - [5.Python注释](#Notes)
 > - [6.等待用户输入](#Enter)
 > - [7.import与from...import](#Import)
 > - [8.变量赋值](#Assignment)

<h3 id="Identifier">1. Python标识符:<sup><a href="#Top">Top</a></sup></h3>

 > - 由字母、数字、下划线组成;
 > - 不能以数字开头;
 > - 单下划线开头`_foo`表示不能直接访问的类属性,需要通过类提供接口进行访问,不能用`from xxx import *`而导入;
 > - 双下划线开头的`__foo`代表类的私有成员;
 >  - 双下划线开头和结尾的`__foo__`代表Python里的特殊方法专用标识,如`__init__()`代表构造函数;
 > - 同一行显示多条语句用`;`分开.  

<h3 id="Keyword">2. Python保留字符:<sup><a href="#Top">Top</a></sup></h3>

	import keyword
	keyword.kwlist
输出:

	['False', 'None', 'True', 'and', 'as', 'assert', 'break', 'class', 'continue', 'def', 'del', 'elif', 'else',
	'except', 'finally', 'for', 'from', 'global', 'if', 'import', 'in', 'is', 'lambda', 'nonlocal', 'not', 'or',
	'pass', 'raise', 'return', 'try', 'while', 'with', 'yield']

<h3 id="Indent">3. 行和缩进<sup><a href="#Top">Top</a></sup></h3>


 > Python语句中一般以新行作为语句的结束符。但是我们可以使用斜杠（ \）将一行的语句分为多行显示

    total = item_one + \
    item_two + \
    item_three
 > 语句中包含 [], {} 或 () 括号就不需要使用多行连接符

    days = ['Monday', 'Tuesday', 'Wednesday',
            'Thursday', 'Friday']
<h3 id="Marks">4. Python引号<sup><a href="#Top">Top</a></sup></h3>

 > Python 可以使用引号( ' )、双引号( " )、三引号( ''' 或 """ ) 来表示字符串，引号的开始与结束必须的相同类型的。其中三引号可以由多行组成，编写多行文本的快捷语法，常用于文档字符串，在文件的特定地点，被当做注释。

    word = 'word'
    sentence = "这是一个句子。"
    paragraph = """这是一个段落。
    包含了多个语句"""

<h3 id="Notes">5. Python注释<sup><a href="#Top">Top</a></sup></h3>

 > - python中单行注释用#开头;
 > - python 中多行注释使用三个单引号(''')或三个双引号(""").

<h3 id="Enter">6. 等待用户输入<sup><a href="#Top">Top</a></sup></h3>

    input("按下 enter 键退出，其他任意键显示...\n")
<h3 id="Import">7. import与from...import<sup><a href="#Top">Top</a></sup></h3>
 > - python用`import`或者`from...import`来导入模块
 > - 整个模块导入`import somemodule`
 > - 从某个模块中导入某个函数`from somemodule import somefunction`
 > - 从某个模块中导入多个函数`from somemodule import firstfunc,secondfunc`
 > - 将某个模块中的全部函数导入`from somemodule import *`

<h3 id="Assignment">8. 变量赋值<sup><a href="#Top">Top</a></sup></h3>
 > - Python中的变量赋值不需要类型声明;
 > - 每个变量在内存中创建,都包括变量的标识,名称和数据这些信息;
 > - 每个变量在使用前都必须赋值,变量赋值以后改变量才会被创建;
 > - 等号(=)来给变量赋值.

    counter = 100 # 赋值整型变量
    miles = 1000.0 # 浮点型
    name = "John" # 字符串
    
    print(counter)
    print(miles)
    print(name)
 > - 多个变量赋值:

 ```
a = b = c = 1
 ```
 > - 多个对象指定多个变量:

 ```
a, b, c = 1, 2, "gool"
 ```