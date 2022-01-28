---
title: teamworkPeripheralsHealth 资源类型
description: 表示连接到已启用Microsoft Teams设备的所有外围设备的运行状况详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d48c0351a20ed1074f5bb2fd4443d40bf96d52d6
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262347"
---
# <a name="teamworkperipheralshealth-resource-type"></a>teamworkPeripheralsHealth 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示连接到已启用Microsoft Teams设备的所有外围设备的[运行状况详细信息](../resources/teamworkdevice.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|communicationSpeakerHealth|[teamworkPeripheralHealth](../resources/teamworkperipheralhealth.md)|有关通信扬声器的运行状况详细信息。|
|contentCameraHealth|[teamworkPeripheralHealth](../resources/teamworkperipheralhealth.md)|有关内容相机的运行状况详细信息。|
|displayHealthCollection|[teamworkPeripheralHealth](../resources/teamworkperipheralhealth.md) 集合|有关显示的运行状况详细信息。|
|microphoneHealth|[teamworkPeripheralHealth](../resources/teamworkperipheralhealth.md)|有关麦克风的运行状况详细信息。|
|roomCameraHealth|[teamworkPeripheralHealth](../resources/teamworkperipheralhealth.md)|有关会议室相机的运行状况详细信息。|
|speakerHealth|[teamworkPeripheralHealth](../resources/teamworkperipheralhealth.md)|有关扬声器的运行状况详细信息。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkPeripheralsHealth"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkPeripheralsHealth",
  "communicationSpeakerHealth": {
    "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
  },
  "contentCameraHealth": {
    "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
  },
  "displayHealthCollection": [
    {
      "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
    }
  ],
  "microphoneHealth": {
    "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
  },
  "roomCameraHealth": {
    "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
  },
  "speakerHealth": {
    "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
  }
}
```

