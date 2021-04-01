---
title: plannerPlanContextCollection 资源类型
description: '**plannerPlanContextCollection** 资源表示计划链接到的外部上下文的集合。 此资源是一个打开的类型，是 plannerPlan 对象的一部分。 属性值对中的值是 plannerPlanContext 对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: b2069fd30ba3beb6150b0fdc5dd5bb0f69956b82
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473596"
---
# <a name="plannerplancontextcollection-resource-type"></a>plannerPlanContextCollection 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


**plannerPlanContextCollection** 资源表示计划链接到的外部上下文的集合。 此资源是一个打开的类型，是 [plannerPlan 对象的一](plannerplan.md) 部分。 属性值对中的值是 [plannerPlanContext](plannerplancontext.md) 对象。


## <a name="properties"></a>属性
您可以定义此打开类型的属性。 属性值应该是唯一标识符，表示作为属性名称的外部上下文。 属性值必须为 [plannerPlanContext](plannerplancontext.md) 对象。 根据 OData 要求，开放类型中的属性名称不能包含下列字符 `.` `:` `%` `@` `#` ：、、。 这些字符需要使用 URL 编码进行编码。 若要删除收藏夹列表中的项目，将 属性的值设置为 `null` 。

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


