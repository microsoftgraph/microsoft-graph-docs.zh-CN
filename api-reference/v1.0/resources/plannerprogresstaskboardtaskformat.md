---
title: plannerProgressTaskBoardTaskFormat 资源类型
description: '**plannerProgressTaskBoardTaskFormat** 资源表示用于在“任务板”的“进度”视图（由任务对象上的 PercentComplete 字段的状态组成的视图，包含“未启动”、“正在进行”和“完成”列）下正确呈现任务的信息。每个任务均将有一个与其相关联的 **plannerProgressTaskBoardTaskFormat** 对象。'
ms.openlocfilehash: 90ac4daa3d6b37f054c00df042de48d4c7706a96
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011117"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a>plannerProgressTaskBoardTaskFormat 资源类型

**plannerProgressTaskBoardTaskFormat** 资源表示用于在“任务板”的“进度”视图（由任务对象上的 PercentComplete 字段的状态组成的视图，包含“未启动”、“正在进行”和“完成”列）下正确呈现任务的信息。每个[任务](plannertask.md)均将有一个与其相关联的 **plannerProgressTaskBoardTaskFormat** 对象。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Get plannerProgressTaskBoardTaskFormat](../api/plannerprogresstaskboardtaskformat-get.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md) |读取 **plannerProgressTaskBoardTaskFormat** 对象的属性和关系。|
|[Update](../api/plannerprogresstaskboardtaskformat-update.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)    |更新 **plannerProgressTaskBoardTaskFormat** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。 资源的 ID。 它是 28 字符长度和区分大小写。 服务上执行[格式验证](planner-identifiers-disclaimer.md)。|
|orderHint|String|用于对任务板进度视图上的任务进行排序的提示值。[此处](planner-order-hint-format.md)概述了此格式。|

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