---
title: deploymentSettings 资源类型
description: 确定服务何时以及如何部署更新。
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 0906f401ac414928549602d602317ddc3f5305c5
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695711"
---
# <a name="deploymentsettings-resource-type"></a>deploymentSettings 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

确定服务何时以及如何部署更新。

[windowsDeploymentSettings 的基本类型](../resources/windowsupdates-windowsdeploymentsettings.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|monitoring|[microsoft.graph.windowsUpdates.monitoringSettings](../resources/windowsupdates-monitoringsettings.md)|设置管理条件以监视要采取的自动操作。|
|推出|[microsoft.graph.windowsUpdates.rolloutSettings](../resources/windowsupdates-rolloutsettings.md)|设置如何推出内容。|
|safeguard|[microsoft.graph.windowsUpdates.safeguardSettings](../resources/windowsupdates-safeguardsettings.md)|设置内容管理安全措施的保留。|

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
  },
  "safeguard": {
    "@odata.type": "microsoft.graph.windowsUpdates.safeguardSettings"
  }
}
```

