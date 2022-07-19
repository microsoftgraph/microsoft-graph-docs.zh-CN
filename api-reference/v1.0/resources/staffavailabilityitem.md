---
title: staffAvailabilityItem 资源类型
description: 表示 Bookings 员工的可用和繁忙时间段。
author: kwekua
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 2737d50eb65d0cdf4d0e44f3df76038968399f93
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856428"
---
# <a name="staffavailabilityitem-resource-type"></a>staffAvailabilityItem 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示Microsoft Bookings[工作人员](bookingstaffmember.md)的可用和繁忙时间段。

## <a name="properties"></a>属性

| 属性  | 类型 |Description|
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
  "availabilityItems": [{"@odata.type": "microsoft.graph.availabilityItem"}],
  "staffId": "String"
}
```