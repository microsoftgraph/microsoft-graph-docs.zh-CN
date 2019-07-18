---
title: plannerPlanContext 资源类型
description: '**PlannerPlanContext**资源表示 PlannerPlan 在计划程序外的用户体验的关系。 Planner 中的计划可以在其他体验 (如 Microsoft 团队) 中进行, 以在该体验的上下文中跟踪工作。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 443331ef12469436e10f63a4311bfea0547be6fd
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778647"
---
# <a name="plannerplancontext-resource-type"></a>plannerPlanContext 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**PlannerPlanContext**资源表示[plannerPlan](plannerplan.md)在计划程序外的用户体验的关系。 Planner 中的计划可以在其他体验 (如 Microsoft 团队) 中进行, 以在该体验的上下文中跟踪工作。
可以基于**ownerAppId**属性来标识**plannerPlanContext**条目 reresents 的体验:
- 5e3ce6c0-2b1f-4285-8d4b-75ee78787346: 上下文条目属于 Microsoft 团队。
- 为 00000003-0000-0ff1-ce00-000000000000: 上下文条目属于 SharePoint。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|associationType|String|可为 Null。 [PlannerPlan](plannerplan.md)与应用之间的应用程序定义类型的关联。 应用程序可以使用此信息跟踪与同一[plannerPlan](plannerplan.md)的不同类型的关系。|
|createdDateTime|DateTimeOffset|只读。 **PlannerPlanContext**的创建日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|displayNameSegments|String collection|外部体验名称的各个部分。 段表示允许其他应用显示关系的层次结构。|
|ownerAppId|String|只读。 创建**plannerPlanContext**的应用程序的 ID。|

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
