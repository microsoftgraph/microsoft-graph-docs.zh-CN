---
title: 'ChartSeriesCollection: ItemAt'
description: 根据其在集合中的位置检索系列
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b96248f80fe01dd1910cb548330dc6951d4470db
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277544"
---
# <a name="chartseriescollection-itemat"></a>ChartSeriesCollection: ItemAt

根据其在集合中的位置检索系列
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
POST /workbook/worksheets/{id|name}/charts/{name}/series/itemAt

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
|index|Int32|要检索的对象的索引值。从零开始编制索引。|

## <a name="response"></a>响应

如果成功, 此方法在`200 OK`响应正文中返回响应代码和[WorkbookChartSeries](../resources/chartseries.md)对象。

## <a name="example"></a>示例
下面是一个如何调用此 API 的示例。
##### <a name="request"></a>请求
下面是一个请求示例。
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "chartseriescollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.chartseriescollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 2
}
```

##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
#### <a name="sdk-sample-code"></a>SDK 示例代码

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/chartseriescollection_itemat-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[目标-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/chartseriescollection_itemat-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeriesCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/chartseriescollection-itemat.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/chartseriescollection-itemat.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
