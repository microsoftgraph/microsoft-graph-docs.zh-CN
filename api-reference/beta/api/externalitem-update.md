---
title: 更新 externalitem
description: 更新 externalitem 的属性。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 05eef675ccb6b79e3919fae9a50e90b2d9a31326
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747195"
---
# <a name="update-externalitem"></a>更新 externalitem

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新[externalitem](../resources/externalitem.md)或[externalFile](../resources/externalfile.md)的属性。

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | 不支持。 |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | ExternalItem.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a>路径参数

| 参数     | 类型   | 说明                                         |
|:--------------|:-------|:----------------------------------------------------|
| connection-id | 字符串 | 包含`id` [externalConnection](../resources/externalconnection.md)的属性 |
| item-id       | 字符串 | 开发人员提供`id`的[externalItem](../resources/externalitem.md)或[externalFile](../resources/externalfile.md)属性。 |

## <a name="request-headers"></a>请求标头

| 名称          | 说明                 |
|:--------------|:----------------------------|
| Authorization | Bearer {token}。必需。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。 可更新以下属性。

> [!NOTE]
> 在预览过程中， `acl`可以通过修补程序来更新属性。 若要更新其他属性，请使用[PUT 将现有项改写为新项](externalconnection-put-items.md)。

### <a name="externalitem-properties"></a>externalItem 属性

| 属性 | 类型                                  | 说明               |
|:---------|:--------------------------------------|:--------------------------|
| acl      | [acl](../resources/acl.md)集合 | 一组访问控制项。 每个条目指定向用户或组授予的访问权限。 |

### <a name="externalfile-properties"></a>externalFile 属性

| 属性 | 类型                                  | 说明               |
|:---------|:--------------------------------------|:--------------------------|
| acl      | [acl](../resources/acl.md)集合 | 一组访问控制项。 每个条目指定向用户或组授予的访问权限。 |

## <a name="response"></a>响应

如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[externalItem](../resources/externalitem.md)或[externalFile](../resources/externalfile.md)对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_externalitem"
}-->

```http
PATCH https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
Content-type: application/json

{
  "acl": [
    {
      "type": "user",
      "value": "49103559-feac-4575-8b94-254814dfca72",
      "accessType": "grant",
      "identitySource": "Azure Active Directory"
    }
  ]
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-externalitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-externalitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a>响应
<!-- markdownlint-enable MD024 -->

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalItem"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "TSP228082938",
  "acl": [
    {
      "type": "user",
      "value": "49103559-feac-4575-8b94-254814dfca72",
      "accessType": "grant",
      "identitySource": "Azure Active Directory"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": "Textual content of the file"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update externalitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
