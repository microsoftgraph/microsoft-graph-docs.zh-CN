---
title: 组： validateProperties
description: 验证 Microsoft 365 组的显示名称或邮件昵称是否符合命名策略。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: acdc168df631a0db5eff277348cf4b0e43d85357
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897104"
---
# <a name="group-validateproperties"></a>组： validateProperties

命名空间：microsoft.graph

验证 Microsoft 365 组的显示名称或邮件昵称是否符合命名策略。  在尝试[更新](group-update.md)Microsoft 365 组之前，客户端可以使用此 API 来确定显示名称或邮件昵称是否有效。 若要在创建组之前验证属性，请使用[directoryobject： validateProperties](directoryobject-validateproperties.md)函数。

将为显示名称和邮件昵称属性执行以下策略验证：
1. 验证前缀和后缀命名策略
2. 验证 "自定义禁止的词语" 策略

此 API 仅返回遇到的第一个验证失败。 如果属性失败多次验证，则仅返回第一个验证失败。 但是，如果仅验证前缀和后缀命名策略，则可以验证邮件别名和显示名称，并接收验证错误的集合。 若要了解有关配置命名策略的详细信息，请参阅[Configure 命名策略](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell)。

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
| Authorization  | Bearer {token}。必需。    |
| Content-Type   | application/json |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型   |说明|
|:---------------|:--------|:----------|
|displayName|String| 要验证的组的显示名称。 属性不是单独需要的。 但是，至少需要一个属性（**displayName**或**mailNickname**）。 |
|mailNickname|String| 要验证的组的邮件别名。 属性不是单独需要的。 但是，至少需要一个属性（**displayName**或**mailNickname**）。 |
|onBehalfOfUserId|Guid| 调用 API 时要模拟的用户的 ID。 验证结果针对的是**onBehalfOfUserId 的**属性和角色。 |

## <a name="response"></a>响应
如果成功且没有验证错误，则该方法返回 `204 No Content` 响应代码。 它不在响应正文中返回任何内容。

如果请求无效，该方法将返回 `400 Bad Request` 响应代码。 有关无效请求的详细信息的错误消息将在响应正文中返回。

如果存在验证错误。 此方法返回 `422 Unprocessable Entity` 响应代码。 响应正文中返回一条错误消息和一组错误详细信息。

## <a name="examples"></a>示例

### <a name="example-1-successful-validation-request"></a>示例1：成功的验证请求
这是一个成功的验证请求的示例。

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/v1.0/groups/{id}/validateProperties
Content-type: application/json
Content-length: 132

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

---


#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-validation-errors"></a>示例2：包含验证错误的请求
这是包含验证错误的请求的示例。

#### <a name="request"></a>请求
``` http
POST https://graph.microsoft.com/v1.0/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

#### <a name="response"></a>响应
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
  ]
}-->
