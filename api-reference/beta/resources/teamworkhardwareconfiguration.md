---
title: teamworkHardwareConfiguration 资源类型
description: 表示有关启用了 Microsoft Teams 设备的硬件配置的详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 118c2cda70a9751ce8c02a9af52d89982141dfef
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262334"
---
# <a name="teamworkhardwareconfiguration-resource-type"></a>teamworkHardwareConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关已启用硬件配置的设备[Microsoft Teams的详细信息。](../resources/teamworkdevice.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|processorModel|String|设备的 CPU 模型。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|compute|[teamworkPeripheral](../resources/teamworkperipheral.md)|团队合作的系统 [详细信息](../resources/teamworkdevice.md)。|
|hdmiIngest|[teamworkPeripheral](../resources/teamworkperipheral.md)|有关设备的 HDMI 输入的产品详细信息。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkHardwareConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkHardwareConfiguration",
  "processorModel": "String"
}
```

