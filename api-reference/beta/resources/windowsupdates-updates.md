---
title: 更新资源类型
description: 充当所有 Windows Update for Business 部署服务功能的容器的实体。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 748ef5c6e8e334b2e1c311c07617c181490f4f39
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861538"
---
# <a name="updates-resource-type"></a>更新资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

充当所有 Windows Update for Business 部署服务功能的容器的实体。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|只读。 继承自 [实体](../resources/entity.md)|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|catalog|[microsoft.graph.windowsUpdates.catalog](../resources/windowsupdates-catalog.md)|部署服务可以批准部署的内容目录。 只读。|
|部署|[microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md) 集合|使用部署服务创建的部署。 只读。|
|updatableAssets|[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合|在部署服务中注册可接收更新的资产。 只读。|

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

