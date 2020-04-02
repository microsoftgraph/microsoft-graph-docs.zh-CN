---
title: 用户： invalidateAllRefreshTokens
description: 使用户的浏览器中颁发给应用程序和会话 cookie 的用户的所有刷新令牌失效。
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 37b6ecb26a6141ff3ac9d49c67f2911e6c84c749
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107785"
---
# <a name="user-invalidateallrefreshtokens"></a>用户： invalidateAllRefreshTokens

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过将**refreshTokensValidFromDateTime**用户属性重置为当前的日期时间来使向应用程序颁发的所有用户刷新令牌失效（以及用户浏览器中的会话 cookie）。 通常，如果用户有丢失或被盗的设备，则执行此操作（由用户或管理员执行）。  此操作将阻止访问通过设备上的应用程序访问的任何组织数据，而用户首次无需再次登录。 实际上，此操作会强制用户再次登录到他们之前同意的所有应用程序，而不依赖于设备。

对于开发人员，如果应用程序尝试使用无效刷新令牌兑换此用户的委派访问令牌，应用程序将收到错误。 如果发生这种情况，应用程序将需要通过向授权终结点发出请求来获取新的刷新令牌，这将强制用户登录。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

+ 对于允许已登录用户使已登录的应用程序无效的应用程序，请执行以下操作： User. ReadWrite、Directory.accessasuser.all
+ 对于允许管理员使用户同意的应用程序无效的应用程序，请执行以下操作： Directory.accessasuser.all

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

## <a name="example"></a>示例
下面是一个如何调用此 API 的示例。
##### <a name="request"></a>请求
下面是一个请求示例。

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

---


##### <a name="response"></a>响应
下面是一个响应示例。 
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
