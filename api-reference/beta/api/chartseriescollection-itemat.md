---
title: 'ChartSeriesCollection: ItemAt'
description: 根据其在集合中的位置检索系列
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d59b4e3e01b123728a3659b77d6e1a859e19f434
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60925613"
---
# <a name="chartseriescollection-itemat"></a>ChartSeriesCollection: ItemAt

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

根据其在集合中的位置检索系列
## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Files.ReadWrite    |
|委派（个人 Microsoft 帐户） | Files.ReadWrite    |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/ItemAt
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/series/ItemAt

```
## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:---------------|:----------|
| Authorization  | Bearer {token}。必需。 |
| Workbook-Session-Id  | 确定是否保留更改的工作簿会话 ID。可选。|

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型   |Description|
|:---------------|:--------|:----------|
|index|number|要检索的对象的索引值。从零开始编制索引。|

## <a name="response"></a>响应

如果成功，此方法在 `200 OK` 响应正文中返回 响应代码和 [workbookChartSeries](../resources/workbookchartseries.md) 对象。

## <a name="example"></a>示例
下面是一个如何调用此 API 的示例。
##### <a name="request"></a>请求
下面是一个请求示例。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartseriescollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/ItemAt
Content-type: application/json

{
  "index": {
  }
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartseriescollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>响应
这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartSeriesCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


