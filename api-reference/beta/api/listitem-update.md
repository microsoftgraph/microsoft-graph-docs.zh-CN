---
author: JeremyKelley
description: 更新 listItem 上的属性。
ms.date: 09/11/2017
title: 更新 SharePoint 列表中的记录
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: c46206a77359a6a60aaa4193f1d5ff7395a597d7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942388"
---
# <a name="update-an-item-in-a-list"></a>更新列表中的项

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 **[listItem][]** 上的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a>可选的请求标头

| 名称       | 值 | 说明
|:-----------|:------|:--------------------------------------------------------
| _if-match_ | etag  | 如果包含此请求标头，且提供的 eTag 与项中的当前 eTag 不匹配，则返回 `412 Precondition Failed` 响应，并且不会更新该项。


## <a name="request-body"></a>请求正文

在请求正文中，提供指定要更新的字段的 [fieldValueSet][] 的 JSON 表示形式。

## <a name="example"></a>示例

下面是一个示例，使用新值更新列表项的“颜色”和“数量”字段。
listItem 上的所有其他值都保持独立。 


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "create-listitem-2", "scopes": "sites.readwrite.all" } -->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-listitem-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-listitem-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-listitem-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a>响应

如果成功，此方法在已更新列表项的响应正文中返回 [fieldValueSet][]。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "Name": "Widget",
  "Color": "Fuchsia",
  "Quantity": 934
}
```

[fieldValueSet]: ../resources/fieldvalueset.md
[listItem]: ../resources/listitem.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update",
  "suppressions": [
  ]
}
-->


