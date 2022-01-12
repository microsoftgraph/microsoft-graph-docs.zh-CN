---
title: deploymentState 资源类型
description: 描述和控制部署的当前状态。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: e900e3ec23e50a33fabb2d9bb55cf5bfab91a3f3
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61798492"
---
# <a name="deploymentstate-resource-type"></a>deploymentState 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述和控制部署的当前状态。

## <a name="properties"></a>属性
|属性|类型|说明|
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

