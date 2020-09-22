---
title: archivedPrintJob 资源类型
description: "\"最终状态\" (\"已完成\"、\"已中止\" 或 \"失败\" 的记录) 用于报告目的的打印作业。 这不是活动的打印作业。"
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: d4bd76dc84ad41c6d412144d13a784bec4f6a9f7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050127"
---
# <a name="archivedprintjob-resource-type"></a>archivedPrintJob 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

"最终状态" ("已完成"、"已中止" 或 "失败" 的记录) 用于报告目的的打印作业。 这不是活动的打印作业。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|存档的打印作业的 GUID。 只读。|
|printerId|String|作业排队等待的打印机 ID。 只读。|
|processingState|printJobProcessingState|打印作业的最终处理状态。 只读。|
|createdDateTime|DateTimeOffset|创建作业时的 dateTimeOffset。 只读。|
|acquiredDateTime|DateTimeOffset|打印机获取作业时的 dateTimeOffset （如果有）。 只读。|
|completionDateTime|DateTimeOffset|作业完成、取消或终止时的 dateTimeOffset。 只读。|
|acquiredByPrinter|Boolean|如果作业是由打印机获取的，则为 True; 否则为否则为 false。 只读。|
|copiesPrinted|Int32|打印的份数。 只读。|
|pageCount|Int32|打印的总页数。 只读。|
|blackAndWhitePageCount|Int32|打印的黑白页面数。 只读。|
|colorPageCount|Int32|打印的彩色页面的数量。 只读。|
|simplexPageCount|Int32|打印的单 (单面) 页的数量。 只读。|
|duplexPageCount|Int32|打印的双面打印 (双面) 页的数量。 只读。|
|createdBy|[userIdentity](useridentity.md)|创建打印作业的用户。 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.archivedPrintJob"
}-->

```json
{
    "id": "String (identifier)",
    "printer": {"@odata.type": "microsoft.graph.directoryObject"},
    "createdBy": {"@odata.type": "microsoft.graph.userIdentity"},
    "processingState": {"@odata.type": "microsoft.graph.printJobProcessingState"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "archivedPrintJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

