---
title: windows 资源类型
description: 充当功能容器Windows实体。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 3f7677f97db8d57e1fba74174df8cd848ad4f224
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067295"
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

