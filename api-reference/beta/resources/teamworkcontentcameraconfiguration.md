---
title: teamworkContentCameraConfiguration 资源类型
description: 表示连接到启用了 Microsoft Teams 设备的内容相机的配置详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 00db0e0fbd61afe3f113a903d60aeb5bf02f6581
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262434"
---
# <a name="teamworkcontentcameraconfiguration-resource-type"></a>teamworkContentCameraConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示连接到启用了 Microsoft Teams 设备的内容相机的配置[详细信息](../resources/teamworkdevice.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|isContentCameraInverted|Boolean|`True` 如果反转内容相机。|
|isContentCameraOptional|Boolean|`True` 如果内容相机是可选的。|
|isContentEnhancementEnabled|Boolean|`True` 如果已启用内容增强功能。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkContentCameraConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkContentCameraConfiguration",
  "isContentCameraInverted": "Boolean",
  "isContentCameraOptional": "Boolean",
  "isContentEnhancementEnabled": "Boolean"
}
```

