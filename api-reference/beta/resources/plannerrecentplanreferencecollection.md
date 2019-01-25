---
title: plannerRecentPlanReferenceCollection 资源类型
description: '**PlannerRecentPlanReferenceCollection**资源代表最近已由用户查看的计划对引用的集合。 此资源是开放的类型，plannerUser 对象的一部分。 属性名称是相应计划的 ID。 属性值对中的值是 plannerRecentPlanReference 对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: e27375e3f2395b3528873d8b83f0b5aa6f48d52e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514990"
---
# <a name="plannerrecentplanreferencecollection-resource-type"></a>plannerRecentPlanReferenceCollection 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**PlannerRecentPlanReferenceCollection**资源代表最近已由用户查看的计划对引用的集合。 此资源是开放的类型， [plannerUser](planneruser.md)对象的一部分。 属性名称是相应计划的 ID。 属性值对中的值是[plannerRecentPlanReference](plannerrecentplanreference.md)对象。
集合的大小超过预先确定的最大值时，添加对新引用此集合将自动删除最早的项。


## <a name="properties"></a>属性
您可以定义此打开类型的属性。 属性名称是`id` [plannerPlan](plannerplan.md)资源的值和它们的值必须是[plannerRecentPlanReference](plannerrecentplanreference.md)对象。 在收藏夹列表中删除项目，设置对属性的值`null`。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerRecentPlanReferenceCollection"
}-->

```json
{
  "7oTB5aMIAE2rVo-1N-L7RmQAGX2q": {
    "@odata.type": "microsoft.graph.plannerRecentPlanReference",
    "lastAccessedDateTime": "2017-12-02T22:49:46.155Z",
    "planTitle": "Purchase Workflow"
  },
  "iKNMHkk3vEWpSF7F7iZWIGQAAMMw": {
    "@odata.type": "microsoft.graph.plannerRecentPlanReference",
    "lastAccessedDateTime": "2017-12-03T21:59:28.975Z",
    "planTitle": "New Year's Office Party"
  }
}
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerRecentPlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerrecentplanreferencecollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
