---
title: archivedPrintJob 资源类型
description: 用于报告目的 (已完成、中止或失败的) 打印作业的“最终状态”记录。 这不是活动打印作业。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 8ba8d49a01e3b10768e83b04b259d6cfd87d65b5
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944974"
---
# <a name="archivedprintjob-resource-type"></a>archivedPrintJob 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于报告目的 (已完成、中止或失败的) 打印作业的“最终状态”记录。 这不是活动打印作业。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|存档的打印作业的 GUID。 只读。|
|printerId|String|作业排队的打印机 ID。 只读。|
|processingState|printJobProcessingState|打印作业的最终处理状态。 只读。|
|createdDateTime|DateTimeOffset|创建作业时的 dateTimeOffset。 只读。|
|acquiredDateTime|DateTimeOffset|打印机获取作业时的 dateTimeOffset（如果有）。 只读。|
|completionDateTime|DateTimeOffset|作业完成、取消或中止时的 dateTimeOffset。 只读。|
|acquiredByPrinter|布尔值|如此 如果作业是由打印机获取的;否则为 false。 只读。|
|copiesPrinted|Int32|打印的副本数。 只读。|
|pageCount|Int32|打印的页面总数。 只读。|
|blackAndWhitePageCount|Int32|打印的黑白页数。 只读。|
|colorPageCount|Int32|打印的颜色页数。 只读。|
|simplexPageCount|Int32|打印的简单 (单面) 页的数目。 只读。|
|duplexPageCount|Int32|双面) 打印的双面 (双面页的数目。 只读。|
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

