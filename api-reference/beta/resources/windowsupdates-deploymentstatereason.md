---
title: deploymentStateReason 资源类型
description: 特定部署状态的原因。
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 54240d057734d17df3e0df3a270d1aab00022586
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890449"
---
# <a name="deploymentstatereason-resource-type"></a>deploymentStateReason 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特定部署状态的原因。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|值|microsoft.graph.windowsUpdates.deploymentStateReasonValue|指定部署状态的原因。 可能的值是：`scheduledByOfferWindow`、`offeringByRequest`、`pausedByRequest`、`pausedByMonitoring`。 请注意，必须使用此可变化枚举中的 (标头) 获取以下 `Prefer: include-unknown-enum-members` [值](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) `faultedByContentOutdated` ： 。 只读。|

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

