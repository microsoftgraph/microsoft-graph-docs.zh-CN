<a id="plannerchecklistitem-resource-type" class="xliff"></a>

# plannerChecklistItem 资源类型


**plannerChecklistItem** 资源表示任务的检查表中的项目。任务上的检查表由 [checklistItems 对象](plannerchecklistitems.md)表示。


<a id="properties" class="xliff"></a>

## 属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|isChecked|Boolean|如果已检查此项目，值则为 `true`，否则为 `false`。|
|lastModifiedBy|[identitySet](identityset.md)| 只读。上一次修改它的用户 ID。|
|lastModifiedDateTime|DateTimeOffset|只读。上一次修改它的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|orderHint|String|用于设置检查表中的项目的相对顺序。[此处](planner_order_hint_format.md)概述了此格式。|
|title|String|检查表项目的标题|

<a id="json-representation" class="xliff"></a>

## JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerChecklistItem"
}-->

```json
{
  "isChecked": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "orderHint": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->