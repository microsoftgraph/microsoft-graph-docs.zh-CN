# <a name="planneruserids-resource-type"></a>plannerUserIds 资源类型

**plannerUserIds** 资源表示与其共享[计划](plannerplan.md)的用户 ID 列表。它是开放类型。如果你正在利用 Office 365 组，使用组 API 管理组成员身份以共享[组的](group.md)计划。你还可以将现有的组成员添加到此集合，尽管他们无需访问组拥有的计划。


### <a name="properties"></a>属性
开放类型的属性可以由客户端定义。在这种情况下，客户端应将用户 ID 作为属性，并且其值需为 `true` 布尔值。不再与用户 ID 共享时，则将属性值设置为 `false` 布尔值来自动删除属性。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUserIds"
}-->

```json
{
  "String-value": true
}
```

// 示例
```json
{
  "400723e1-102b-43aa-aba9-f35524827084": true, // property name is user id
  "f117339e-c914-4a9c-9b66-1c062b027556": true,
  "e886d105-23b9-47e2-bde1-757e75ee4a28": true
}

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUserIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->