---
title: bookingWorkHours 资源类型
description: 表示对于 bookingBusiness 或 bookingStaffMember，一周中一天的工作时间集合。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 959b9d1c325c4c765fc55e1d230b6ca480d01674
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525027"
---
# <a name="bookingworkhours-resource-type"></a>bookingWorkHours 资源类型

命名空间：microsoft.graph
 
表示对于 [bookingBusiness](bookingbusiness.md) 或 [bookingStaffMember，](bookingstaffmember.md)一周中一天的工作时间集合。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|day|String| 此实例表示的一周中的一天。 可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday` 或 `saturday`。|
|timeSlots|[bookingWorkTimeSlot](bookingworktimeslot.md) 集合|一天中的开始时间/结束时间列表。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingWorkHours"
}-->

```json
{
  "day": "String",
  "timeSlots": [{"@odata.type": "microsoft.graph.bookingWorkTimeSlot"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingWorkHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


