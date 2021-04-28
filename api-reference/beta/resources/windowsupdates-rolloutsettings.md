---
title: rolloutSettings 资源类型
description: 设置控制服务如何随着时间的推移部署更新。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 705eeae189d9159c07d3c115c77383a207eae6db
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067851"
---
# <a name="rolloutsettings-resource-type"></a>rolloutSettings 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

设置控制服务如何随着时间的推移部署更新。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|startDateTime|DateTimeOffset|部署中的设备开始接收更新的日期。 未设置时，一旦分配设备，部署就会开始。|
|devicesPerOffer|Int32| 指定同时提供的设备数。 设置 **endDateTime 时** 不起作用。 当 **未设置 endDateTime** 和 **devicesPerOffer** 时，将同时提供部署中所有设备的内容。|
|durationBetweenOffers|String|指定提供更新的每组设备之间的持续时间。 定义 **endDateTime 或** **devicesPerOffer 时** 有效。 默认值为 (`P1D` 1 天) 。|
|endDateTime|DateTimeOffset|指定向当前部署中所有设备提供更新的日期。 在此日期之后添加的设备将立即提供。 当 **未设置 endDateTime** 和 **devicesPerOffer** 时，将同时提供部署中所有设备的内容。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.rolloutSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.rolloutSettings",
  "startDateTime": "String",
  "durationBetweenOffers": "String",
  "endDateTime": "String (timestamp)",
  "devicesPerOffer": "Integer"
}
```

