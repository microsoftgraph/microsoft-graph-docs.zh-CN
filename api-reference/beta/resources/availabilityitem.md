---
title: availabilityItem 资源类型
description: 指示给定时间段的工作人员的状态。
author: kwekua
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 2b51fe3644fc6ca884d1eb4435a6b874f2293fa2
ms.sourcegitcommit: 19558bd9de9b717e7a36bfce1d6d84d0132e2697
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2022
ms.locfileid: "64755735"
---
# <a name="availabilityitem-resource-type"></a>availabilityItem 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指示给定时间段 [的工作人员](bookingstaffmember.md) 的状态。

## <a name="properties"></a>属性

| 属性  | 类型 |说明|
|:---------------|:--------|:----------|
|endDateTime |dateTimeTimeZone |时间段的结束时间。|
|服务 Id |String |指示 1：n 约会时的服务 ID。 如果约会类型为 1：n，则此字段将存在，否则 `null`。|
|状态 |bookingsAvailabilityStatus |工作人员的状态。 可取值为：`available`、`busy`、`slotsAvailable`、`outOfOffice`、`unknownFutureValue`。|
|startDateTime |dateTimeTimeZone |时间段的开始时间。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.availabilityItem"
}-->

``` json
{
  "endDateTime": "DateTimeInfo",
  "serviceId": "String",
  "status": "String",
  "startDateTime": "DateTimeInfo"
}
```
