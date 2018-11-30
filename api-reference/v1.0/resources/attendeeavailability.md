---
title: attendeeAvailability 资源类型
description: 与会者的类型和忙/闲状态。
ms.openlocfilehash: 446dfb77d8f85021f41795038c3c1d597c6f1a6d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008451"
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
