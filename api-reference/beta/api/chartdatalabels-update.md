---
title: 更新 workbookChartDataLabels
description: 更新 workbookchartdatalabels 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 054e26a9653d35b403aa3ff1cc38487830b7a067
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317198"
---
# <a name="update-workbookchartdatalabels"></a>更新 workbookChartDataLabels

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 chartdatalabels 对象的属性。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Files.ReadWrite    |
|委派（个人 Microsoft 帐户） | Files.ReadWrite    |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/datalabels
```
## <a name="optional-request-headers"></a>可选的请求标头
| 名称       | 说明|
|:-----------|:-----------|
| Authorization  | Bearer {token}。必需。 |
| Workbook-Session-Id  | 确定是否保留更改的工作簿会话 ID。可选。|

## <a name="request-body"></a>请求正文
在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|position|字符串|表示数据标签位置的 DataLabelPosition 值。可能的值是：`None`、`Center`、`InsideEnd`、`InsideBase`、`OutsideEnd`、`Left`、`Right`、`Top`、`Bottom`、`BestFit`、`Callout`。|
|separator|string|表示用于图表中数据标签的分隔符的字符串。|
|showBubbleSize|boolean|表示数据标签气泡大小是否可见的布尔值。|
|showCategoryName|boolean|表示数据标签类别名称是否可见的布尔值。|
|showLegendKey|boolean|表示数据标签图例标示是否可见的布尔值。|
|showPercentage|boolean|表示数据标签百分比是否可见的布尔值。|
|showSeriesName|boolean|表示数据标签系列名称是否可见的布尔值。|
|showValue|布尔|表示数据标签值是否可见的布尔值。|

## <a name="response"></a>响应

如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[workbookChartDataLabels](../resources/workbookchartdatalabels.md)对象。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。

# <a name="httptabhttp"></a>[HTTP.SYS](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartdatalabels"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/datalabels
Content-type: application/json
Content-length: 134

{
  "position": "position-value",
  "showValue": true,
  "showSeriesName": true,
  "showCategoryName": true,
  "showLegendKey": true
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartdatalabels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartdatalabels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目标-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartdatalabels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartdatalabels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "position": "position-value",
  "showValue": true,
  "showSeriesName": true,
  "showCategoryName": true,
  "showLegendKey": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartdatalabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
