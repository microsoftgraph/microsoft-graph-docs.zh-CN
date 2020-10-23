---
title: printJobStatus 资源类型
description: 表示打印作业的当前状态。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: bb3221eb12946d58664211731a31993e540aaf00
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728933"
---
# <a name="printjobstatus-resource-type"></a>printJobStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示打印作业的当前状态。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|state|printJobProcessingState|打印作业的当前处理状态。 有效值如下表所述。 只读。|
|详细信息|printJobProcessingDetail 集合|打印作业状态的其他详细信息。 有效值如下表所述。 只读。|
|说明|String|打印作业的当前处理状态的可读说明。 只读。|
|isAcquiredByPrinter|布尔|如果作业已由打印机确认，则为 True; 否则为 false。否则为 false。 只读。|

### <a name="printjobprocessingstate-values"></a>printJobProcessingState 值

|成员|值|说明|
|:---|:---|:---|
|unknown|0|无法识别打印机报告的处理状态。|
|决|1|打印作业正在等待打印机处理。|
|处理|双面|打印机当前正在处理打印作业。|
|停留|第三章|打印作业已暂停。|
|停止|4 |打印作业已停止，因为需要先解决打印机问题，然后才能继续执行作业。 在打印机状态资源中可以找到详细信息。|
|后|5 |打印作业已成功完成，不会进行进一步的处理。|
|取消|6 |打印作业已被用户取消，不会进行进一步的处理。|
|其间|7 |打印作业已被用户或打印机中止，不会进行进一步处理。|

### <a name="printjobprocessingdetail-values"></a>printJobProcessingDetail 值

|成员|值|说明|
|:---|:---|:---|
|uploadPending|0|尚未上传文档有效负载。|
|改变|1|正在转换文档有效负载。|
|completedSuccessfully|双面|作业已成功完成。|
|completedWithWarnings|第三章|作业已完成，但出现警告。|
|completedWithErrors|4 |作业已完成，但有错误。|
|releaseWait|5 |作业挂起，无法释放。|
|口译|6 |作业处于 "正在处理" 状态，但更具体地说，是解释文档有效负载。|

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
    "state": "String",
    "description": "String",
    "isAcquiredByPrinter": true,    
    "details": ["String"]
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

