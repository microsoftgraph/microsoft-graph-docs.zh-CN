---
title: printJobStatus 资源类型
description: 表示打印作业的当前状态。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: acb8b99af64a33219336972fa9df590dac602138058307fc5ca690322e4ada9b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218427"
---
# <a name="printjobstatus-resource-type"></a>printJobStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

表示打印作业的当前状态。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|state|printJobProcessingState|打印作业的当前处理状态。 下表介绍了有效值。 只读。|
|详细信息|printJobProcessingDetail 集合|打印作业状态的其他详细信息。 下表介绍了有效值。 只读。|
|说明|String|可读的打印作业当前处理状态的说明。 只读。|
|isAcquiredByPrinter|Boolean|如此 如果打印机确认作业;否则为 false。 只读。|

### <a name="printjobprocessingstate-values"></a>printJobProcessingState 值

|成员|值|说明|
|:---|:---|:---|
|unknown|0|无法识别打印机报告的处理状态。|
|pending|1|打印作业正等待打印机进行处理。|
|processing|2|打印作业当前正由打印机处理。|
|paused|3|打印作业已暂停。|
|已停止|4 |打印作业已停止，因为需要解决打印机的问题，然后作业才能继续。 有关详细信息，请参阅打印机状态资源。|
|已完成|5 |打印作业已成功完成，不会进行进一步处理。|
|canceled|6 |打印作业已由用户取消，不会进行进一步处理。|
|aborted|7 |打印作业已由用户或打印机中止，不会进行进一步处理。|

### <a name="printjobprocessingdetail-values"></a>printJobProcessingDetail 值

|成员|值|说明|
|:---|:---|:---|
|uploadPending|0|文档有效负载尚未上载。|
|transforming|1|正在转换文档负载。|
|completedSuccessfully|2|作业已成功完成。|
|completedWithWarnings|3|作业已完成，并出现警告。|
|completedWithErrors|4 |作业已完成，出现错误。|
|releaseWait|5 |作业正在等待释放。|
|解释|6 |作业的状态为"正在处理"，但更具体地说，正在解释文档有效负载。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printJobStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printJobStatus",
  "state": "String",
  "description": "String",
  "isAcquiredByPrinter": "Boolean",
  "details": [
    "String"
  ]
}
```

