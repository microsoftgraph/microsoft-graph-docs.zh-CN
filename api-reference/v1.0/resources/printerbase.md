---
title: printerBase 资源类型
description: 表示打印机和打印机共享的基本类型
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 12b611e73fab82d0ac1eafbdc19b26069ccfd94fa3806e4286da0f0c6516202b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235371"
---
# <a name="printerbase-resource-type"></a>printerBase 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

表示打印机和[printer 的基类型](printer.md)[Share](printerShare.md)实体类型。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|capabilities|[printerCapabilities](printercapabilities.md)|printer/printerShare 的功能。|
|defaults|[printerDefaults](printerdefaults.md)|printer/printerShare 的默认打印设置。|
|displayName|String|printer/printerShare 的名称。|
|id|String|标识符。|
|isAcceptingJobs|Boolean|打印机/打印机共享当前是否接受新的打印作业。|
|位置|[printerLocation](printerlocation.md)|打印机/printerShare 的物理和/或组织位置。|
|manufacturer|String|printer/printerShare 的制造商。|
|model|String|打印机/printerShare 的模型名称。|
|status|[printerStatus](printerstatus.md)|printer/printerShare 的处理状态，包括任何错误。|

## <a name="relationships"></a>关系
|关系|类型|说明|
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

