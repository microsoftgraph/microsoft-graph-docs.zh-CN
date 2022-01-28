---
title: teamworkMicrophoneConfiguration 资源类型
description: 表示有关设备麦克风配置Microsoft Teams 会议室的详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cd24375f573e9ff57a0cf9786aee26b1e0826c7c
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262311"
---
# <a name="teamworkmicrophoneconfiguration-resource-type"></a>teamworkMicrophoneConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关设备麦克风配置Microsoft Teams 会议室[的详细信息](../resources/teamworkdevice.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|isMicrophoneOptional|Boolean|`True` 如果配置的麦克风是可选的。 `False` 如果麦克风不是可选的，并且应计算设备的运行状况。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|defaultMicrophone|[teamworkPeripheral](../resources/teamworkperipheral.md)|有关默认麦克风的信息。|
|麦克风|[teamworkPeripheral](../resources/teamworkperipheral.md) 集合|麦克风的集合。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkMicrophoneConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkMicrophoneConfiguration",
  "isMicrophoneOptional": "Boolean"
}
```

