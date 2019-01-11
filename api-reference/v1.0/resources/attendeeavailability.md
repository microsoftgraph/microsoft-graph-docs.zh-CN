---
title: attendeeAvailability 资源类型
description: 与会者的类型和忙/闲状态。
localization_priority: Normal
ms.openlocfilehash: a6dee994fc5eb3786fc1a432adcb9333bdb56ec8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834746"
---
# <a name="attendeeavailability-resource-type"></a>attendeeAvailability 资源类型

与会者的类型和忙/闲状态。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailability"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeBase"},
  "availability": "String"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|attendee|[AttendeeBase](attendeebase.md)|与会者类型，即是人员还是资源；如果是人员，是必需还是可选。|
|availability|freeBusyStatus| 可用性的与会者的状态。 可能的值为： `free`， `tentative`， `busy`， `oof`， `workingElsewhere`， `unknown`。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
