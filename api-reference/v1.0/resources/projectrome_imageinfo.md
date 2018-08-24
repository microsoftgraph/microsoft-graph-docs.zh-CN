# <a name="imageinfo-resource-type"></a>imageInfo 资源类型

代表 [activity](../resources/projectrome_activity.md) 对象 [visualInfo](../resources/projectrome_visualinfo.md) 部分中 **attribution** 属性的复杂类型。

## <a name="properties"></a>属性

|名称 | 类型 | 说明|
|:----|:-----|:-----------|
|iconUrl | 字符串 | 可选；指向一个表示用于生成活动的应用程序图标的 URI|
|alternateText | 字符串 | 可选；图像的替换文字可访问内容|
|addImageQuery | 布尔 | 可选；用来指示服务器能否动态呈现图像以响应参数化的参数。 例如，一幅高对比度图像|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "iconUrl",
    "alternateText",
    "addImageQuery"
  ],
  "@odata.type": "microsoft.graph.imageInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.imageInfo",
    "iconUrl": "String (URL)",
    "alternateText": "String",
    "addImageQuery": "boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->