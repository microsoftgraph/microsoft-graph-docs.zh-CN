---
title: 创建 tableRow
description: 将行添加到表的末尾。
ms.localizationpriority: medium
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b5299e8db954f1c8e103059115cbb6a7679f2c66
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507545"
---
# <a name="create-tablerow"></a>创建 tableRow

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将行添加到表的末尾。 

请注意，API 可以使用此 API 接受多行数据。 一次添加一行可能会导致性能下降。 建议的方法是在单个调用中一起批处理行，而不是执行单行插入。 为了获得最佳结果，请收集应用程序端要插入的行并执行单行添加操作。 试验行数，以确定在单个 API 调用中的理想行数。 

此请求有时可能会导致 `504 HTTP` 错误。 此错误的适当响应做法是重复发出请求。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Files.ReadWrite    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/rows
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/rows
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/rows
POST /me/drive/root:/{item-path}:/workbookworksheets/{id|name}/tables/{id|name}/rows
```

## <a name="request-headers"></a>请求标头

| 名称 | 说明 |
|:---------------|:----------|
| Authorization  | Bearer {token}。必需。 |
| Content-Type | application/json. Required.|
| Prefer  | respond-async。 指示请求是异步请求。 可选。  |
| Workbook-Session-Id  | {Workbook-Session-Id}。 根据 **createSession 请求** 创建。 可选。|

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

|参数|类型|Description|
|:---------------|:--------|:----------|
| index| Int32| 可选。指定新行的相对位置。如果为空，将在末尾进行添加。插入的行下方的任何行将向下移动。从零开始编制索引。|
| 值| [Json](../resources/json.md)| 表格行的无格式值的二维数组。|

## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [workbookTableRow](../resources/workbooktablerow.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-add-two-rows-to-a-table"></a>示例 1：向表中添加两行

本示例中，在表格末尾插入两行数据。 

#### <a name="request"></a>请求

下面是一个请求示例。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ", "Table1"],
  "name": "tablerowcollection_add_1"
}-->

```http
POST https://graph.microsoft.com/beta/me/drive/items/01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ/workbook/tables/Table1/rows
Content-type: application/json
Content-length: 90

{
  "values": "[
    [1, 2, 3],
    [4, 5, 6]
  ]"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerowcollection-add-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablerowcollection-add-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablerowcollection-add-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablerowcollection-add-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应

下面是一个响应示例。 

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "[[1, 2, 3]]"
}
```

### <a name="example-2-add-two-rows-to-a-table-asynchronously"></a>示例 2：异步向表中添加两行

如果请求所花的时间超过预期，异步请求将非常有用。 请注意， `Workbook-Session-Id` 发出异步请求时需要 标头。 用户需要在使用 [异步富](./workbook-createsession.md) API 功能之前创建会话。 在 `Prefer:respond-async` 异步请求中，标头也是必需的。

对于异步功能，用户通常需要发出 2-3 个请求。 此请求 [Get workbookOperation](./workbookoperation-get.md) 请求和（可选） [获取 tableRowOperationResult](./workbook-tablerowoperationresult.md) 请求。

#### <a name="request"></a>请求

下面是异步请求的示例。 请注意 `202 Accepted` ，仅在请求需要很长时间才能响应时发生。 如果请求快速完成，它将像常规同步请求一样工作，回滚到 [示例 1](#example-1-add-two-rows-to-a-table)。


<!-- {
  "blockType": "request",
  "sampleKeys": ["01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ", "Table1"],
  "name": "tablerowcollection_add_1"
}-->

```http
POST https://graph.microsoft.com/beta/me/drive/items/01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ/workbook/tables/Table1/rows
Content-type: application/json
Prefer: respond-async
Workbook-Session-Id: {Workbook-Session-Id}
Content-length: 51

{
  "values": "[
    [1, 2, 3],
    [4, 5, 6]
  ]"
}
```

#### <a name="response"></a>响应

下面是另一个将导致异步操作的响应示例。 有关详细信息，请参阅获取 [workbookOperation 和](./workbookoperation-get.md) [Get tableRowOperationResult](./workbook-tablerowoperationresult.md)。
<!-- {
  "blockType": "response",
  "truncated": true,
  "sampleKeys": ["01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ", "0195cfac-bd22-4f91-b276-dece0aa2378b", "Y2x1c3Rlcj1QU0c0JnNlc3Npb249MTUuU0cyUEVQRjAwMDI4RjI1MS5BMTE2LjEuVTM2LmM4MGRiNjkwLTQwMTktNGNkNS1hYWJiLTJmYzczM2YxZTQ5ZjE0LjUuZW4tVVM1LmVuLVVTMjQuMTAwM2JmZmRhYzUyMzkzOS1Qcml2YXRlMS5TMjQuJTJmUEI0JTJmWjJqZmt1aXhJZHBjeE8xYmclM2QlM2QxNi4xNi4wLjE0NDEwLjM1MDUwMTQuNS5lbi1VUzUuZW4tVVMxLk0xLk4wLjEuUyZ1c2lkPWExOTMyNTU0LTlhNDAtNzYzNi1mNDU3LWEyNjExMmFkNDg2YQ=="],
  "@odata.type": "microsoft.graph.Json"
} -->

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/me/drive/items/01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ/workbook/operations/0195cfac-bd22-4f91-b276-dece0aa2378b?sessionId=Y2x1c3Rlcj1QU0c0JnNlc3Npb249MTUuU0cyUEVQRjAwMDI4RjI1MS5BMTE2LjEuVTM2LmM4MGRiNjkwLTQwMTktNGNkNS1hYWJiLTJmYzczM2YxZTQ5ZjE0LjUuZW4tVVM1LmVuLVVTMjQuMTAwM2JmZmRhYzUyMzkzOS1Qcml2YXRlMS5TMjQuJTJmUEI0JTJmWjJqZmt1aXhJZHBjeE8xYmclM2QlM2QxNi4xNi4wLjE0NDEwLjM1MDUwMTQuNS5lbi1VUzUuZW4tVVMxLk0xLk4wLjEuUyZ1c2lkPWExOTMyNTU0LTlhNDAtNzYzNi1mNDU3LWEyNjExMmFkNDg2YQ==
Content-type: application/json
Content-length: 45

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
