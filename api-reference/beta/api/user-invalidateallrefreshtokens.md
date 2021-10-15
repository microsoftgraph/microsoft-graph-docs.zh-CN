---
title: user：invalidateAllRefreshTokens
description: 使颁发给用户浏览器中的应用程序和会话 Cookie 的用户刷新令牌失效。
ms.localizationpriority: medium
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 36d012a2299e4a84d62769661d3662a69e171bfe
ms.sourcegitcommit: c3f849e5a052b1926373a4b316ec303250e6d09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/15/2021
ms.locfileid: "60369767"
---
# <a name="user-invalidateallrefreshtokens"></a>user：invalidateAllRefreshTokens

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将 **refreshTokensValidFromDateTime** 用户属性重置为当前日期时间，使颁发给应用程序 (的所有用户刷新令牌以及用户浏览器) 中的会话 cookie 失效。 通常，如果用户的设备丢失 (，则由用户或管理员) 用户或管理员执行此操作。  此操作将阻止访问通过设备上的应用程序访问的任何组织数据，而无需首先要求用户重新登录。 事实上，此操作将强制用户重新登录之前已同意的所有应用程序，而与设备无关。

对于开发人员，如果应用程序尝试使用无效的刷新令牌为该用户兑换委派访问令牌，则应用程序将发生错误。 如果发生这种情况，应用程序将需要通过向授权终结点提出请求来获取新的刷新令牌，这将强制用户登录。


## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | User.ReadWrite、Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /me/invalidateAllRefreshTokens
POST /users/{id | userPrincipalName}/invalidateAllRefreshTokens
```
## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文
此操作没有请求内容。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

>[!NOTE]
>此 API 返回不同的 HTTP 响应代码，类似于 [revokeSignInSessions](user-revokesigninsessions.md) 操作。 有关详细信息，请参阅 [已知问题](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code)。 

## <a name="example"></a>示例

### <a name="request"></a>请求
下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-invalidateallrefreshtokens-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-invalidateallrefreshtokens-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-invalidateallrefreshtokens-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-invalidateallrefreshtokens-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
下面展示了示例响应。 
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
  "description": "user: invalidateAllRefreshTokens",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


