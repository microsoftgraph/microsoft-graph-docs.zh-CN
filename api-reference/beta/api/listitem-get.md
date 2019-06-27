---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 从 SharePoint 列表中获取条目
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1cb6a51434aba70964321bc99e72603911af3b7b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266176"
---
# <a name="get-an-item-in-a-list"></a>获取列表中的项

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

返回[列表][]中某个[项][]的元数据。

[列表]: ../resources/list.md
[项]: ../resources/listitem.md

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.Read.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Sites.Read.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a>示例

##### <a name="request"></a>请求

<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a>响应

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "d14922d8-43e6-4c8a-b029-e35c5b4e0d63",
  "listItemId": 2,
  "fields": {
    "Name": "Widget",
    "Color": "Blue",
    "Quantity": 2357
    }
}
```
#### <a name="sdk-sample-code"></a>SDK 示例代码
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-item-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[目标-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-list-item-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
    "Error: /api-reference/beta/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
