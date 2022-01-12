---
title: windows 资源类型
description: 充当功能容器Windows实体。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 8033e9a349be7aafa584d6ab2e5e69bdab66eeb7
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861488"
---
# <a name="windows-resource-type"></a>windows 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

充当功能容器Windows实体。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|只读。 继承自 [实体](../resources/entity.md)|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|updates|[microsoft.graph.windowsUpdates.updates](../resources/windowsupdates-updates.md)|充当 Windows Update for Business 部署服务功能的容器的实体。 只读。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.windows",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.windows",
  "id": "String (identifier)"
}
```

