---
title: deploymentSettings 资源类型
description: 设置控制服务何时以及如何部署更新。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: f7c00ec8e880e7fd7ae9109fd1ac015868da902a
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067856"
---
# <a name="deploymentsettings-resource-type"></a>deploymentSettings 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

设置控制服务何时以及如何部署更新。

[windowsDeploymentSettings 的基本类型](../resources/windowsupdates-windowsdeploymentsettings.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|monitoring|[microsoft.graph.windowsUpdates.monitoringSettings](../resources/windowsupdates-monitoringsettings.md)|设置管理条件，以监视要采取的自动操作。|
|推出|[microsoft.graph.windowsUpdates.rolloutSettings](../resources/windowsupdates-rolloutsettings.md)|设置如何推出内容。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.deploymentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deploymentSettings",
  "rollout": {
    "@odata.type": "microsoft.graph.windowsUpdates.rolloutSettings"
  },
  "monitoring": {
    "@odata.type": "microsoft.graph.windowsUpdates.monitoringSettings"
  }
}
```

