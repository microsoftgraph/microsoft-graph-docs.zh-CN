---
title: printJobStatus 资源类型
description: 表示打印作业的当前状态。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 73038bbea54860ef37b8ebbf2602450dc556efd2
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176674"
---
# <a name="printjobstatus-resource-type"></a>printJobStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示打印作业的当前状态。

## <a name="properties"></a>属性
| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|state|printJobProcessingState|打印作业的当前处理状态。 下表描述了有效值。 只读。|
|详细信息|printJobProcessingDetail 集合|打印作业状态的其他详细信息。 下表描述了有效值。 只读。|
|说明|String|打印作业当前处理状态的人工可读说明。 只读。|
|isAcquiredByPrinter|Boolean|如此 如果该作业已由打印机确认;否则为 false。 只读。|

### <a name="printjobprocessingstate-values"></a>printJobProcessingState 值

|成员|值|Description|
|:---|:---|:---|
|unknown|0|无法识别打印机报告的处理状态。|
|等待|1|打印作业正在等待打印机的处理。|
|处理|2|打印机当前正在处理打印作业。|
|暂停|3|打印作业已暂停。|
|停止|4|打印作业已停止，因为在继续作业之前，需要解决打印机问题。 可以在打印机状态资源中找到详细信息。|
|完成|5|打印作业已成功完成，不会进行进一步处理。|
|取消|6 |打印作业已由用户取消，不会进行进一步处理。|
|中止|7 |打印作业已被用户或打印机中止，不会进行进一步处理。|

### <a name="printjobprocessingdetail-values"></a>printJobProcessingDetail 值

|成员|值|Description|
|:---|:---|:---|
|uploadPending|0|文档有效负载尚未上传。|
|转化|1|正在转换文档有效负载。|
|completedSuccessfully|2|作业已成功完成。|
|completedWithWarnings|3|作业已使用警告完成。|
|completedWithErrors|4|作业已完成并出现错误。|
|releaseWait|5|作业正在等待发布。|
|解释|6 |作业处于“处理”状态，但更具体地说，正在解释文档有效负载。|

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

