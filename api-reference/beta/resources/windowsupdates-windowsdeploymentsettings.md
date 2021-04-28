---
title: windowsDeploymentSettings 资源类型
description: 设置控制服务何时以及如何部署Windows 10更新。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: bc55f0643e789c802254064797bf8a5c2047cb64
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067300"
---
# <a name="windowsdeploymentsettings-resource-type"></a>windowsDeploymentSettings 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

设置控制服务何时以及如何部署Windows 10更新。

继承自 [deploymentSettings](../resources/windowsupdates-deploymentsettings.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|monitoring|[microsoft.graph.windowsUpdates.monitoringSettings](../resources/windowsupdates-monitoringsettings.md)|设置管理条件，以监视要采取的自动操作。 继承自 [deploymentSettings](../resources/windowsupdates-deploymentsettings.md)。|
|推出|[microsoft.graph.windowsUpdates.rolloutSettings](../resources/windowsupdates-rolloutsettings.md)|设置如何推出内容。继承自[deploymentSettings](../resources/windowsupdates-deploymentsettings.md)。|
|userExperience|[microsoft.graph.windowsUpdates.userExperienceSettings](../resources/windowsupdates-userexperiencesettings.md)|设置在设备上管理用户的更新体验。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.windowsDeploymentSettings",
  "rollout": {
    "@odata.type": "microsoft.graph.windowsUpdates.rolloutSettings"
  },
  "monitoring": {
    "@odata.type": "microsoft.graph.windowsUpdates.monitoringSettings"
  },
  "userExperience": {
    "@odata.type": "microsoft.graph.windowsUpdates.userExperienceSettings"
  }
}
```

