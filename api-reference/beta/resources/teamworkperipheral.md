---
title: teamworkPeripheral 资源类型
description: 表示与连接到启用了Microsoft Teams的外围设备有关的详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 645cf2d64e50d4d46fe2e76ff8c92dcdf948c74f
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262345"
---
# <a name="teamworkperipheral-resource-type"></a>teamworkPeripheral 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与连接到已启用Microsoft Teams的外围设备[有关的详细信息](../resources/teamworkdevice.md)。

继承自 [实体](../resources/entity.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|外设的显示名称。|
|id|String|特定外设的唯一标识符。 继承自 [实体](../resources/entity.md)。|
|productId|String|设备的产品 ID。 供应商的每个产品都有自己的 ID。|
|vendorId|String|设备供应商的唯一标识符。 每个供应商都有一个唯一 ID。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkPeripheral",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkPeripheral",
  "displayName": "String",
  "id": "String (identifier)",
  "productId": "String",
  "vendorId": "String"
}
```

