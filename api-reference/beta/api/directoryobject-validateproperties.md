---
title: directoryObject： validateProperties
description: 验证 Microsoft 365 组的显示名称或邮件昵称是否符合命名策略。
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 39bd3f2aeeb87ff82fca521173b78f2be6a9b215
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854562"
---
# <a name="directoryobject-validateproperties"></a>directoryObject： validateProperties

命名空间：microsoft.graph

验证 Microsoft 365 组的显示名称或邮件昵称是否符合命名策略。  客户端可以使用此 API 确定显示名称或邮件昵称是否有效，然后再尝试创建Microsoft 365组。 若要验证现有组的属性，请对组 [使用 validateProperties](group-validateproperties.md) 函数。

对邮件和邮件昵称显示名称执行以下验证： 
1. 验证前缀和后缀命名策略
2. 验证自定义禁止字策略
3. 验证邮件昵称是否唯一

此 API 返回遇到的第一个故障。 如果一个或多个属性未能通过多次验证，则仅返回第一个验证失败的属性。 但是，如果您仅验证前缀和后缀命名策略，您可以验证邮件昵称和显示名称并接收验证错误集合。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a>请求标头

| 名称           | 说明      |
|:---------------|:-----------------|
| Authorization  | Bearer {code}。 必需。   |
| Content-Type   | application/json. Required. |

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型   |说明|
|:---------------|:--------|:----------|
|entityType|String| `Group` 是唯一受支持的实体类型。 |
|displayName|String| 要显示名称组的成员。 属性不单独是必需的。 但是，至少需要一 (displayName 或 mailNickname) 属性。 |
|mailNickname|String| 要验证的组的邮件昵称。 属性不单独是必需的。 但是，至少需要一 (displayName 或 mailNickname) 属性。 |
|onBehalfOfUserId|GUID| 调用 API 时要模拟的用户的对象 ID。 验证结果适用于 onBehalfOfUserId 的属性和角色。 |

## <a name="response"></a>响应

如果成功且没有验证错误，该方法将返回 `204 No Content` 响应代码。 它不会在响应正文中返回任何内容。

如果请求无效，该方法将返回 `400 Bad Request` 响应代码。 响应正文中返回一条错误消息，包含有关无效请求的详细信息。

如果存在验证错误，该方法将返回响应 `422 Unprocessable Entity` 代码。 响应正文中返回错误消息和错误详细信息集合。

## <a name="examples"></a>示例

这是成功验证请求的一个示例。

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/beta/directoryObjects/validateProperties
Content-type: application/json

{
  "entityType": "Group",
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/directoryobject-validateproperties-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/directoryobject-validateproperties-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

这是一个出现验证错误的请求示例。

### <a name="request"></a>请求
```http
POST https://graph.microsoft.com/beta/directoryObjects/validateProperties
Content-type: application/json

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
  ]
}-->


