---
title: windowsDeploymentSettings 资源类型
description: 设置控制服务何时以及如何部署Windows 10更新。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 16aa8592dc03dda799ffbddf838520ca0f159192
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861370"
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
|推出|[microsoft.graph.windowsUpdates.rolloutSettings](../resources/windowsupdates-rolloutsettings.md)|设置如何推出内容。。继承自[deploymentSettings](../resources/windowsupdates-deploymentsettings.md)。|
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

