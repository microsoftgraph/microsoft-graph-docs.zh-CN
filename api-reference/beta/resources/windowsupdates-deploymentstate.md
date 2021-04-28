---
title: deploymentState 资源类型
description: 描述和控制部署的当前状态。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: d05bf09fbad405e93ee994858e2d6ac65a8088a7
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067292"
---
# <a name="deploymentstate-resource-type"></a>deploymentState 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述和控制部署的当前状态。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|原因|[microsoft.graph.windowsUpdates.deploymentStateReason](../resources/windowsupdates-deploymentstatereason.md) 集合|指定部署具有其状态值的原因。 只读。|
|requestedValue|microsoft.graph.windowsUpdates.requestedDeploymentStateValue|指定部署的请求状态。 支持 **requestedDeploymentStateValue 值的子集**。 可取值为：`none`、`paused`。|
|值|microsoft.graph.windowsUpdates.deploymentStateValue|指定部署的状态。 支持 **deploymentStateValue** 值的子集。 可取值为：`scheduled`、`offering`、`paused`。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.deploymentState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deploymentState",
  "value": "String",
  "reasons": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason"
    }
  ],
  "requestedValue": "String",
}
```

