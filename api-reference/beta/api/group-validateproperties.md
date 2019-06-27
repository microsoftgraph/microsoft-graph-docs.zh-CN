---
title: '组: validateProperties'
description: 验证 Office 365 组的显示名称或邮件昵称是否符合命名策略。 在尝试**更新**Office 365 组之前, 客户端可以使用 API 来确定显示名称或邮件昵称是否有效。 若要在创建组之前验证属性, 请使用目录对象的 validateProperties 函数。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: ecf5be372cb00df26bf6ae14fdba933782040bc6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262802"
---
# <a name="group-validateproperties"></a>组: validateProperties

验证 Office 365 组的显示名称或邮件昵称是否符合命名策略。 在尝试**更新**Office 365 组之前, 客户端可以使用 API 来确定显示名称或邮件昵称是否有效。 若要在创建组之前验证属性, 请使用目录对象的[validateProperties 函数](directoryobject-validateproperties.md)。

将为显示名称和邮件昵称属性执行以下验证: 
1. 验证前缀和后缀命名策略
2. 验证 "自定义禁止的词语" 策略

此 API 在遇到第一次失败时返回。 如果一个或多个属性失败多次验证, 则仅返回第一个验证失败的属性。 但是, 如果仅验证前缀和后缀命名策略, 则可以验证邮件别名和显示名称, 并接收验证错误的集合。

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
| Authorization  | Bearer {code}    |
| Content-Type   | application/json |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型   |说明|
|:---------------|:--------|:----------|
|displayName|String| 要验证的组的显示名称。 属性不是单独需要的。 但是, 至少需要一个属性 (displayName 或 mailNickname)。 |
|mailNickname|String| 要验证的组的邮件别名。 属性不是单独需要的。 但是, 至少需要一个属性 (displayName 或 mailNickname)。 |
|onBehalfOfUserId|Guid| 调用 API 时要模拟的用户的对象 ID。 验证结果针对的是 onBehalfOfUserId 的属性和角色。 |

## <a name="response"></a>响应
如果成功且没有验证错误, 则该方法返回`204 No Content`响应代码。 它不在响应正文中返回任何内容。

如果请求无效, 该方法将返回`400 Bad Request`响应代码。 有关无效请求的详细信息的错误消息将在响应正文中返回。

如果存在验证错误。 此方法返回`422 Unprocessable Entity`响应代码。 响应正文中返回一条错误消息和一组错误详细信息。

## <a name="examples"></a>示例

这是一个成功的验证请求的示例。

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
#### <a name="sdk-sample-code"></a>SDK 示例代码
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/group_validateproperties-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_validateproperties-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[目标-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/group_validateproperties-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

这是包含验证错误的请求的示例。

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
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-validateproperties.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-validateproperties.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-validateproperties.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
