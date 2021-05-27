---
title: 删除本地化的组织BrandingProperties
description: 删除 organizationalBrandingProperties 以用于特定本地化。
localization_priority: Normal
author: AlexanderMars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 38cd43af8e91ee0399000ec856856a86fb482ea9
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680813"
---
# <a name="delete-localized-organizationalbrandingproperties"></a>删除本地化的组织BrandingProperties

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

删除 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Organization.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{tenant id}/branding/localizations/{locale}
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_organizationalbrandingproperties_2"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-organizationalbrandingproperties-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-organizationalbrandingproperties-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-organizationalbrandingproperties-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-organizationalbrandingproperties-2-java-snippets.md)]
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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
