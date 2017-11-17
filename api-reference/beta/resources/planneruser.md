<a id="planneruser-resource-type" class="xliff"></a>
# plannerUser 资源类型

**plannerUser** 资源提供[用户](user.md)的 Planner 资源的访问权限。它不包含任何可用属性。


<a id="methods" class="xliff"></a>
## 方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[List plans](../api/planneruser_list_plans.md) |[plannerPlan](plannerplan.md) collection| 获取 **plannerPlan** 对象集合。|
|[List tasks](../api/planneruser_list_tasks.md) |[plannerTask](plannertask.md) collection| 获取 **plannerTask** 对象集合。|

<a id="properties" class="xliff"></a>
## 属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|字符串| 只读。planenrUser 的标识符|

<a id="relationships" class="xliff"></a>
## 关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|plans|[plannerPlan](plannerplan.md) collection| 只读。可为 NULL。返回分配给用户的 [plannerTasks](plannertask.md)。|
|tasks|[plannerTask](plannertask.md) collection| 只读。可为 NULL。返回与用户共享的 [plannerPlans](plannerplan.md)。|

<a id="json-representation" class="xliff"></a>
## JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
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
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->