---
title: 创建表
description: 使用此 API 创建新的表。
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 7502d0b394d100b029f98d3b1217b4b107078f8a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036807"
---
# <a name="create-table"></a>创建表

命名空间：microsoft.graph

使用此 API 创建新的表。
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
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:---------------|:----------|
| Authorization  | 持有者{令牌}。必需。 |
| Workbook-Session-Id  | 确定是否保留更改的工作簿会话 ID。可选。|

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数           | 类型      |说明|
|:---------------|:----------|:----------|
| Address  | string| 区域地址。若要从 `worksheets/{id or name}/tables/add` 路径调用此 API，地址中无需有工作表名称前缀。不过，若要从 `workbook/tables/add` 路径调用此 API，请提供需要在其中创建表的工作表名称（例如：`sheet1!A1:D4`）|
| hasHeaders  | 布尔|指示区域是否具有列标签的布尔值。如果源不包含标头（即，当此属性设置为 false 时），Excel 将自动生成标头，数据将向下移动一行。|

## <a name="response"></a>响应

如果成功，此方法在 `201 Created` 响应正文中返回 响应代码和 [WorkbookTable](../resources/table.md) 对象。

## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "create_table_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id}/add
Content-type: application/json
Content-length: 109

{
  "address": "A1:D8",
  "hasHeaders": false
}
```
##### <a name="response"></a>响应
这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

