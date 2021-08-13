---
title: shiftAvailability 资源类型
description: 计划工作的用户的可用性及其定期模式。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d1c75c5496df6e8d858be74b8001c57fe16de0b3d44a98d4229e1ad09ab77f8c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54174876"
---
# <a name="shiftavailability-resource-type"></a>shiftAvailability 资源类型

命名空间：microsoft.graph

要安排排班的用户的可用性及其定期模式。 [](shift.md)

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|recurrence|[patternedRecurrence](patternedrecurrence.md)| 指定定期模式 |
|timeSlots|[timeRange](timerange.md) 集合|时间段 (用户) 首选。|
|timeZone|String|指定指定时间时区。 |

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

