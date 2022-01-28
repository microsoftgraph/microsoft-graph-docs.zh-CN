---
title: teamworkSpeakerConfiguration 资源类型
description: 表示有关设备扬声器配置Microsoft Teams 会议室的详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 88c15b97ea1b2d3984f8e3c3c4a41873fc228ad0
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262312"
---
# <a name="teamworkspeakerconfiguration-resource-type"></a>teamworkSpeakerConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关设备扬声器配置Microsoft Teams 会议室[的详细信息](../resources/teamworkdevice.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|isCommunicationSpeakerOptional|Boolean|`True` 如果通信扬声器是可选的。 用于计算通信扬声器不是可选的运行状况。|
|isSpeakerOptional|Boolean|`True` 如果配置的扬声器是可选的。 用于在扬声器不是可选的时计算运行状况。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|defaultCommunicationSpeaker|[teamworkPeripheral](../resources/teamworkperipheral.md)|用于会议的默认通信扬声器。|
|defaultSpeaker|[teamworkPeripheral](../resources/teamworkperipheral.md)|用于所有媒体和通知声音的默认扬声器。|
|扬声器|[teamworkPeripheral](../resources/teamworkperipheral.md) 集合|连接的扬声器列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkSpeakerConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkSpeakerConfiguration",
  "isCommunicationSpeakerOptional": "Boolean",
  "isSpeakerOptional": "Boolean"
}
```

