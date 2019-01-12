---
title: plannerPlanContext 资源类型
description: '**PlannerPlanContext**资源表示 plannerPlan 计划程序之外的用户体验的关系。 可以在其他体验，如 Microsoft 团队，来跟踪工作的用户体验的上下文中显示计划程序中的计划。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: e118e32ea74332f0d8d0f958f7c55cd9980acb8f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962889"
---
# <a name="plannerplancontext-resource-type"></a>plannerPlanContext 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

**PlannerPlanContext**资源表示[plannerPlan](plannerplan.md)计划程序之外的用户体验的关系。 可以在其他体验，如 Microsoft 团队，来跟踪工作的用户体验的上下文中显示计划程序中的计划。
可以基于**ownerAppId**属性标识**plannerPlanContext**条目 reresents 的体验：
 - 5e3ce6c0-2b1f-4285-8d4b-75ee78787346： 上下文项目所属的 Microsoft 团队。
 - 00000003-0000-0ff1-ce00-000000000000： 上下文项目属于 SharePoint。

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|associationType|字符串|可为 Null。 [PlannerPlan](plannerplan.md)和应用程序之间的关联的应用程序定义的类型。 应用程序可以使用此信息来跟踪对同一[plannerPlan](plannerplan.md)不同类型的关系。|
|createdDateTime|DateTimeOffset|此为只读属性。 日期和时间创建**plannerPlanContext**时。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|displayNameSegments|String 集合|线段的外部体验的名称。 段表示允许其他应用程序，以显示关系的层次结构。|
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
