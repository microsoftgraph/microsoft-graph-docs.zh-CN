---
title: plannerProgressTaskBoardTaskFormat 资源类型
description: '**plannerProgressTaskBoardTaskFormat** 资源表示用于在任务板 (的"进度"视图中正确呈现任务的信息 (该视图按任务对象上"PercentComplete"字段的状态组织，包含"未启动"、正在进行和完成) 的列。 每个任务都有一个 **与之关联的 plannerProgressTaskBoardTaskFormat** 对象。'
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 0288b8c5ef99f4e72f019c6ffaee15bfe1022348
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59052935"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a>plannerProgressTaskBoardTaskFormat 资源类型

命名空间：microsoft.graph

**plannerProgressTaskBoardTaskFormat** 资源表示用于在任务板 (的"进度"视图中正确呈现任务的信息 (该视图按任务对象上"PercentComplete"字段的状态组织，包含"未启动"、正在进行和完成) 的列。 每个 [任务](plannertask.md) 都有一个 **与之关联的 plannerProgressTaskBoardTaskFormat** 对象。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 plannerProgressTaskBoardTaskFormat](../api/plannerprogresstaskboardtaskformat-get.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md) |读取 **plannerProgressTaskBoardTaskFormat 对象的属性和** 关系。|
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

