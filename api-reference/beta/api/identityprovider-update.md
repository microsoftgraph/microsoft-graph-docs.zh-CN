---
title: 更新 identityProvider
description: 更新现有 Identityprovider.read.all 中的属性。
localization_priority: Normal
ms.openlocfilehash: 8d51307d65ae3ae957b42f31117322d3f5bc5602
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441798"
---
# <a name="update-identityprovider"></a>更新 identityProvider

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新现有 [identityProvider](../resources/identityprovider.md) 中的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）|IdentityProvider.ReadWrite.All|
|委派（Microsoft 个人帐户）| 不支持。|
|应用程序|不支持。|

工作或学校帐户必须是租户的全局管理员。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---------------|:----------|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，为 JSON 对象提供一个或多个需要更新的属性。

|属性|类型|说明|
|:---------------|:--------|:----------|
|clientId|字符串|应用程序的客户端 ID。 这是向标识提供程序注册应用程序时获取的客户端 ID。|
|clientSecret|字符串|应用程序的客户端密码。 这是向标识提供程序注册应用程序时获取的客户端密码。|
|name|字符串|标识提供程序的显示名称。|

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。 如果失败，将返回 `4xx` 错误并显示具体详细信息。

## <a name="example"></a>示例

以下示例会更新令牌生命周期 **identityProvider** 的定义并将其设置为组织默认值。

##### <a name="request"></a>请求


# <a name="httptabhttp"></a>[HTTP.SYS](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_identityprovider"
}-->
```http
PATCH https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
Content-type: application/json
Content-length: 41

{
    "clientSecret": "1111111111111"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目标-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identityprovider-objc-snippets.md)]
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
  "description": "Update identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
