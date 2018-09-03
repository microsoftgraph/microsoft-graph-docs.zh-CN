# <a name="plannertaskdetails-resource-type"></a>plannerTaskDetails 资源类型

**plannerTaskDetails** 资源表示任务的其他相关信息。每个[任务](plannertask.md)对象均有一个详细信息对象。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 plannerTaskDetails](../api/plannertaskdetails_get.md) | [plannerTaskDetails](plannertaskdetails.md) |读取 **plannerTaskDetails** 对象的属性和关系。|
|[更新](../api/plannertaskdetails_update.md) | [plannerTaskDetails](plannertaskdetails.md)    |更新 **plannerTaskDetails** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|列表框|[plannerChecklistItems](plannerchecklistitems.md)|任务上的检查表项目集合。|
|说明|字符串|任务描述|
|id|字符串| 只读。 任务详细信息的 ID。 长度为 28 个字符，区分大小写。 [格式验证](planner_identifiers_disclaimer.md) 由服务执行。|
|previewType|字符串|这将设置显示任务的预览类型。 可能的值为： `automatic` 、 `noPreview` 、 `checklist` 、 `description` 、 `reference` 。 当设置为 `automatic` 查看任务应用程序所选择的预览显示。|
|参考|[plannerExternalReferences](plannerexternalreferences.md)|任务上的引用集合。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
