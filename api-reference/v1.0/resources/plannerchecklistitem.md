---
title: plannerChecklistItem 资源类型
description: '**PlannerChecklistItem**资源表示任务清单中的项。 任务上的检查表由 checklistItems 对象表示。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 4d4762a9ca4aee30b32e6810dfb7ffd14451ed92
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037519"
---
# <a name="plannerchecklistitem-resource-type"></a>plannerChecklistItem 资源类型

命名空间：microsoft.graph


**PlannerChecklistItem**资源表示任务清单中的项。 任务上的检查表由 [checklistItems 对象](plannerchecklistitems.md)表示。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|isChecked|Boolean|Value 是 `true` 选中该项时为， `false` 否则为。|
|lastModifiedBy|[identitySet](identityset.md)| 只读。 上次修改此 ID 的用户 ID。|
|lastModifiedDateTime|DateTimeOffset|只读。 上次修改的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|orderHint|String|用于设置清单中项的相对顺序。 格式[定义如下所示。](planner-order-hint-format.md)|
|title|String|检查表项的标题|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerChecklistItem"
}-->

```json
{
  "isChecked": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "orderHint": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

