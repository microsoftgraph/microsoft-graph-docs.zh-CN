# <a name="thumbnail-resource-type"></a>thumbnail 资源类型

**缩略图**资源类型表示 OneDrive 上具有图形表示的图像、视频、文档、任何文件或文件夹的缩略图。

## <a name="properties"></a>属性

| 属性 | 类型   | 说明                                  |
|:---------|:-------|:---------------------------------------------|
| height   | Int32  | 缩略图高度，以像素为单位。      |
| url      | String | 用于提取缩略图内容的 URL。 |
| width    | Int32  | 缩略图宽度，以像素为单位。       |


## <a name="relationships"></a>关系

| 名称    | 类型   | 说明         |
|:--------|:-------|:--------------------|
| 内容 | 流 | 内容流。 |


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": ["content", "height", "width"],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "url": "string",
  "height": 1024,
  "width": 1024,
  "content": "stream"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "thumbnail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
