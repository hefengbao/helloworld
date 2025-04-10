# JSON

[JSON-RPC 2.0 Specification (jsonrpc.org)](https://www.jsonrpc.org/specification)

[Google JSON Style Guide](https://google.github.io/styleguide/jsoncstyleguide.xml?showone=error#error)

## JSON基本概念

```
释义:
    JSON是存储和传递数据的语法,它采用键值对(下文解释)的方式来编写。
优点:
    易于人们的阅读和编写,同时也易于机器的解析和生成。
特点:
    只要按照JSON的规则,不管什么语言都可以使用JSON的形式,来存储数据。
```

## JSON语法规则

```
实例:
    json = {
        "sex":"男",
        "age":80
    }
释义:
    "sex":"男"
       "sex" : 便是名称,也就是键
       "男"  : 值
格式

    名称/值对的组合中,名称写在前面(且都需要用在双引号中),中间用冒号隔开。

    若在一个json对象中,有多个键值对那么每个键值对之间用逗号隔开。

调用
    json对象名.名称

    json.sex 便可获取到该键值对的值,“男”
```

```
SON值类型

    数字(整数或浮点数) : 无需双引号
    字符串            : 在引号中
    逻辑值            : true 或 false 无需双引号
    数组              : []  无需双引号
    对象              : {}  无需双引号
    null              : 空值 无需双引号
```

```
实例
    jsonone = {
        "staff":[
                {"name":"小王","age":70},
                {"name":"赵五","age":80}
            ]
    }

    创建的jsonone对象中有一个键值对,该键值对的值是一个数组,
        数组里面有两个json对象.

    可以都过如下调用获取小王的年龄
    jsonone.staff[0].age
```
