# Smock
---
Smock 是一款基于nodeJs的简单mock工具🔧

## 1. Init

初始化如下，然后去config目录下编写合适你的index.json

```bash
npm i 
```

## 2. How to use？

超简单的配置，只需以json数组的方式写你想返回的接口的值，以及接口调用的方法，参考如下：

```javascript
[{
   "url": "/test",
   "data": [
       {"name": "@r12312"},
       {"name": 2},
       {"name": "@r"},
       {"name": [
           {"test":1},
           {"test":2},
           {"test":"@r"}
       ]}
   ]
}]
```
如此就完成了一个接口的定义，访问地址是ip+端口/test，返回的值是data里面的内容