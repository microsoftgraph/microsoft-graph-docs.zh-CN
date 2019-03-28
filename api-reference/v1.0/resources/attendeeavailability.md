---
title: attendeeAvailability 资源类型
description: 与会者的可用性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 63014553824b833e2e4cdfb03485fcb7962c01a0
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/28/2019
ms.locfileid: "30936246"
---
# <a name="attendeeavailability-resource-type"></a>attendeeAvailability 资源类型

与会者的可用性。

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
|attendee|[attendeeBase](attendeebase.md)|电子邮件地址和与会者类型-无论是个人还是资源, 如果是个人或资源, 是必需的还是可选的。|
|availability|freeBusyStatus| 与会者的忙/闲状态。 可能的值为: `free`、 `tentative`、 `busy` `oof`、、 `workingElsewhere`、 `unknown`。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
