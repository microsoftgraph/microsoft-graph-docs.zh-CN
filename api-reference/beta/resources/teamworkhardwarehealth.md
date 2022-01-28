---
title: teamworkHardwareHealth 资源类型
description: 表示有关已启用Microsoft Teams硬件运行状况的详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cc552dc46199e1107220ae6ed27c839126e4888f
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262313"
---
# <a name="teamworkhardwarehealth-resource-type"></a>teamworkHardwareHealth 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关已启用Microsoft Teams硬件运行状况[的详细信息](../resources/teamworkdevice.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|computeHealth|[teamworkPeripheralHealth](../resources/teamworkperipheralhealth.md)|团队合作的系统运行状况 [详细信息](../resources/teamworkdevice.md)。|
|hdmiIngestHealth|[teamworkPeripheralHealth](../resources/teamworkperipheralhealth.md)|有关设备的 HDMI 输入的运行状况详细信息。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkHardwareHealth"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkHardwareHealth",
  "computeHealth": {
    "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
  },
  "hdmiIngestHealth": {
    "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
  }
}
```

