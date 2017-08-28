# <a name="provisionedplan-resource-type"></a>provisionedPlan 资源类型

[用户](user.md) 实体和 [组织](organization.md) 实体的 **provisionedPlans** 属性都是一个 **provisionedPlan** 集合。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|capabilityStatus|String|例如，“Enabled”。|
|provisioningStatus|String|例如，“Success”。|
|service|String|服务名称；例如，“AccessControlS2S”|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedplan"
}-->

```json
{
  "capabilityStatus": "string",
  "provisioningStatus": "string",
  "service": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->