---
title: plannerRecentPlanReference 资源类型
description: '**plannerRecentPlanReference** 资源类型表示对最近由用户查看的 plannerPlan 的引用。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 8a8fbf3ce9f39c49dde4bbeee96a3aab15a00077
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720975"
---
# <a name="plannerrecentplanreference-resource-type"></a>plannerRecentPlanReference 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**plannerRecentPlanReference** 资源类型表示对最近由用户查看的 [plannerPlan](plannerplan.md)的引用。 **用户的 plannerRecentPlanReferences** 由应用显式维护。 任何实现最近计划功能的应用都应记录用户上次查看计划时，并相应地更新 **plannerRecentPlanReference** 条目。
应用应注意 **plannerRecentPlanReference** 条目可以引用已删除、用户无法再访问或已使用其他标题更新的 **plannerPlans。**
我们建议应用在存在差异时通知用户，并保持条目最新。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|lastAccessedDateTime|DateTimeOffset|用户上次查看计划的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|planTitle|String|用户查看计划时计划的标题。|

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
  "suppressions": []
}
-->


