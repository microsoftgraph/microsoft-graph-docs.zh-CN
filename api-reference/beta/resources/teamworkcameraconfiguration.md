---
title: teamworkCameraConfiguration 资源类型
description: 表示有关设备相机配置的详细信息Microsoft Teams 会议室设备。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f10a0db06b158dda00f4db9e7df0e34e1ab6ac1c
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262325"
---
# <a name="teamworkcameraconfiguration-resource-type"></a>teamworkCameraConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关移动设备的相机配置Microsoft Teams 会议室[的详细信息](../resources/teamworkdevice.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|contentCameraConfiguration|[teamworkContentCameraConfiguration](../resources/teamworkcontentcameraconfiguration.md)|内容相机的配置。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|相机|[teamworkPeripheral](../resources/teamworkperipheral.md) 集合|连接的相机列表。|
|defaultContentCamera|[teamworkPeripheral](../resources/teamworkperipheral.md)|配置的内容相机，用于共享会议中的模拟白板内容。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkCameraConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkCameraConfiguration",
  "contentCameraConfiguration": {
    "@odata.type": "microsoft.graph.teamworkContentCameraConfiguration"
  }
}
```

