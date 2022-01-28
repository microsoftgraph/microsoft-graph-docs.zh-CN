---
title: teamworkHardwareDetail 资源类型
description: 表示有关启用了 Microsoft Teams 的硬件属性的详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ec4c292666a8889a34d1dce85c9a3d70630825a7
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262323"
---
# <a name="teamworkhardwaredetail-resource-type"></a>teamworkHardwareDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关已启用Microsoft Teams硬件属性[的详细信息](../resources/teamworkdevice.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|macAddresses|String 集合|MAC 地址。|
|manufacturer|String|设备制造商。|
|model|String|开发模型。|
|serialNumber|String|设备序列号。|
|uniqueId|String|设备唯一标识符。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkHardwareDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkHardwareDetail",
  "macAddresses": [
    "String"
  ],
  "manufacturer": "String",
  "model": "String",
  "serialNumber": "String",
  "uniqueId": "String"
}
```

