---
title: 更新 personAnniversary
description: 更新 personAnniversary 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 571a298bec352362f0796b953b00a6df010b1ce0
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228743"
---
# <a name="update-personanniversary"></a>更新 personAnniversary

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新用户的[配置文件](../resources/profile.md)中的[personAnniversary](../resources/personanniversary.md)对象的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | 所有用户读写。          |
| 委派（个人 Microsoft 帐户） | 所有用户读写。          |
| 应用程序                            | User.ReadWrite.All                          |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/anniversaries/{id} 
```

## <a name="request-headers"></a>请求标头

| 名称           |说明                  |
|:---------------|:----------------------------|
| Authorization  | Bearer {token}。必需。   |
| Content-Type   | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性     | 类型        | 说明                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|date          |Date         | 包含与周年纪念类型相关联的日期。          |
|类型          |string       | 可取值为：`birthday`、`wedding`、`unknownFutureValue`。|

## <a name="response"></a>响应

如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[personAnniversary](../resources/personanniversary.md)对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personanniversary"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/anniversaries/{id}
Content-type: application/json

{
  "type": "type-value",
  "date": "datetime-value"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personanniversary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personanniversary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personanniversary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAnniversary"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "type": "type-value",
  "date": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update personanniversary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
