---
title: 'TableRowCollection: add'
description: '向表末尾的行。 请注意 API 可以接受使用此 API 的多个行数据。 一次添加一个行可能导致性能下降。 建议的方法是批处理一起中单个呼叫，而不是以单个行插入行。 为了获得最佳结果，收集要插入的应用程序一侧，并执行单个行的行添加操作。 试验要确定的理想要使用一个 API 调用中的行数的行数。 '
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: f51e7b9ff52c728a7ac2446d538b939d8d5be57a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912559"
---
# <a name="tablerowcollection-add"></a>TableRowCollection: add

向表末尾的行。 请注意 API 可以接受使用此 API 的多个行数据。 一次添加一个行可能导致性能下降。 建议的方法是批处理一起中单个呼叫，而不是以单个行插入行。 为了获得最佳结果，收集要插入的应用程序一侧，并执行单个行的行添加操作。 试验要确定的理想要使用一个 API 调用中的行数的行数。 

## <a name="error-handling"></a>错误处理

此请求有时可能会收到 504 HTTP 错误。 此错误的适当响应做法是重复发出请求。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Files.ReadWrite    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:---------------|:----------|
| Authorization  | Bearer {token}。必需。 |
| Workbook-Session-Id  | 确定是否保留更改的工作簿会话 ID。可选。|

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型   |说明|
|:---------------|:--------|:----------|
|index|Int32|可选。指定新行的相对位置。如果为空，将在末尾进行添加。插入的行下方的任何行将向下移动。从零开始编制索引。|
|values|Json|可选。未设置格式的表行值的二维数组。|

## <a name="response"></a>响应

如果成功，此方法返回`200 OK`响应代码和[WorkbookTableRow](../resources/tablerow.md)响应正文中的对象。

## <a name="example"></a>示例
在此示例中的表的末尾插入两行数据。 

##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "index": 5,
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```

##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/api/tablerowcollection-add.md/tablerowcollection_add/values:
      Inconsistent types between parameter (Collection) and table (None)",
    "Error: /api-reference/v1.0/api/tablerowcollection-add.md/tablerowcollection_add/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Collection)) is a collection, while the table description type (microsoft.graph.Json) is not."
  ],
  "tocPath": ""
}-->
