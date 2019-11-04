---
title: 更新 itemphone
description: 更新 itemphone 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 16c50b41e0c8a5993433b98bf394d22379ae04bb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938076"
---
# <a name="update-itemphonenumber"></a>更新 itemphonenumber

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新用户的[配置文件](../resources/profile.md)中的[itemPhone](../resources/itemphone.md)对象的属性。

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
PATCH /me/profile/phones/{id} 
```

## <a name="request-headers"></a>请求标头

| 名称           |说明                  |
|:---------------|:----------------------------|
| Authorization  | Bearer {token}。必需。   |
| Content-Type   | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性     | 类型        | 描述                                                                                                                     |
|:-------------|:------------|:--------------------------------------------------------------------------------------------------------------------------------|
|displayName   |字符串       | 包含电话号码的友好名称。                                                                                  |
|number        |字符串       | 包含电话号码。                                                                                                      |
|类型          |字符串       | 可取值为：`home`、`business`、`mobile`、`other`、`assistant`、`homeFax`、`businessFax`、`otherFax`、`pager`、`radio`。|

## <a name="response"></a>响应

如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[itemPhone](../resources/itemphone.md)对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "update_itemphone"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/phones/{id}
Content-type: application/json

{
  "displayName": "displayName-value",
  "type": "type-value",
  "number": "number-value"
}
```

### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPhone"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "type": "type-value",
  "number": "number-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update itemphone",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->