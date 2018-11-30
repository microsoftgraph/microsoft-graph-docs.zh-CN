---
title: 'directoryObject: validateProperties'
description: 验证如果 Office 365 组的显示名称或邮件昵称符合命名策略。  客户端可以使用 API 以确定是否显示名称或邮件昵称有效，然后尝试**创建**到 Office 365 组。 用于验证的现有组属性，使用组 validateProperties 函数。
ms.openlocfilehash: 82592eff14829fdd8ae1d74c87f43402a3938adf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042922"
---
# <a name="directoryobject-validateproperties"></a>directoryObject: validateProperties

验证如果 Office 365 组的显示名称或邮件昵称符合命名策略。  客户端可以使用 API 以确定是否显示名称或邮件昵称有效，然后尝试**创建**到 Office 365 组。 用于验证的现有组属性，使用组[validateProperties 函数](group-validateproperties.md)。

显示名称和邮件昵称属性执行以下验证： 
1. 验证前缀和后缀命名策略
2. 验证自定义禁止的单词策略
3. 验证邮件昵称是唯一

此 API 返回与第一个遇到故障。 如果一个或多个属性失败多个验证，则返回仅与第一个验证失败的属性。 但是，您可以验证邮件昵称和显示名称和接收验证错误的集合，如果您仅验证前缀和后缀命名策略。

## <a name="prerequisites"></a>先决条件

执行此 API 所需的以下**权限**： *Group.Read.All*

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a>请求标头

| 名称           | 说明      |
|:---------------|:-----------------|
| Authorization  | 持有者 {code}    |
| Content-Type   | application/json |

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型   |说明|
|:---------------|:--------|:----------|
|entityType|字符串| `Group`是唯一受支持的实体类型。 |
|displayName|字符串| 要验证的组的显示名称。 该属性不是单独必需的。 但是，至少一个属性 （displayName 或 mailNickname） 是必需的。 |
|mailNickname|字符串| 要验证的组邮件昵称。 该属性不是单独必需的。 但是，至少一个属性 （displayName 或 mailNickname） 是必需的。 |
|onBehalfOfUserId|Guid| 调用 API 时模拟用户对象 ID。 验证结果是针对 onBehalfOfUserId 的属性和角色。 |

## <a name="response"></a>响应

如果成功，并有没有验证错误，该方法返回`204 No Content`响应代码。 它不返回任何响应正文中。

如果请求无效，则该方法返回`400 Bad Request`响应代码。 响应正文中返回有关无效请求的详细错误消息。

如果验证错误，则该方法返回`422 Unprocessable Entity`响应代码。 在响应正文中将返回一条错误消息和错误详细信息的集合。

## <a name="examples"></a>示例

这是一个成功验证请求示例。

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "directoryobject_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

这是一个带有验证错误的请求示例。

### <a name="request"></a>请求
```http
POST https://graph.microsoft.com/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "test",
  "mailNickname": "test",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a>响应
```http
HTTP/1.1 422 
Content-Type: application/json

{
  "error": {
    "code": "Request_UnprocessableEntity",
    "message": "The values provided contain one or more validation errors.",
    "innerError": {
      "request-id": "request-id-value",
      "date": "date-value"
    },
    "details": [
      {
        "target": "displayName",
        "code": "MissingPrefixSuffix",
        "message": "Property mailNickname is missing a required prefix/suffix per your organization's Group naming requirements.",
        "prefix": "Myprefix_",
        "suffix": "_mysuffix"
      },
      {
        "target": "mailNickname",
        "code": "MissingPrefixSuffix",
        "message": "Property mailNickname is missing a required prefix/suffix per your organization's Group naming requirements.",
        "prefix": "Myprefix_",
        "suffix": "_mysuffix"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: validateProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
