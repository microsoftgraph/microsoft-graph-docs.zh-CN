---
title: availabilityItem 资源类型
description: 指示给定时间段的工作人员的状态。
author: kwekua
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: a4a95c8954ce2541a6096f8fd31fd87517143060
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856424"
---
# <a name="availabilityitem-resource-type"></a>availabilityItem 资源类型

命名空间：microsoft.graph

指示给定时间段 [的工作人员](bookingstaffmember.md) 的状态。

## <a name="properties"></a>属性

| 属性  | 类型 |Description|
|:---------------|:--------|:----------|
|endDateTime |dateTimeTimeZone |时间段的结束时间。|
|服务 Id |String |指示 1：n 约会时的服务 ID。 如果约会类型为 1：n，则此字段将存在，否则 `null`。|
|status |bookingsAvailabilityStatus |工作人员的状态。 可取值为：`available`、`busy`、`slotsAvailable`、`outOfOffice`、`unknownFutureValue`。|
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