---
title: 工作簿资源类型
description: 包含相关的工作簿对象，如工作表、表、区域等。
ms.localizationpriority: medium
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ac8454ea02a81151be85267cb70e7909cb47e83d
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2022
ms.locfileid: "62291055"
---
# <a name="workbook-resource-type"></a>工作簿资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含相关的工作簿对象，如工作表、表、区域等。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[创建会话](../api/workbook-createsession.md) | [workbookSessionInfo](workbooksessioninfo.md) |创建工作簿会话以启动永久或非永久会话。|
|[关闭会话](../api/workbook-closesession.md) | 无 |关闭现有会话。|
|[刷新会话](../api/workbook-refreshsession.md) | 无 |刷新现有会话。|

## <a name="properties"></a>属性
无。

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|names|[workbookNamedItem](workbooknameditem.md) 集合 |表示工作簿范围内的已命名项目（称为区域和常量）的集合。只读。|
|表格|[workbookTable](workbooktable.md) 集合 |表示与工作簿关联的表的集合。只读。|
|Worksheets|[workbookWorksheet](workbookworksheet.md) 集合 |表示与工作簿关联的工作表的集合。只读。|
|workbbookApplication|[workbookApplication](workbookapplication.md) |表示Excel工作簿的 workbookApplication 对象。|
|operations|[workbookOperation](workbookoperation.md) 集合|工作簿操作的状态。 不支持获取操作集合，但如果响应中返回 `Location` 标头，可以获取长时间运行操作的状态。 只读。 可为 NULL。|

## <a name="functions"></a>函数

[Excel 函数](#functions)使用 JSON 对象调用使用语法 `POST /me/drive/root/workbook/functions/{function-name}` 并在正文中提供函数自变量的工作簿函数。该函数产生 `value`，所有 `error` 字符串均返回到函数结果对象中。`null` 的 `error` 值表示该函数执行成功。 

受支持函数的完整列表在 [此处](https://support.office.com/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188)。请参阅特定参数名称和数据类型的函数签名。

_重要说明_： 
* 使用 range 对象（而不是范围地址字符串）提供范围输入参数。  
* 与大部分 API 中使用的从 0 开始编制的索引不同，索引参数是从 1 开始编制索引。 

示例：**vlookup**

在 Excel 电子表格中，`vlookup` 函数需要使用以下参数：

1. 要查找的值（亦称为“查阅值”）。
2. 查阅值所在的区域。 请注意，查阅值应始终位于区域中的第一列，这样 VLOOKUP 才能正常运行。 例如，如果查阅值位于单元格 C2，那么区域应从 C 列开始。
3. 区域中包含返回值的列号。例如，如果指定 B2: D11 作为区域，那么应该将 B 算作第一列，C 作为第二列，以此类推。
4. （可选）如果想要近似匹配，可指定 TRUE；如果想要返回值的完全匹配，则可指定 FALSE。
 如果未指定，默认值始终为 TRUE 或近似匹配。

在单元格中，`vlookup` 函数如下所示： 

=VLOOKUP(查阅值, 包含查阅值的区域, 包含返回值的区域的列号, 视需要为近似匹配指定 TRUE 或为完全匹配指定 FALSE)

（请参阅 [VLOOKUP Excel 函数](https://support.office.com/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1)文档。）

下面的示例展示了如何使用 Excel REST API 调用 `vlookup`  函数，以及一个或多个输入区域。
请求： 

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

响应：

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

下面的示例展示了如何调用 `median` 函数，以及如何使用 Excel REST API 传递一个或多个输入区域。 

请求： 

```http 
POST https://graph.microsoft.com/beta/me/drive/root:/book1.xlsx:/workbook/functions/median
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
   "values":[
      {
         "address":"Sheet2!A1:A5"
      },
      {
         "address":"Sheet2!B1:B5"
      }
   ]
}
```

响应：

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
## <a name="json-representation"></a>JSON 表示形式

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.workbook"
}-->
``` json
{
    "id": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Workbook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


