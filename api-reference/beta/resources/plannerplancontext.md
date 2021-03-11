---
title: plannerPlanContext 资源类型
description: '**plannerPlanContext** 资源表示 plannerPlan 与 Planner 之外的用户体验的关系。 Planner 中的计划可以显示在其他体验（如 Microsoft Teams）中，以跟踪该体验上下文中的工作。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: f8a3b82c35339bb8bc6b3d3d7923b41ed97ecc02
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720982"
---
# <a name="plannerplancontext-resource-type"></a>plannerPlanContext 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**plannerPlanContext** 资源表示 [plannerPlan](plannerplan.md)与 Planner 之外的用户体验的关系。 Planner 中的计划可以显示在其他体验（如 Microsoft Teams）中，以跟踪该体验上下文中的工作。 [plannerPlanContextDetails](plannerplancontextdetails.md)中具有外部链接的体验可以显示在用户界面中，从而允许用户访问这些体验。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|associationType|String|可为 NULL。 plannerPlan 与应用之间的应用定义的关联[](plannerplan.md)类型。 应用可以使用此信息跟踪与同一 [plannerPlan 的不同类型的关系](plannerplan.md)。|
|createdDateTime|DateTimeOffset|只读。 创建 **plannerPlanContext 的** 日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|displayNameSegments|字符串集合|外部体验名称的段。 分段表示允许其他应用显示关系的分层结构。|
|isCreationContext|Boolean|只读。 指示是否从指定上下文创建计划。 根据上下文是否指定为计划创建一部分而自动生成。|
|ownerAppId|String|只读。 创建 **plannerPlanContext** 的应用的 ID。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContext"
}-->

```json
{
  "associationType": "Board",
  "createdDateTime": "2015-10-14T00:57:28.4698344Z",
  "displayNameSegments": [
    "Finance Team",
    "Budget Plans"
  ],
  "isCreationContext": false,
  "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


