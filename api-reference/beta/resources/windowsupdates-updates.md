---
title: 更新资源类型
description: 充当企业部署服务功能所有Windows 更新的容器的实体。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a315516e8ded53cfacbe94c0ace2d9c12c5b3f78
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856412"
---
# <a name="updates-resource-type"></a>更新资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

充当企业部署服务功能所有Windows 更新的容器的实体。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|只读。 继承自 [实体](../resources/entity.md)|

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|目录|[microsoft.graph.windowsUpdates.catalog](../resources/windowsupdates-catalog.md)|可由部署服务批准部署的内容目录。 只读。|
|部署|[microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md) 集合|使用部署服务创建的部署。 只读。|
|resourceConnections|[microsoft.graph.windowsUpdates.resourceConnection](../resources/windowsupdates-resourceconnection.md) 集合|与外部资源（如分析工作区）的服务连接。|
|updatableAssets|[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合|向部署服务注册的可接收更新的资产。 只读。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.updates",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updates",
  "id": "String (identifier)"
}
```

