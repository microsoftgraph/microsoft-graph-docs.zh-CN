---
title: plannerAssignedToTaskBoardTaskFormat 资源类型
description: '**plannerAssignedToTaskBoardTaskFormat** 资源表示用于在任务板的 AssignedTo 视图中正确呈现任务的信息 (该视图由任务分配给) 的用户组织。 每个任务都有一个 **与之关联的 plannerAssignedToTaskBoardTaskFormat** 对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: ca256007f0e4b10fab53f814942736ead094555fef69b038c9680a8e08139303
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152325"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a>plannerAssignedToTaskBoardTaskFormat 资源类型

命名空间：microsoft.graph

**plannerAssignedToTaskBoardTaskFormat** 资源表示用于在任务板的 AssignedTo 视图中正确呈现任务的信息 (该视图由任务分配给) 的用户组织。 每个 [任务](plannertask.md) 都有一个 **与之关联的 plannerAssignedToTaskBoardTaskFormat** 对象。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 plannerAssignedToTaskBoardTaskFormat](../api/plannerassignedtotaskboardtaskformat-get.md) | [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) |读取 **plannerAssignedToTaskBoardTaskFormat 对象的属性和** 关系。|
|[更新](../api/plannerassignedtotaskboardtaskformat-update.md) | [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)  |更新 **plannerAssignedToTaskBoardTaskFormat** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。 资源的 ID。 长度为 28 个字符，区分大小写。 [格式验证](planner-identifiers-disclaimer.md)在服务上完成。|
|orderHintsByAssignee|[plannerOrderHintsByAssignee](plannerorderhintsbyassignee.md)|用于为任务板 AssignedTo 视图上的任务进行排序的提示字典。每个条目的键是任务分配到的用户之一，值为排序提示。[此处](planner-order-hint-format.md)概述了各值的格式。|
|unassignedOrderHint|字符串|当任务未分配给任何人，或 orderHintsByAssignee 字典未向分配到任务的用户提供排序提示时，用于为任务板 AssignedTo 视图上的任务进行排序的提示值。[此处](planner-order-hint-format.md)概述了此格式。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHintsByAssignee": {"@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"},
  "unassignedOrderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignedToTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

