---
title: 用户： invalidateAllRefreshTokens
description: 使所有用户的刷新令牌颁发给应用程序 （以及用户的浏览器中的会话 cookie） 到当前日期时间重置**refreshTokensValidFromDateTime**用户属性失效。 通常情况下，执行此操作 （按用户或管理员） 如果用户具有丢失或被盗的设备。  此操作将阻止对任何用户首先需要再次登录的情况下访问通过设备上的应用程序的组织的数据访问。 实际上，此操作会强制用户再次登录的所有应用程序的这些以前同意，独立于设备。
localization_priority: Normal
ms.openlocfilehash: 4ece9866e703d47ab8f7b024496f92f30a4a14b8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858077"
---
# <a name="user-invalidateallrefreshtokens"></a>用户： invalidateAllRefreshTokens

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

使所有用户的刷新令牌颁发给应用程序 （以及用户的浏览器中的会话 cookie） 到当前日期时间重置**refreshTokensValidFromDateTime**用户属性失效。 通常情况下，执行此操作 （按用户或管理员） 如果用户具有丢失或被盗的设备。  此操作将阻止对任何用户首先需要再次登录的情况下访问通过设备上的应用程序的组织的数据访问。 实际上，此操作会强制用户再次登录的所有应用程序的这些以前同意，独立于设备。

面向开发人员，如果应用程序尝试使用无效的刷新令牌，兑换为此用户的委派的访问令牌的应用程序将收到错误。 如果发生这种情况，应用程序需要获取新刷新令牌的授权终结点，则会强制用户登录向发出请求。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

+ 应用程序，以便在用户以使应用程序无效签名他们已同意： User.ReadWrite，Directory.ReadWrite.All，Directory.AccessAsUser.All
+ 要允许管理员使失效应用程序的应用程序的用户已同意： Directory.ReadWrite.All、 Directory.AccessAsUser.All

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
此操作不包含任何请求内容。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="example"></a>示例
下面是一个如何调用此 API 的示例。
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```

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
<!-- {
  "type": "#page.annotation",
  "description": "user: invalidateAllRefreshTokens",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
