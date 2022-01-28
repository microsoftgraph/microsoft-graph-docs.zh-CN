---
title: teamworkActivePeripherals 资源类型
description: 表示与连接到已启用Microsoft Teams设备的活动外围设备有关的详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e1f740a347f4adc717588dccc49acafc145e42c8
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262486"
---
# <a name="teamworkactiveperipherals-resource-type"></a>teamworkActivePeripherals 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与连接到启用了 Microsoft Teams 的设备的活动外围设备[有关的详细信息](../resources/teamworkdevice.md)。

## <a name="properties"></a>属性
无。

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|communicationSpeaker|[teamworkPeripheral](../resources/teamworkperipheral.md)|链接的通信扬声器详细信息。|
|contentCamera|[teamworkPeripheral](../resources/teamworkperipheral.md)|链接的内容相机详细信息。|
|麦克风|[teamworkPeripheral](../resources/teamworkperipheral.md)|链接的麦克风详细信息。|
|roomCamera|[teamworkPeripheral](../resources/teamworkperipheral.md)|链接的会议室相机详细信息。|
|speaker|[teamworkPeripheral](../resources/teamworkperipheral.md)|链接的扬声器详细信息。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkActivePeripherals"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkActivePeripherals"
}
```

