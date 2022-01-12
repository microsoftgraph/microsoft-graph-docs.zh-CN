---
title: 部署资源类型
description: 表示内容部署到一组设备。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: d4d34481b6a1d99d7c2a48b3becd7b8def764924
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61841940"
---
# <a name="deployment-resource-type"></a>部署资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示内容部署到一组设备。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出部署](../api/windowsupdates-updates-list-deployments.md)|[microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md) 集合|获取部署对象 [及其](../resources/windowsupdates-deployment.md) 属性的列表。|
|[创建部署](../api/windowsupdates-updates-post-deployments.md)|[microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md)|创建新的 [部署](../resources/windowsupdates-deployment.md) 对象。|
|[获取部署](../api/windowsupdates-deployment-get.md)|[microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md)|读取部署 [对象的属性和](../resources/windowsupdates-deployment.md) 关系。|
|[更新部署](../api/windowsupdates-deployment-update.md)|[microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md)|更新 [部署对象的属性](../resources/windowsupdates-deployment.md) 。|
|[删除部署](../api/windowsupdates-deployment-delete.md)|None|删除 [部署对象](../resources/windowsupdates-deployment.md) 。|
|[列出访问群体成员](../api/windowsupdates-deploymentaudience-list-members.md)|[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合|列出部署访问群体的成员。|
|[列出访问群体排除项](../api/windowsupdates-deploymentaudience-list-exclusions.md)|[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合|列出部署访问群体中的排除项。|
|[更新访问群体成员和排除项](../api/windowsupdates-deploymentaudience-updateaudience.md)|None|添加或删除部署访问群体的成员和排除项。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|内容|[microsoft.graph.windowsUpdates.deployableContent](../resources/windowsupdates-deployablecontent.md)|指定要部署的内容。 无法更改。 默认情况下返回。|
|createdDateTime|DateTimeOffset|创建部署的日期和时间。 默认情况下返回。 只读。|
|id|String|部署的唯一标识符。 默认情况下返回。 键。 不可为 null。 只读。|
|lastModifiedDateTime|DateTimeOffset|上次修改部署的日期和时间。 默认情况下返回。 只读。|
|settings|[microsoft.graph.windowsUpdates.deploymentSettings](../resources/windowsupdates-deploymentsettings.md)|设置在管理如何部署内容的特定部署上 **指定。** 默认返回。|
|state|[microsoft.graph.windowsUpdates.deploymentState](../resources/windowsupdates-deploymentstate.md)|部署的执行状态。 默认返回。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|audience|[microsoft.graph.windowsUpdates.deploymentAudience](../resources/windowsupdates-deploymentaudience.md)|指定内容部署到的目标访问群体。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.deployment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
  "id": "String (identifier)",
  "state": {
    "@odata.type": "microsoft.graph.windowsUpdates.deploymentState"
  },
  "content": {
    "@odata.type": "microsoft.graph.windowsUpdates.deployableContent"
  },
  "settings": {
    "@odata.type": "microsoft.graph.windowsUpdates.deploymentSettings"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

