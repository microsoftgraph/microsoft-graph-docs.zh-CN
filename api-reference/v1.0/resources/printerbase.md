---
title: printerBase 资源类型
description: 表示打印机和打印机共享的基本类型
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 515c14bb4de7352a8c17cffdacbd7a4c9091fc70
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516946"
---
# <a name="printerbase-resource-type"></a>printerBase 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

表示打印机和[printerShare](printer.md) [](printerShare.md)实体类型的基本类型。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|capabilities|[printerCapabilities](printercapabilities.md)|printer/printerShare 的功能。|
|defaults|[printerDefaults](printerdefaults.md)|printer/printerShare 的默认打印设置。|
|displayName|String|printer/printerShare 的名称。|
|id|String|标识符。|
|isAcceptingJobs|Boolean|打印机/打印机共享当前是否接受新的打印作业。|
|位置|[printerLocation](printerlocation.md)|打印机/printerShare 的物理和/或组织位置。|
|manufacturer|String|打印机/printerShare 的制造商。|
|model|String|打印机/printerShare 的模型名称。|
|状态|[printerStatus](printerstatus.md)|打印机/printerShare 的处理状态，包括任何错误。|

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|jobs|[printJob](printjob.md) 集合|由打印机/printerShare 排入打印队列的作业列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printerBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerBase",
  "id": "String (identifier)",
  "displayName": "String",
  "manufacturer": "String",
  "model": "String",
  "isAcceptingJobs": "Boolean",
  "defaults": {
    "@odata.type": "microsoft.graph.printerDefaults"
  },
  "location": {
    "@odata.type": "microsoft.graph.printerLocation"
  },
  "capabilities": {
    "@odata.type": "microsoft.graph.printerCapabilities"
  },
  "status": {
    "@odata.type": "microsoft.graph.printerStatus"
  }
}
```

