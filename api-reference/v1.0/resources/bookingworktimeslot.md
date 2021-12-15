---
title: bookingWorkTimeSlot 资源类型
description: 定义工作的开始时间和结束时间。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 119062c301844f297a57c47829ffab4465ea4ec4
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525106"
---
# <a name="bookingworktimeslot-resource-type"></a>bookingWorkTimeSlot 资源类型

命名空间：microsoft.graph

定义工作的开始时间和结束时间。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|endTime|TimeOfDay|一天中停止工作的时间。 例如，17：00：00.0000000。|
|startTime|TimeOfDay|一天中工作开始的时间。 例如，08：00：00.0000000。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingWorkTimeSlot"
}-->

```json
{
  "endTime": "String (timestamp)",
  "startTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingWorkTimeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


