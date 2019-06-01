---
title: 'directoryObject: validateProperties'
description: 验证 Office 365 组的显示名称或邮件昵称是否符合命名策略。  在尝试**创建**Office 365 组之前, 客户端可以使用 API 来确定显示名称或邮件昵称是否有效。 若要验证现有组的属性, 请使用组的 validateProperties 函数。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4f672d4b6d2f33921f79d74d5213948dc630abda
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656039"
---
# <a name="directoryobject-validateproperties"></a>directoryObject: validateProperties

验证 Office 365 组的显示名称或邮件昵称是否符合命名策略。  在尝试**创建**Office 365 组之前, 客户端可以使用 API 来确定显示名称或邮件昵称是否有效。 若要验证现有组的属性, 请使用组的[validateProperties 函数](group-validateproperties.md)。

将为显示名称和邮件昵称属性执行以下验证: 
1. 验证前缀和后缀命名策略
2. 验证 "自定义禁止的词语" 策略
3. 验证邮件昵称是否唯一

此 API 在遇到第一次失败时返回。 如果一个或多个属性失败多次验证, 则仅返回第一个验证失败的属性。 但是, 如果仅验证前缀和后缀命名策略, 则可以验证邮件别名和显示名称, 并接收验证错误的集合。

## <a name="prerequisites"></a>先决条件

若要执行此 API, 需要以下**权限**: *Group. All*

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a>请求标头

| 名称           | 说明      |
|:---------------|:-----------------|
| Authorization  | Bearer {code}    |
| Content-Type   | application/json |

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型   |说明|
|:---------------|:--------|:----------|
|entityType|String| `Group`是唯一受支持的实体类型。 |
|displayName|String| 要验证的组的显示名称。 属性不是单独需要的。 但是, 至少需要一个属性 (displayName 或 mailNickname)。 |
|mailNickname|String| 要验证的组的邮件别名。 属性不是单独需要的。 但是, 至少需要一个属性 (displayName 或 mailNickname)。 |
|onBehalfOfUserId|Guid| 调用 API 时要模拟的用户的对象 ID。 验证结果针对的是 onBehalfOfUserId 的属性和角色。 |

## <a name="response"></a>响应

如果成功且没有验证错误, 则该方法返回`204 No Content`响应代码。 它不在响应正文中返回任何内容。

如果请求无效, 该方法将返回`400 Bad Request`响应代码。 有关无效请求的详细信息的错误消息将在响应正文中返回。

如果存在验证错误, 该方法将返回`422 Unprocessable Entity`响应代码。 响应正文中返回一条错误消息和一组错误详细信息。

## <a name="examples"></a>示例

这是一个成功的验证请求的示例。

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "directoryobject_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/beta/directoryObjects/validateProperties
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
#### <a name="sdk-sample-code"></a>SDK 示例代码
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/directoryobject_validateproperties-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/directoryobject_validateproperties-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

这是包含验证错误的请求的示例。

### <a name="request"></a>请求
```http
POST https://graph.microsoft.com/beta/directoryObjects/validateProperties
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
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryobject-validateproperties.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directoryobject-validateproperties.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
