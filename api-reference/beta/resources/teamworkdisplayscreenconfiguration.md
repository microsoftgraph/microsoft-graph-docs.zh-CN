---
title: teamworkDisplayScreenConfiguration 资源类型
description: 表示有关已启用屏幕的设备显示屏幕Microsoft Teams的详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2346de5fa301d1b2db7fd50e4a64c7168eea8a47
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262308"
---
# <a name="teamworkdisplayscreenconfiguration-resource-type"></a>teamworkDisplayScreenConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关已启用屏幕的设备显示屏幕[Microsoft Teams的详细信息。](../resources/teamworkdevice.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|一些|Int32|设备的亮度级别 (0-100) 。 不适用于Microsoft Teams 会议室设备。|
|将timeout|期限| (30-3600 秒) 。 不适用于Teams 会议室设备。|
|isHighContrastEnabled|Boolean|`True` 如果启用高对比度模式。 不适用于Teams 会议室设备。|
|isScreensaverEnabled|Boolean|`True` 如果启用了屏幕保护程序。 不适用于Teams 会议室设备。|
|screensaverTimeout|期限|屏幕保护超时时间从 30 秒到 3600 秒。 不适用于Teams 会议室设备。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkDisplayScreenConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDisplayScreenConfiguration",
  "backlightBrightness": "Integer",
  "backlightTimeout": "String (duration)",
  "isHighContrastEnabled": "Boolean",
  "isScreensaverEnabled": "Boolean",
  "screensaverTimeout": "String (duration)"
}
```

