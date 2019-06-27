---
title: 删除用户 - Microsoft Graph API
description: 介绍删除 Microsoft Graph API (REST) 的用户资源（实体）的方法。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4ee725065269313e2b596305888d157edecdcc5f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270376"
---
# <a name="delete-a-user"></a>删除用户

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

删除用户。  

删除时，将用户资源转移到存储时限为 30 日的临时容器中。  此后，它们将被永久删除。  要了解详细信息，请参阅 [deletedItems](../resources/directory.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | User.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | User.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a>请求标头

| 标头       | 值|
|:-----------|:------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/ba9a3254-9f18-4209-aeb3-9e42a35b5be4 
```
### <a name="response"></a>响应

下面是一个响应示例。 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a>SDK 示例代码
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[目标-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
