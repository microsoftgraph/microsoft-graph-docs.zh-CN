---
title: printUsageSummaryByPrinter 资源类型
description: 描述在指定时间段 (usageDate) 时打印机的打印活动。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 4d33ab99780f980dcc24e267ba1ac6603f602aa2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070646"
---
# <a name="printusagesummarybyprinter-resource-type"></a>printUsageSummaryByPrinter 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述在指定时间段 (usageDate) 时打印机的打印活动。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 (每日) ](../api/reportroot-list-dailyprintusagesummariesbyprinter.md) | [printUsageSummaryByPrinter](printusagesummarybyprinter.md) | 获取按打印机分组的每日打印使用率摘要列表。 |
| [每月 () 列表 ](../api/reportroot-list-monthlyprintusagesummariesbyprinter.md) | [printUsageSummaryByPrinter](printusagesummarybyprinter.md) | 获取按打印机分组的按月打印使用情况摘要列表。 |
| [Get](../api/printusagesummarybyprinter-get.md) | [printUsageSummaryByPrinter](printusagesummarybyprinter.md) | 读取 **printUsageSummaryByPrinter** 对象的属性和关系。 |

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|此使用率摘要的 ID。|
|printerID|String|由这些统计信息表示的打印机的 ID。|
|usageDate|日期|与这些统计信息关联的日期。|
|completedBlackAndWhiteJobCount|Int64|打印机在关联日期完成的黑色和白色打印作业的数量。|
|completedColorJobCount|Int64|打印机在关联日期完成的彩色打印作业数。|
|incompleteJobCount|Int64|在关联的日期上排队等候打印机但尚未完成的打印作业的数量。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUsageSummaryByPrinter"
}-->

```json
{
    "id": "String (identifier)",
    "printerId": "String (identifier)",
    "usageDate": "String (timestamp)",
    "completedBlackAndWhiteJobCount": 123456,
    "completedColorJobCount": 123456,
    "incompleteJobCount": 123456
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printUsageSummaryByPrinter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

