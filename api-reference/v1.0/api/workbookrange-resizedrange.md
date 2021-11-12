---
title: 'workbookRange: resizedRange'
description: 获取与当前范围对象类似的范围对象，但其右下角可通过一定数量的行和列进行展开（或合拢）。
ms.localizationpriority: medium
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 4e64ae05c5dec6cd9750e23e6c86d20178229fc0
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60940139"
---
# <a name="workbookrange-resizedrange"></a>workbookRange: resizedRange

命名空间：microsoft.graph 获取与当前 range 对象类似的 range 对象，但其右下角展开 (或按) 行和列数缩小。

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
POST /me/drive/items/{id}/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```

## <a name="function-parameters"></a>函数参数

| 参数    | 类型   |Description|
|:---------------|:--------|:----------|
|deltaRows|Int32|相对于当前范围，右下角展开的行数。使用正数可展开范围，使用负数可合拢范围|
|deltaColumns|Int32|相对于当前范围，右下角展开的列数。 使用正数可展开范围，使用负数可合拢范围。|

## <a name="request-headers"></a>请求头
| 名称       | 说明|
|:---------------|:----------|
| Authorization  | Bearer {token}。必需。 |
| Workbook-Session-Id  | 确定是否保留更改的工作簿会话 ID。可选。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

### <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/range.md) 对象。

## <a name="example"></a>示例
下面是一个如何调用此 API 的示例。
##### <a name="request"></a>请求
下面是一个请求示例。
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_resizedrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})
```

##### <a name="response"></a>响应
这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookRange: resizedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

