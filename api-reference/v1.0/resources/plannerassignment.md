# <a name="plannerassignment-resource-type"></a>plannerAssignment 资源类型

**plannerAssignment** 资源表示针对用户的任务分配。该类型用于开放类型 [plannerAssignments](plannerassignments.md)。


### <a name="properties"></a>属性
| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|assignedBy|[identitySet](identityset.md)|执行任务分配的用户身份，即委派者。|
|assignedDateTime|DateTimeOffset|分配任务的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|orderHint|String|用于对任务中的代理人进行排序的提示。[此处](planner_order_hint_format.md)概述了此格式。|

### <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignment"
}-->

```json
{
  "assignedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "assignedDateTime": "String (timestamp)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->