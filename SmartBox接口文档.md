---
title: SmartBox接口文档
language_tabs:
  - java: Java
toc_footers: []
includes: []
search: true
code_clipboard: true
highlight_theme: darkula
headingLevel: 2
generator: "@tarslib/widdershins v4.0.23"

---

# 善格智能挂牌服务

Base URLs:

* <a href="http://{host:port}/dev-api/jobplan">测试环境: http://{host:port}/dev-api/jobplan</a>

# Authentication

# BoxController

## GET 查询智能Box详细信息

GET /box/{id}

查询智能Box详细信息

### 请求参数

|名称|类型|必选|说明|
|---|---|---|---|
|id|string| 是 |id|

> 返回示例

```json
{
  "msg": "操作成功",
  "code": 200,
  "data": {
    "powerStatus": 0,
    "lockStatus": 0,
    "id": 1
  }
}
```

### 返回结果

|状态码|状态码含义|说明|数据模型|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### 返回数据结构

状态码 **200**

*操作消息提醒*

|名称|类型|中文名|说明|
|---|---|---|---|
|» msg|string||none|
|» code|integer||none|
|» data|object||none|
|»» powerStatus|integer|断电状态|0为断电状态  1为通电状态|
|»» lockStatus|integer|上锁状态|0为断电状态  1为通电状态|
|»» id|integer|Box的ID|none|

