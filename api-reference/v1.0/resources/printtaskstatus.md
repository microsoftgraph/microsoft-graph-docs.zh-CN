---
title: printTaskStatus 资源类型
description: 表示 printTask 的当前执行状态。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 7f07ee889cb8f04edff66416ebc6ce49f7e7a3ab67a07119170929fdc12cdf8c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229015"
---
# <a name="printtaskstatus-resource-type"></a>printTaskStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

表示 [printTask 的当前执行状态](printtask.md)。 

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|state|printTaskProcessingState|[printTask 的当前处理状态](printtask.md)。 下表介绍了有效值。|
|说明|String|可读的 [printTask](printtask.md)当前处理状态的说明。|

### <a name="printtaskprocessingstate-values"></a>printTaskProcessingState 值

|成员|值|说明|
|:---|:---|:---|
|pending|0|任务执行挂起。|
|processing|1|任务执行正在进行中。|
|已完成|2|任务执行已完成。|
|aborted|3|任务执行已中止。|
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

