---
title: group： validateProperties
description: 验证用户Microsoft 365或邮件昵显示名称是否符合命名策略。
ms.localizationpriority: medium
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4cc1aa6a36a0e270313c1654814149ee3e8d5ce4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61015069"
---
# <a name="group-validateproperties"></a>group： validateProperties

命名空间：microsoft.graph

验证用户Microsoft 365或邮件昵显示名称是否符合命名策略。 客户端可以使用 API 确定显示名称或邮件昵称是否有效，然后再尝试更新Microsoft 365组。  若要在创建组之前验证属性，请对目录 [对象使用 validateProperties](directoryobject-validateproperties.md) 函数。

对邮件和邮件昵称显示名称执行以下验证： 
1. 验证前缀和后缀命名策略
2. 验证自定义禁止字策略

此 API 返回遇到的第一个故障。 如果一个或多个属性未能通过多次验证，则仅返回第一个验证失败的属性。 但是，如果您仅验证前缀和后缀命名策略，您可以验证邮件昵称和显示名称并接收验证错误集合。

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
POST /groups/{id}/validateProperties
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
|displayName|String| 要显示名称组的成员。 属性不单独是必需的。 但是，至少需要一 (displayName 或 mailNickname) 属性。 |
|mailNickname|String| 要验证的组的邮件昵称。 属性不单独是必需的。 但是，至少需要一 (displayName 或 mailNickname) 属性。 |
|onBehalfOfUserId|Guid| 调用 API 时要模拟的用户的对象 ID。 验证结果适用于 onBehalfOfUserId 的属性和角色。 |

## <a name="response"></a>响应
如果成功且没有验证错误，该方法将返回 `204 No Content` 响应代码。 它不会在响应正文中返回任何内容。

如果请求无效，该方法将返回 `400 Bad Request` 响应代码。 响应正文中返回一条错误消息，包含有关无效请求的详细信息。

如果存在验证错误。 方法返回 `422 Unprocessable Entity` 响应代码。 响应正文中返回错误消息和错误详细信息集合。

## <a name="examples"></a>示例

这是成功验证请求的一个示例。

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json

{
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/group-validateproperties-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

这是一个出现验证错误的请求示例。

### <a name="request"></a>请求
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

### <a name="response"></a>响应
```http
HTTP/1.1 422
Content-type: application/json

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
  ]
}-->


