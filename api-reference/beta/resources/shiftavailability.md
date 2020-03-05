---
title: shiftAvailability 资源类型
description: 用户计划的工作及其定期模式的可用性。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8e06b64bc01be163149468c9090df2a8ea59497d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520623"
---
# <a name="shiftavailability-resource-type"></a>shiftAvailability 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

要安排的用户在[班次](shift.md)和定期模式中的可用性。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|recurrence|[patternedRecurrence](patternedrecurrence.md)| 指定定期模式 |
|因此|[timeRange](timerange.md)集合|用户首选的时隙（s）。|
|timeZone|String|指定所指定时间的时区。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.shiftAvailability",
  "baseType": null
}-->

```json
{
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "timeSlots": [{"@odata.type": "microsoft.graph.timeRange"}],
  "timeZone": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "shiftAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
