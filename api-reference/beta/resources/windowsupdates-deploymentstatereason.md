---
title: deploymentStateReason 资源类型
description: 特定部署状态的原因。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 754bf9ad430e86be987d913335b761447a9c6956
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61862330"
---
# <a name="deploymentstatereason-resource-type"></a>deploymentStateReason 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特定部署状态的原因。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|值|microsoft.graph.windowsUpdates.deploymentStateReasonValue|指定部署状态的原因。 可能的值是：`scheduledByOfferWindow`、`offeringByRequest`、`pausedByRequest`、`pausedByMonitoring`。 请注意，必须使用此可变化枚举 (请求) 获取以下 `Prefer: include-unknown-enum-members` [值](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) `faultedByContentOutdated` ： 。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deploymentStateReason",
  "value": "String"
}
```

