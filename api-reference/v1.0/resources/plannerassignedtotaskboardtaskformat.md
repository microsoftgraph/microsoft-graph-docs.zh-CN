<a id="plannerassignedtotaskboardtaskformat-resource-type" class="xliff"></a>

# plannerAssignedToTaskBoardTaskFormat 资源类型

**plannerAssignedToTaskBoardTaskFormat** 资源表示用于在“任务板”的“AssignedTo”视图（由已向其分配任务的用户组成的视图）下正确呈现任务的信息。每个[任务](plannertask.md)均将有一个与其相关联的 **plannerAssignedToTaskBoardTaskFormat** 对象。


<a id="methods" class="xliff"></a>

## 方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Get plannerAssignedToTaskBoardTaskFormat](../api/plannerassignedtotaskboardtaskformat_get.md) | [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) |读取 **plannerAssignedToTaskBoardTaskFormat** 对象的属性和关系。|
|[Update](../api/plannerassignedtotaskboardtaskformat_update.md) | [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)  |更新 **plannerAssignedToTaskBoardTaskFormat** 对象。 |

<a id="properties" class="xliff"></a>

## 属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。资源的 ID。长度为 28 个字符，区分大小写。[格式验证](planner_identifiers_disclaimer.md)在服务上完成。|
|orderHintsByAssignee|[plannerOrderHintsByAssignee](plannerorderhintsbyassignee.md)|用于为任务板 AssignedTo 视图上的任务进行排序的提示字典。每个条目的键是任务分配到的用户之一，值为排序提示。[此处](planner_order_hint_format.md)概述了各值的格式。|
|unassignedOrderHint|字符串|当任务未分配给任何人，或 orderHintsByAssignee 字典未向分配到任务的用户提供排序提示时，提示值用于为任务板 AssignedTo 视图上的任务排序。[此处](planner_order_hint_format.md)概述了此格式。|

<a id="relationships" class="xliff"></a>

## 关系
无


<a id="json-representation" class="xliff"></a>

## JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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