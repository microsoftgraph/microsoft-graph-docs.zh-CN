# <a name="plannerplan-resource-type"></a>plannerPlan 资源类型

**plannerPlan** 资源表示 Office 365 中的计划。计划可以由[组](group.md)所有，并包含 [plannerTasks](plannerTask.md) 集合。其也可以有 [plannerBuckets](plannerBucket.md) 集合。每个计划对象具有可以包含此计划的更多信息的[详细信息](plannerPlanDetails.md)对象。有关组、计划和任务之间的关系的详细信息，请参阅 [Planner](planner_overview.md)。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Get plannerPlan](../api/plannerplan_get.md) | [plannerPlan](plannerplan.md) |读取 **plannerPlan** 对象的属性和关系。|
|[列出存储桶](../api/plannerplan_list_buckets.md) |[plannerBucket](plannerbucket.md) collection| 获取 **plannerBucket** 对象集合。|
|[List tasks](../api/plannerplan_list_tasks.md) |[plannerTask](plannertask.md) collection| 获取 **plannerTask** 对象集合。|
|[Update](../api/plannerplan_update.md) | [plannerPlan](plannerplan.md) |更新 **plannerPlan** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|createdDateTime|DateTimeOffset|只读。创建计划的日期和时间时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|id|String| 只读。 在计划的 ID。 它是 28 字符长度和区分大小写。 服务上执行[格式验证](planner_identifiers_disclaimer.md)。|
|owner|字符串|拥有计划的[组](group.md)ID。 此字段可以设置之前，必须存在有效的组。 设置后，无法更新此属性。|
|title|String|必填。计划的标题|
|createdBy|[identitySet](identityset.md)|只读。创建计划的用户。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|buckets|[plannerBucket](plannerbucket.md) collection| 只读。可为 Null。计划中的存储桶集合。|
|详细信息|[plannerPlanDetails](plannerplandetails.md)| 只读。可为 NULL。关于计划的其他详细信息。|
|tasks|[plannerTask](plannertask.md) collection| 只读。可为 Null。计划中的任务集合。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "owner": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->