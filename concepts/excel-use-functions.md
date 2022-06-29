---
title: 在 Excel 中使用工作簿函数
description: 可以将 Excel 中的工作簿函数与 Microsoft Graph 配合使用，以调用任何工作簿函数。 包括 vlookup 和中值函数的示例。
ms.localizationpriority: medium
author: lumine2008
ms.prod: excel
ms.openlocfilehash: eec1834a63ab87304b33eea1f75629fe12e56aec
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66443366"
---
# <a name="use-workbook-functions-in-excel"></a>在 Excel 中使用工作簿函数

可以将 Excel 中的工作簿函数与 Microsoft Graph 配合使用，以使用以下语法调用任何工作簿函数： `POST /me/drive/root/workbook/functions/{function-name}` 使用 JSON 对象在正文中提供函数参数。 该函数产生 `value`，所有 `error` 字符串均返回到函数结果对象中。 `null` 的 `error` 值表示该函数执行成功。

有关支持的函数的完整列表，请参阅 [Excel.Functions 类](/javascript/api/excel/excel.functions?view=excel-js-preview&preserve-view=true)。 请参阅特定参数名称和数据类型的函数签名。

> [!IMPORTANT]
> - 使用 range 对象（而不是范围地址字符串）提供范围输入参数。  
> - 与大部分 API 中使用的从 0 开始编制的索引不同，索引参数是从 1 开始编制索引。

## <a name="example-vlookup"></a>例如：`vlookup`

在 Excel 电子表格中，`vlookup` 函数需要使用以下参数：

- **lookup_value** (所需的) ：要查找的值。

- **table_array** (所需的) ：查找值所在的单元格区域。 请记住，查找值应始终位于 **VLOOKUP** 范围内的第一列中，以便正常工作。 例如，如果查阅值位于单元格 C2 中，则范围应从 C 开始。

- **col_index_num** (所需的) ：包含返回值的范围内的列号。 例如，如果指定 B2: D11 作为区域，应将 B 计为第一列，将 C 计为第二列，依此类推。

- **range_lookup** (可选) ：指定是要 **VLOOKUP** 查找近似值还是精确匹配项的逻辑值。 如果想要近似匹配，可指定 TRUE；如果想要返回值的完全匹配，则可指定 FALSE。 如果未指定任何内容，默认值将始终为 TRUE 或近似匹配。

在单元格中，`vlookup` 函数如下所示：

`=VLOOKUP` (查阅值、包含查阅值的范围、包含返回值的区域中的列号（可选）为近似匹配指定 TRUE，或者为精确匹配的 FALSE 指定 FALSE) 

有关详细信息，请参阅 [VLOOKUP Excel 函数](https://support.office.com/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1)的文档。

### <a name="request"></a>请求

下面的示例展示了如何使用 Excel REST API 调用 `vlookup` 函数和传递这些参数。

```http
POST https://graph.microsoft.com/beta/me/drive/root:/book1.xlsx:/workbook/functions/vlookup
content-type: Application/Json
authorization: Bearer {access-token}
workbook-session-id: {session-id}

{
    "lookupValue": "Temperature",
    "tableArray": { "Address": "Sheet1!E1:G5" },
    "colIndexNum": 2,
    "rangeLookup": false
}
```

### <a name="response"></a>响应

```http
HTTP code: 200 OK
content-type: application/json;odata.metadata

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#workbookFunctionResult",
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/workbook/functions/vlookup()",
    "error": null,
    "value": "28.3"
}
```

## <a name="example-median"></a>示例：`median`

在 Excel 电子表格中，`median` 函数需要使用一个或多个输入区域。

在单元格中，`median` 函数如以下示例所示：

`=MEDIAN(A2:A6)`

有关详细信息，请参阅 [MEDIAN Excel 函数](https://support.office.com/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2)的文档。

### <a name="request"></a>请求

以下示例演示如何使用 Excel REST API 调 `median` 用函数和一个或多个输入范围。

```http
POST https://graph.microsoft.com/beta/me/drive/root:/book1.xlsx:/workbook/functions/median
content-type: Application/Json
authorization: Bearer {access-token}
workbook-session-id: {session-id}

{
"values" :  [
        { "address": "Sheet2!A1:A5" },
        { "address": "Sheet2!B1:B5" },
      ]
}
```

### <a name="response"></a>响应

```http
HTTP code: 200 OK
content-type: application/json;odata.metadata

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#workbookFunctionResult",
  "@odata.type": "#microsoft.graph.workbookFunctionResult",
  "@odata.id": "/users('2abcad6a-2fca-4b6e-9577-e358a757d77d')/drive/root/workbook/functions/median()",
  "error": null,
  "value": 30
}
```

## <a name="see-also"></a>另请参阅

* [通过 Microsoft Graph 管理 Excel 会话](excel-manage-sessions.md)
* [使用 Microsoft Graph 编写 Excel 工作簿](excel-write-to-workbook.md)
* [通过 Microsoft Graph 更新 Excel 区域的格式](excel-update-range-format.md)
* [通过 Microsoft Graph 显示 Excel 图表图像](excel-display-chart-image.md)
* [使用 Excel REST API](/graph/api/resources/excel)
