---
title: timeConstraint 资源类型
description: 根据指定的活动和开放时间段的性质，将会议时间建议限制为一周中的特定时段和日期。
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c7b5ed13c523fca24d9b8fad79f6271d4333177c7d2d0f2eece5354423ba370d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54221177"
---
# <a name="timeconstraint-resource-type"></a>timeConstraint 资源类型

命名空间：microsoft.graph

根据指定的活动和开放时间段的性质，将会议时间建议限制为一周中的特定时段和日期。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeConstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|activityDomain|activityDomain|（可选）会议性质。 可能的值是 `work` `personal` ：、、 `unrestricted` 或 `unknown` 。|
|timeslots|[timeSlot](timeslot.md) 集合|一组时间段。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

