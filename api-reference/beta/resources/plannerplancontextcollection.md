---
title: plannerPlanContextCollection 资源类型
description: '**PlannerPlanContextCollection**资源表示的外部上下文计划链接到的集合。 此资源是开放的类型，plannerPlan 对象的一部分。 属性值对中的值是 plannerPlanContext 对象。'
localization_priority: Normal
ms.openlocfilehash: 51a09353993a61324f31a03c8ffadd5462cac692
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805451"
---
# <a name="plannerplancontextcollection-resource-type"></a>plannerPlanContextCollection 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。


**PlannerPlanContextCollection**资源表示的外部上下文计划链接到的集合。 此资源是开放的类型， [plannerPlan](plannerplan.md)对象的一部分。 属性值对中的值是[plannerPlanContext](plannerplancontext.md)对象。


## <a name="properties"></a>属性
您可以定义此打开类型的属性。 属性值应为独特标识符值，该值代表外部上下文与属性名称。 属性值必须是[plannerPlanContext](plannerplancontext.md)对象。 基于 OData 要求，在打开的类型的属性名称不能包含下列字符： `.`， `:`， `%`， `@`。 需要使用 URL 编码进行编码这些字符。 在收藏夹列表中删除项目，设置对属性的值`null`。

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContextCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
