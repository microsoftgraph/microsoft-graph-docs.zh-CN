---
title: 组： validateProperties
description: 验证如果 Office 365 组的显示名称或邮件昵称符合命名策略。 客户端可以使用 API 以确定是否显示名称或邮件昵称有效，然后尝试**更新**到 Office 365 组。 用于创建组之前验证属性，将 validateProperties 函数用于目录对象。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5361e05d2a58e2d4c27bd662f158d4f185c447fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990886"
---
# <a name="group-validateproperties"></a>组： validateProperties

验证如果 Office 365 组的显示名称或邮件昵称符合命名策略。 客户端可以使用 API 以确定是否显示名称或邮件昵称有效，然后尝试**更新**到 Office 365 组。 用于创建组之前验证属性，将[validateProperties 函数](directoryobject-validateproperties.md)用于目录对象。

显示名称和邮件昵称属性执行以下验证： 
1. 验证前缀和后缀命名策略
2. 验证自定义禁止的单词策略

此 API 返回与第一个遇到故障。 如果一个或多个属性失败多个验证，则返回仅与第一个验证失败的属性。 但是，您可以验证邮件昵称和显示名称和接收验证错误的集合，如果您仅验证前缀和后缀命名策略。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Group.Read.All、Group.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Group.Read.All、Group.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/<id>/validateProperties
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
|displayName|字符串| 要验证的组的显示名称。 该属性不是单独必需的。 但是，至少一个属性 （displayName 或 mailNickname） 是必需的。 |
|mailNickname|字符串| 要验证的组邮件昵称。 该属性不是单独必需的。 但是，至少一个属性 （displayName 或 mailNickname） 是必需的。 |
|onBehalfOfUserId|Guid| 调用 API 时模拟用户对象 ID。 验证结果是针对 onBehalfOfUserId 的属性和角色。 |

## <a name="response"></a>响应
如果成功，并有没有验证错误，该方法返回`204 No Content`响应代码。 它不返回任何响应正文中。

如果请求无效，则该方法返回`400 Bad Request`响应代码。 响应正文中返回有关无效请求的详细错误消息。

如果没有验证错误。 该方法返回`422 Unprocessable Entity`响应代码。 在响应正文中将返回一条错误消息和错误详细信息的集合。

## <a name="examples"></a>示例

这是一个成功验证请求示例。

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "group_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 132

{
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

这是一个带有验证错误的请求示例。

### <a name="request"></a>请求
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

### <a name="response"></a>响应
```http
HTTP/1.1 422
Content-type: application/json
Content-length: 223

{
  "error": {
    "code": "Request_UnprocessableEntity",
    "message": "The values provided contain one or more validation errors.",
    "innerError": {
      "request-id": "id-value",
      "date": "date-value"
    },
    "details": [
      {
        "target": "mailNickname",
        "code": "PropertyConflict",
        "message": "Another object with the same value for property mailNickname already exists."
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: validateProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
