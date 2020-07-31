---
title: "刻意练习"
date: 2020-06-30
category: Others
tags: [Read]
excerpt: 《刻意练习：如何从新手到大师》
---

## 有目的的练习的四个特点

1. 具有定义明确的特定目标
2. 专注
3. 包含反馈
4. 走出舒适区
   
惰性求值：返回值为stream
及早求值：返回值为另一个值或为空

collect(toList):有stream方法生成一个列表
map：将函数中的一种类型转换成另一种类型
filter：过滤掉不满足条件的元素
flatMap：将多个stream连接成一个stream
max、min：最大值最小值


请求报文方法：
GET:向特定的资源发出请求。
POST:向指定资源提交数据进行处理请求（例如提交表单或者上传文件）。
HEAD:向服务器索与GET请求相一致的响应，只不过响应体将不会被返回.
PUT:向指定资源位置上传其最新内容
DELETE:请求服务器删除Request-URL所标识的资源
CONNECT：HTTP/1.1协议中预留给能够将连接改为管道方式的代理服务器。
OPTIONS:返回服务器针对特定资源所支持的HTTP请求方法，也可以利用向web服务器发送‘*’的请求来测试服务器的功能性
TRACE:回显服务器收到的请求，主要用于测试或诊断

1XX:信息性状态码
2XX:成功状态码
3XX:重定向状态码
4XX:客户端错误状态码
5XX:服务端错误状态码

200 OK  当您的操作将在响应正文中返回数据时，出现此结果。
204 No Content 当您的操作成功，但不在响应正文中返回数据时，出现此结果。

304 Not Modified（重定向）  当测试实体自上次检索以来是否被修改时，出现此结果。

403 Forbidden   客户端错误
401 Unauthorized 客户端错误
413 Payload Too Large（客户端错误） 当请求长度过长时，出现此结果。
400 BadRequest（客户端错误） 当参数无效时，出现此结果。
404 Not Found（客户端错误） 当资源不存在时，出现此结果。
405 Method Not Allowed（客户端错误）由于方法和资源组合不正确而出现此错误。 例如，您不能对一个实体集合使用 DELETE 或 PATCH。
412 Precondition Failed  客户端错误

501 Not Implemented（服务器错误） 当未实施某个请求的操作时，出现此结果。
503 Service Unavailable（服务器错误） 当 Web API 服务不可用时，出现此结果。