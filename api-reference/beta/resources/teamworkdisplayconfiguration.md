---
title: teamworkDisplayConfiguration 资源类型
description: 表示有关已启用屏幕的设备Microsoft Teams配置的详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 88de0c02af3012b1fff55f4ef1cb0f58773c4f7b
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262306"
---
# <a name="teamworkdisplayconfiguration-resource-type"></a>teamworkDisplayConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关已启用屏幕的设备Microsoft Teams配置[的详细信息](../resources/teamworkdevice.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|configuredDisplays|[teamworkConfiguredPeripheral](../resources/teamworkconfiguredperipheral.md) 集合|配置的显示列表。 仅适用于Microsoft Teams 会议室设备。|
|displayCount|Int32|连接显示器的总数，包括内置屏幕。 仅适用于Teams 会议室设备。|
|inBuiltDisplayScreenConfiguration|[teamworkDisplayScreenConfiguration](../resources/teamworkdisplayscreenconfiguration.md)|内置显示器的配置。 不适用于Teams 会议室设备。|
|isContentDuplicationAllowed|Boolean|`True` 是否允许内容复制。 仅适用于Teams 会议室设备。|
|isDualDisplayModeEnabled|Boolean|`True` 如果启用了双显示模式。 如果 **isDualDisplayModeEnabled** `true`为 ，则当内容通过 Microsoft Teams 会议室 设备的 HDMI 输入模块共享时，内容将显示在两个会议室屏幕的前面，而不是只显示在一个屏幕上。 仅适用于Teams 会议室设备。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkDisplayConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDisplayConfiguration",
  "configuredDisplays": [
    {
      "@odata.type": "microsoft.graph.teamworkConfiguredPeripheral"
    }
  ],
  "displayCount": "Integer",
  "inBuiltDisplayScreenConfiguration": {
    "@odata.type": "microsoft.graph.teamworkDisplayScreenConfiguration"
  },
  "isContentDuplicationAllowed": "Boolean",
  "isDualDisplayModeEnabled": "Boolean"
}
```

