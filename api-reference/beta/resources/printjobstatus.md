---
title: printJobStatus 资源类型
description: 表示打印作业的当前状态。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 1973d00ff8ca544f0acd1992626de9a3eaf59700
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895602"
---
# <a name="printjobstatus-resource-type"></a>printJobStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示打印作业的当前状态。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|processingState|printJobProcessingState|打印作业的当前处理状态。 有效值如下表所述。 只读。|
|processingStateDescription|String|打印作业的当前处理状态的可读说明。 只读。|
|acquiredByPrinter|布尔|如果作业已由打印机确认，则为 True; 否则为 false。否则为 false。 只读。|

### <a name="printjobprocessingstate-values"></a>printJobProcessingState 值

|成员|值|说明|
|:---|:---|:---|
|unknown|0|无法识别打印机报告的处理状态。|
|决|1|打印作业正在等待打印机处理。|
|pendingHeld|双面|该作业不是处理的候选项。 确保没有导致作业无法启动的错误或资源限制。|
|处理|第三章|打印机当前正在处理打印作业。|
|停留|4 |用户已暂停打印作业。|
|停止|5 |打印作业已停止，因为需要先解决打印机问题，然后才能继续执行作业。 在打印机状态资源中可以找到详细信息。|
|后|6 |打印作业已成功完成，不会进行进一步的处理。|
|取消|7 |打印作业已被用户取消，不会进行进一步的处理。|
|其间|8 |打印作业已被用户或打印机中止，不会进行进一步处理。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printJobStatus"
}-->

```json
{
    "processingState": "String",
    "processingStateDescription": "String",
    "acquiredByPrinter": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJobStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->