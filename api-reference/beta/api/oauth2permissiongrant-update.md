---
title: 更新 oAuth2PermissionGrant
description: 更新 oAuth2PermissionGrant 的属性，该属性代表委派权限授予。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 1d9aff9e74168c5077350def5fcd230e5e75bbd8
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383649"
---
# <a name="update-a-delegated-permission-grant-oauth2permissiongrant"></a>更新委派权限授予（oAuth2PermissionGrant）

命名空间：microsoft.graph

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)对象的属性，该对象代表委派权限授予。

可以通过在**范围**的列表中添加或删除项目来更新**oAuth2PermissionGrant** ，以更改要授予的委派权限。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | DelegatedPermissionGrant、Directory.accessasuser.all、all 和的所有子目录    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|Application | Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /oauth2PermissionGrants/{id}
```

## <a name="request-headers"></a>请求标头

| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。

| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|scope|String| 指定在 OAuth 2.0 访问令牌中，资源应用程序应预期的范围声明的值。 |

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_oAuth2PermissionGrant"
}-->

```http
PATCH https://graph.microsoft.com/beta/oauth2PermissionGrants/{id}
Content-Type: application/json
Content-Length: 30

{
  "scope": "scope-value"
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-oauth2permissiongrant-objc-snippets.md)]
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update oAuth2PermissionGrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
