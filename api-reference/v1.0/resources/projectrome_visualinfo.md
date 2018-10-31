# <a name="visualinfo-resource-type"></a>visualInfo 资源类型

代表 activity 对象中 **visual ** Elements[ visualElements](../resources/projectrome_activity.md) 属性的复杂类型。

每个用户活动都将作为自适应卡片在日程表中显示。 鼓励应用程序开发人员提供自定义卡片，用于捕获应用程序中发生的活动的本质。 这可以通过在内容属性中提供自定义 JSON 卡来实现。

除了具有自适应卡的可视元数据，应用还可以指定内容元数据，该数据可用于根据用户活动生成推断，以此提供可用于未来重新使用的新活动。 可通过使用活动的 contentInfo 属性提供一个 JSON 对象来实现，该 JSON 对象利用 schema.org 属性描述内容。

如果未提供自定义卡片，则使用 displayText 和说明属性生成简单卡片。 建议使用自定义卡片展示应用程序中的最佳内容。

## <a name="properties"></a>属性

|名称 | 类型 | 说明|
|:----|:------|:-----------|
|displayText | String | 必需。 用户唯一活动的简短文本说明（例如，在活动引用文档创建的情况下的文档名称）|
|description | 字符串 | 可选。 用户唯一活动的详细文本说明（例如，文档名称、第一句和/或元数据）|
|backgroundColor | String | 可选。 用于在 UI 中呈现活动的背景颜色 - 活动的应用程序源中的品牌颜色。 必须是有效的十六进制颜色|
|content | 无类型的 JSON 对象 | 可选。 自定义的数据 - 用于提供自定义内容，以在 Windows  Shell UI 中呈现活动的 JSON 对象|
|attribution | [imageInfo](../resources/projectrome_imageinfo.md) | 可选。 JSON 对象，用于表示一个图标，代表用于生成活动的应用程序|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attribution",
    "description",
    "backgroundColor",
    "content"
  ],
  "@odata.type": "microsoft.graph.visualInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.visualInfo",
    "attribution": {
        "@odata.type": "microsoft.graph.imageInfo",
        "iconUrl": "String (URL)",
        "alternateText": "String",
        "addImageQuery": "boolean"
    },
    "description": "String",
    "backgroundColor": "String",
    "displayText": "String",
    "content": {
        "@odata.type": "microsoft.graph.Json"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "visualinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
