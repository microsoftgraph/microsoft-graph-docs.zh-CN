---
title: printUsageSummaryByPrinter 资源类型
description: 描述指定时间段内打印机的打印活动 (usageDate) 。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 4d33ab99780f980dcc24e267ba1ac6603f602aa2
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753586"
---
# <a name="printusagesummarybyprinter-resource-type"></a>printUsageSummaryByPrinter 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述指定时间段内打印机的打印活动 (usageDate) 。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [列出 (每天) ](../api/reportroot-list-dailyprintusagesummariesbyprinter.md) | [printUsageSummaryByPrinter](printusagesummarybyprinter.md) | 获取按打印机分组的每日打印使用情况摘要列表。 |
| [列出 (月) ](../api/reportroot-list-monthlyprintusagesummariesbyprinter.md) | [printUsageSummaryByPrinter](printusagesummarybyprinter.md) | 获取按打印机分组的每月打印使用情况摘要列表。 |
| [获取](../api/printusagesummarybyprinter-get.md) | [printUsageSummaryByPrinter](printusagesummarybyprinter.md) | 读取 **printUsageSummaryByPrinter** 对象的属性和关系。 |

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|此使用率摘要的 ID。|
|printerID|String|这些统计信息表示的打印机 ID。|
|usageDate|日期|与这些统计信息关联的日期。|
|completedBlackAndWhiteJobCount|Int64|打印机在关联日期完成的黑白打印作业数。|
|completedColorJobCount|Int64|打印机在关联日期完成的颜色打印作业数。|
|incompleteJobCount|Int64|在关联日期中已排入打印机队列但未完成的打印作业数。|

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

