---
title: plannerRecentPlanReference 资源类型
description: '**PlannerRecentPlanReference**资源类型代表最近已由用户查看 plannerPlan 的引用。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 55ccf34055d7d181dbbeecd5b6c30a3843f211d5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509159"
---
# <a name="plannerrecentplanreference-resource-type"></a>plannerRecentPlanReference 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**PlannerRecentPlanReference**资源类型代表最近已由用户查看[plannerPlan](plannerplan.md)的引用。 **PlannerRecentPlanReferences**用户明确维护应用程序中。 用户上次查看的计划和更新**plannerRecentPlanReference**条目相应时，应记录实现最新的计划功能任何应用程序。
应用程序应注意**plannerRecentPlanReference**条目可以引用**plannerPlans**的被删除，用户不再可以访问，或已更新具有不同的标题。
建议的应用程序差异时通知用户，并保持最新条目。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|lastAccessedDateTime|DateTimeOffset|日期和时间计划上次查看的用户。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|planTitle|String|标题时计划的用户查看它。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerRecentPlanReference"
}-->

```json
{
  "lastAccessedDateTime": "String (timestamp)",
  "planTitle": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerRecentPlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerrecentplanreference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
