---
title: timeConstraint 资源类型
description: 根据活动的特定性质和开放时间段，将会议时间建议限制为某周的几个小时或几天。
localization_priority: Normal
ms.openlocfilehash: 88035d0617523c51bb01ee0a467e8c84785ad6aa
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643564"
---
# <a name="timeconstraint-resource-type"></a>timeConstraint 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

根据活动的特定性质和开放时间段，将会议时间建议限制为某周的几个小时或几天。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeconstraint"
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
|activityDomain|String|（可选）活动性质。可取值为：`work`、`personal`、`unrestricted` 或 `unknown`。|
|timeslots|[timeSlot](timeslot.md) 集合|一组时间段。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeconstraint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
