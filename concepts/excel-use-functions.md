---
title: 通过 Microsoft Graph 使用 Excel 工作簿函数
description: 可以使用以下语法调用任何工作簿函数：`POST /me/drive/root/workbook/functions/{function-name}`。 使用 JSON 对象提供正文中的函数参数。 该函数产生 `value`，所有 `error` 字符串均返回到函数结果对象中。 `null` 的 `error` 值表示该函数执行成功。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 6ba9c94f78325fe855ec6f0c4b2a0dcff8de559a
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491038"
---
# <a name="use-workbook-functions-in-excel-with-microsoft-graph"></a>通过 Microsoft Graph 使用 Excel 工作簿函数

可以使用以下语法调用任何工作簿函数：`POST /me/drive/root/workbook/functions/{function-name}`。 使用 JSON 对象提供正文中的函数参数。 该函数产生 `value`，所有 `error` 字符串均返回到函数结果对象中。 `null` 的 `error` 值表示该函数执行成功。

有关受支持的函数的完整列表，请参阅 [Excel.Functions 类](/javascript/api/excel/excel.functions?view=excel-js-preview)。 请参阅特定参数名称和数据类型的函数签名。

_重要说明_：
* 使用 range 对象（而不是范围地址字符串）提供范围输入参数。  
* 与大部分 API 中使用的从 0 开始编制的索引不同，索引参数是从 1 开始编制索引。

示例：**vlookup**

在 Excel 电子表格中，`vlookup` 函数需要使用以下参数：

1. lookup_value（必需）要查找的值。
2. table_array **table_array**（必需）查阅值所在的单元格的区域。 请注意，查阅值应始终位于区域中的第一列，这样 VLOOKUP 才能正常运行。 例如，如果查阅值位于单元格 C2，那么区域应从 C 列开始。
3. col_index_num（必需）包含返回值的区域的列号。 例如，如果指定 B2: D11 作为区域，应将 B 计为第一列，将 C 计为第二列，依此类推。
4. range_lookup（可选）一个逻辑值，指定希望 VLOOKUP 查找近似匹配还是精确的匹配。 如果想要近似匹配，可指定 TRUE；如果想要返回值的完全匹配，则可指定 FALSE。 如果未指定，默认值始终为 TRUE 或近似匹配。

在单元格中，`vlookup` 函数如下所示：

=VLOOKUP(查阅值, 包含查阅值的区域, 包含返回值的区域的列号, 视需要为近似匹配指定 TRUE 或为完全匹配指定 FALSE)

（请参阅 [VLOOKUP Excel 函数](https://support.office.com/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1)文档。）


##### <a name="request"></a>请求:
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

##### <a name="response"></a>响应

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

示例：`median`

在 Excel 电子表格中，`median` 函数需要使用一个或多个输入区域。

在单元格中，`median` 函数如以下示例所示：

=MEDIAN(A2:A6)

（请参阅 [MEDIAN Excel 函数](https://support.office.com/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2)文档。）

##### <a name="request"></a>请求
以下示例演示如何使用 Excel REST API 调用 函数和一 `median` 个或多个输入区域。

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

##### <a name="response"></a>响应

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
* [使用 Excel REST API](/graph/api/resources/excel?view=graph-rest-1.0)
