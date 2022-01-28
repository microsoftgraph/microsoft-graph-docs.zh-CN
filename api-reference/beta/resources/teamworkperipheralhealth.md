---
title: teamworkPeripheralHealth 资源类型
description: 表示连接到已启用Microsoft Teams设备的外围设备的运行状况详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 914165343623fea7f807b5dc5f8146b79714c90e
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262329"
---
# <a name="teamworkperipheralhealth-resource-type"></a>teamworkPeripheralHealth 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示连接到已启用Microsoft Teams设备的外围设备的运行状况[详细信息](../resources/teamworkdevice.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|connection|[teamworkConnection](../resources/teamworkconnection.md)|外围设备连接后已连接的状态和时间。|
|isOptional|Boolean|`True` 如果外设是可选的。 用于运行状况计算。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|外设|[teamworkPeripheral](../resources/teamworkperipheral.md)|有关外围设备的信息。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkPeripheralHealth",
  "connection": {
    "@odata.type": "microsoft.graph.teamworkConnection"
  },
  "isOptional": "Boolean"
}
```

