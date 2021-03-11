---
title: user： revokeSignInSessions
description: 将 **signInSessionsValidFromDateTime** 用户属性重置为当前日期时间，使颁发给应用程序 (的所有用户刷新令牌以及用户浏览器) 中的会话 cookie 失效。
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 53d194ac1058652c06e673beca1fdd6aeb876719
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719729"
---
# <a name="user-revokesigninsessions"></a>user： revokeSignInSessions

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将 **signInSessionsValidFromDateTime** 用户属性重置为当前日期时间，使颁发给用户 (应用程序的所有刷新令牌以及用户浏览器) 中的会话 cookie 失效。 通常，如果用户的设备丢失 (，则由用户或) 管理员执行此操作。 此操作通过要求用户重新登录到之前同意的所有应用程序（独立于设备）来阻止通过设备上的应用程序访问组织数据。

如果应用程序尝试使用无效的刷新令牌为此用户兑换委派访问令牌，则应用程序将出现错误。 如果发生这种情况，应用程序将需要通过向授权终结点提出请求来获取新的刷新令牌，这将强制用户登录。

>[!NOTE]
>调用 **revokeSignInSessions** 后，在吊销令牌之前可能有几分钟的一小延迟。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | User.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /me/revokeSignInSessions
POST /users/{id | userPrincipalName}/revokeSignInSessions
```

## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>请求正文
此操作没有请求内容。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

>[!NOTE]
>此 API 存在一个[已知问题](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code)。 它返回不同的 HTTP 响应代码。

## <a name="example"></a>示例
以下示例演示如何调用此 API。

##### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_revokesigninsessionss"
}-->
```http
POST https://graph.microsoft.com/beta/me/revokeSignInSessions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-revokesigninsessionss-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-revokesigninsessionss-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-revokesigninsessionss-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-revokesigninsessionss-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: revokeSignInSessions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


