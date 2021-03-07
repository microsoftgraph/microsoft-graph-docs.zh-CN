---
title: printTaskStatus 资源类型
description: 表示 printTask 的当前执行状态。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: ef5587050926fef5fa924f6d541de63d5b1d33aa
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517265"
---
# <a name="printtaskstatus-resource-type"></a>printTaskStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

表示 [printTask 的当前执行状态](printtask.md)。 

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|state|printTaskProcessingState|[printTask 的当前处理状态](printtask.md)。 下表介绍了有效值。|
|说明|String|打印 [Task](printtask.md)的当前处理状态的人读说明。|

### <a name="printtaskprocessingstate-values"></a>printTaskProcessingState 值

|成员|值|Description|
|:---|:---|:---|
|挂起|0|任务执行挂起。|
|processing|1 |任务执行正在进行中。|
|已完成|2 |任务执行已完成。|
|已中止|3 |任务执行已中止。|
|unknownFutureValue|4 |可发展枚举 sentinel 值。 请勿使用。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printTaskStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printTaskStatus",
  "state": "String",
  "description": "String"
}
```

