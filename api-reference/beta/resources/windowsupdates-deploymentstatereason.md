---
title: deploymentStateReason 资源类型
description: 特定部署状态的原因。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 19a5063cd4f103b0f065311118bc5d8ac97a3c7a
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067977"
---
# <a name="deploymentstatereason-resource-type"></a>deploymentStateReason 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特定部署状态的原因。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|值|microsoft.graph.windowsUpdates.deploymentStateReasonValue|指定部署状态的原因。 可取值为：`scheduledByOfferWindow`、`offeringByRequest`、`pausedByRequest`、`pausedByMonitoring`。 只读。|

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

