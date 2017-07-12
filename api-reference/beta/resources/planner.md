<a id="planner-resource-type" class="xliff"></a>

# planner 资源类型

**planner** 资源是 Planner 对象模型的入口点。其返回单一的 **planner** 资源。它不包含任何可用属性。


<a id="methods" class="xliff"></a>

## 方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Create plannerBucket](../api/planner_post_buckets.md) |[plannerBucket](plannerbucket.md)| 通过发布到存储桶集合新建 **plannerBucket**。|
|[Create plannerPlan](../api/planner_post_plans.md) |[plannerPlan](plannerplan.md)| 通过发布到计划集合新建 **plannerPlan**。|
|[Create plannerTask](../api/planner_post_tasks.md) |[plannerTask](plannertask.md)| 通过发布到任务集合新建 **plannerTask**。|

<a id="properties" class="xliff"></a>

## 属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。**planner** 资源的标识符|

<a id="relationships" class="xliff"></a>

## 关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|buckets|[plannerBucket](plannerbucket.md) collection| 只读。可为 NULL。返回指定存储桶的集合|
|plans|[plannerPlan](plannerplan.md) collection| 只读。可为 NULL。返回指定计划的集合|
|tasks|[plannerTask](plannertask.md) collection| 只读。可为 NULL。返回指定任务的集合|

<a id="json-representation" class="xliff"></a>

## JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->