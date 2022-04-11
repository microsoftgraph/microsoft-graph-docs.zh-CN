---
title: staffAvailabilityItem 资源类型
description: 表示Bookings工作人员的可用和繁忙时间段。
author: kwekua
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 5c130388ce2b728c22c467689b998ffe8673c718
ms.sourcegitcommit: 19558bd9de9b717e7a36bfce1d6d84d0132e2697
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2022
ms.locfileid: "64755729"
---
# <a name="staffavailabilityitem-resource-type"></a>staffAvailabilityItem 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示Bookings[工作人员](bookingstaffmember.md)的可用和繁忙时间段。

## <a name="properties"></a>属性

| 属性  | 类型 |说明|
|:---------------|:--------|:----------|
|availabilityItems |[availabilityItem](availabilityitem.md) 集合 |此集合中的每个项都指示一个槽和工作人员的状态。|
|staffId |String |工作人员的 ID。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.staffAvailabilityItem"
}-->

``` json
{
  "availabilityItems": "availabilityItem",
  "staffId": "String"
}
```
