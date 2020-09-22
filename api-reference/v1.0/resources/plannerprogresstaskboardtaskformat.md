---
title: plannerProgressTaskBoardTaskFormat 资源类型
description: '**PlannerProgressTaskBoardTaskFormat**资源表示用于在任务板的 "进度" 视图中按任务对象的 "百分比" 字段组织的视图（包含未启动的列、"正在进行" 和 "完成") ）在任务 (板的 "进度" 视图中正确呈现任务的信息。 每个任务都有一个与之关联的 **plannerProgressTaskBoardTaskFormat** 对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 0c08fed11b53610c06b27b9fa9d5e898b2f0620d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037360"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a>plannerProgressTaskBoardTaskFormat 资源类型

命名空间：microsoft.graph

**PlannerProgressTaskBoardTaskFormat**资源表示用于在任务板的 "进度" 视图中按任务对象的 "百分比" 字段组织的视图（包含未启动的列、"正在进行" 和 "完成") ）在任务 (板的 "进度" 视图中正确呈现任务的信息。 每个 [任务](plannertask.md) 都有一个与之关联的 **plannerProgressTaskBoardTaskFormat** 对象。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 plannerProgressTaskBoardTaskFormat](../api/plannerprogresstaskboardtaskformat-get.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md) |读取 **plannerProgressTaskBoardTaskFormat** 对象的属性和关系。|
|[更新](../api/plannerprogresstaskboardtaskformat-update.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)    |更新 **plannerProgressTaskBoardTaskFormat** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。 资源的 ID。 长度为 28 个字符，区分大小写。 [格式验证](planner-identifiers-disclaimer.md)在服务上完成。|
|orderHint|String|用于为任务板“进度”视图上的任务进行排序的提示值。[此处](planner-order-hint-format.md)概述了此格式。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

