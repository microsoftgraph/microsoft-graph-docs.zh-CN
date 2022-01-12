---
title: deploymentAudience 资源类型
description: 部署可应用到的 updatableAsset 资源集。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: ab436c0fa9f726528b190fa6fe2f638890447ce4
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61863362"
---
# <a name="deploymentaudience-resource-type"></a>deploymentAudience 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

部署[可应用到的 updatableAsset](../resources/windowsupdates-updatableasset.md)[资源集](../resources/windowsupdates-deployment.md)。

如果排除项和成员关系中包含同一 **updatableAsset** **资源，** 则部署不适用于它。 

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出成员](../api/windowsupdates-deploymentaudience-list-members.md)|[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合|列出 [deploymentAudience 的成员](../resources/windowsupdates-deploymentaudience.md)。|
|[列表排除项](../api/windowsupdates-deploymentaudience-list-exclusions.md)|[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合|列出 [deploymentAudience 的排除项](../resources/windowsupdates-deploymentaudience.md)。|
|[更新成员和排除项](../api/windowsupdates-deploymentaudience-updateaudience.md)|None|添加或删除成员和排除项。|
|[按 ID 更新 (排除) ](../api/windowsupdates-deploymentaudience-updateaudiencebyid.md)|None|添加或删除相同类型的成员和排除项。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|部署访问群体的唯一标识符。 默认情况下返回。 键。 不可为 null。 只读。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|排除项|[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合|指定要从访问群体中排除的资产。|
|members|[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合|指定要包括在访问群体中的资源。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.deploymentAudience",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deploymentAudience",
  "id": "String (identifier)"
}
```

