---
title: staffAvailabilityItem 资源类型
description: 表示Microsoft Bookings工作人员的可用和繁忙时间段。
author: kwekua
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: fa6a7e856060209f274c0503d3c0c27f567ae910
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917764"
---
# <a name="staffavailabilityitem-resource-type"></a>staffAvailabilityItem 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示Microsoft Bookings[工作人员](bookingstaffmember.md)的可用和繁忙时间段。

## <a name="properties"></a>属性

| 属性  | 类型 |说明|
|:---------------|:--------|:----------|
|availabilityItems |[availabilityItem](availabilityitem.md) 集合 |此集合中的每个项都指示一个槽和工作人员的状态。|
|staffId |字符串 |工作人员的 ID。|

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
