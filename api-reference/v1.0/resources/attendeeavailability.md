---
title: attendeeAvailability 资源类型
description: 与会者的出席情况。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3bcb4e113e1b0c5c132a8f152f59293930376b085fdeb3a0baf6c14af2bb274e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54238193"
---
# <a name="attendeeavailability-resource-type"></a>attendeeAvailability 资源类型

命名空间：microsoft.graph

与会者的出席情况。

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
|attendee|[attendeeBase](attendeebase.md)|与会者的电子邮件地址和类型 - 无论是人员还是资源，如果是人员，是必需还是可选。|
|availability|freeBusyStatus| 与会者的忙/闲状态。 可能的值包括 `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

