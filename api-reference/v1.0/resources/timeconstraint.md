---
title: timeConstraint 资源类型
description: 根据指定的活动和打开时间段的性质, 将会议时间建议限制在一周的特定时间和几天。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7da2a3a2c712cdbe1fc3fb961781e35099a565d7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033612"
---
# <a name="timeconstraint-resource-type"></a>timeConstraint 资源类型

根据指定的活动和打开时间段的性质, 将会议时间建议限制在一周的特定时间和几天。

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
|activityDomain|activityDomain|（可选）会议性质。 可能的值是: `work`、 `personal`、 `unrestricted`或`unknown`。|
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
