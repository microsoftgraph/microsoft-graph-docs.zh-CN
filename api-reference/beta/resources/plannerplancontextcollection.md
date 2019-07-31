---
title: plannerPlanContextCollection 资源类型
description: '**PlannerPlanContextCollection**资源表示规划所链接到的外部上下文的集合。 此资源是打开的类型, 并且是 plannerPlan 对象的一部分。 属性-值对中的值是 plannerPlanContext 对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 34fecf604b68fe092e1feeac2c0e99cc0d59cd77
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965927"
---
# <a name="plannerplancontextcollection-resource-type"></a>plannerPlanContextCollection 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


**PlannerPlanContextCollection**资源表示规划所链接到的外部上下文的集合。 此资源是打开的类型, 并且是[plannerPlan](plannerplan.md)对象的一部分。 属性-值对中的值是[plannerPlanContext](plannerplancontext.md)对象。


## <a name="properties"></a>属性
您可以定义此开放类型的属性。 属性值应是表示外部上下文作为属性名称的独特标识符。 属性值必须是[plannerPlanContext](plannerplancontext.md)对象。 根据 OData 要求, 开放式类型中的属性名称不能包含以下字符: `.`、 `:`、 `%`、 `@`。 需要使用 URL 编码对这些字符进行编码。 若要删除收藏夹列表中的项, 请将该属性的值设置`null`为。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextCollection"
}-->

```json
{
  "48#19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype": {
    "@odata.type": "#microsoft.graph.plannerPlanContext",
    "associationType": "Board",
    "createdDateTime": "2015-10-14T00:57:28.4698344Z",
    "displayNameSegments": [
        "Finance Team",
        "Budget Plans"
    ],
    "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
