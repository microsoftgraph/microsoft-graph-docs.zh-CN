---
title: deploymentState 资源类型
description: 描述和控制部署的当前状态。
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 80b691c6404bac3e98c4c5c6acb9596b5d4c8821
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890827"
---
# <a name="deploymentstate-resource-type"></a>deploymentState 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述和控制部署的当前状态。

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|原因|[microsoft.graph.windowsUpdates.deploymentStateReason](../resources/windowsupdates-deploymentstatereason.md) 集合|指定部署具有其状态值的原因。 只读。|
|requestedValue|microsoft.graph.windowsUpdates.requestedDeploymentStateValue|指定部署的请求状态。 支持 **requestedDeploymentStateValue 值的子集**。 可取值为：`none`、`paused`、`unknownFutureValue`。|
|值|microsoft.graph.windowsUpdates.deploymentStateValue|指定部署的状态。 支持 **deploymentStateValue** 值的子集。 可取值为：`scheduled`、`offering`、`paused`、`unknownFutureValue`。 只读。|

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

