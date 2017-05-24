# <a name="plannerplandetails-resource-type"></a>plannerPlanDetails 资源类型


**plannerPlanDetails** 资源表示计划的其他相关信息。每个[计划](plannerplan.md)对象均有一个详细信息对象。


### <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Get plannerPlanDetails](../api/plannerplandetails_get.md) | [plannerPlanDetails](plannerplandetails.md) |读取 **plannerPlanDetails** 对象的属性和关系。|
|[Update](../api/plannerplandetails_update.md) | [plannerPlanDetails](plannerplandetails.md)    |更新 **plannerPlanDetails** 对象。 |


### <a name="properties"></a>属性
| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|categoryDescriptions|[plannerCategoryDescriptions](plannercategorydescriptions.md)|指定可与计划中的任务相关联的六个类别的描述的对象|
|id|String| 只读。计划详细信息 ID。长度为 28 个字符，区分大小写。[格式验证](planner_identifiers_disclaimer.md)在服务上完成。|
|sharedWith|[plannerUserIds](planneruserids.md)|此计划共享的用户 id 集合。如果你正在利用 Office 365 组，使用组 API 管理组成员身份以共享[组的](group.md)计划。你还可以将现有的组成员添加到此集合，尽管他们无需访问组拥有的计划。 |

### <a name="relationships"></a>关系
无


### <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "id": "String (identifier)",
  "sharedWith": {"@odata.type": "microsoft.graph.plannerUserIds"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->