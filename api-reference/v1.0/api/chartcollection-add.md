---
title: 'ChartCollection: add'
description: 创建新图表。
author: lumine2008
ms.openlocfilehash: bfae5968c6a1131cb58bda80bd2587a68047bed9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332954"
---
# <a name="chartcollection-add"></a>ChartCollection: add

创建新图表。
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
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a>请求标头
| Name       | 说明|
|:---------------|:----------|
| Authorization  | Bearer {token}。必需。 |
| Workbook-Session-Id  | 确定是否保留更改的工作簿会话 ID。可选。|

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | Type   |说明|
|:---------------|:--------|:----------|
|type|string|代表图表的类型。  可能的值为： `ColumnClustered`， `ColumnStacked`， `ColumnStacked100`， `BarClustered`， `BarStacked`， `BarStacked100`， `LineStacked`， `LineStacked100`， `LineMarkers`， `LineMarkersStacked`， `LineMarkersStacked100`， `PieOfPie`， `etc.`。|
|sourceData|Json|对应于源数据的 Range 对象。|
|seriesBy|string|可选。 指定的方式列或行用作图表上的数据系列。  可能的值为： `Auto`， `Columns`， `Rows`。|

## <a name="response"></a>响应

如果成功，此方法返回`200 OK`响应代码和[WorkbookChart](../resources/chart.md)响应正文中的对象。

## <a name="example"></a>示例
下面是一个如何调用此 API 的示例。
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "chartcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add
Content-type: application/json
Content-length: 94

{
  "type": "ColumnStacked",
  "sourceData": "A1:B1",
  "seriesBy": "Auto"
}
```

##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
