# <a name="chartfont-resource-type"></a>ChartFont 资源类型

此对象表示 chart 对象的字体属性（字体名称、字体大小、颜色等）。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 ChartFont](../api/chartfont_get.md) | [ChartFont](chartfont.md) |读取 chartFont 对象的属性和关系。|
|[更新](../api/chartfont_update.md) | [ChartFont](chartfont.md)    |更新 ChartFont 对象。 |

## <a name="properties"></a>属性
| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|bold|boolean|表示字体的加粗状态。|
|color|string|文本颜色的 HTML 颜色代码表示。例如，#FF0000 表示红色。|
|italic|boolean|表示字体的斜体状态。|
|name|string|字体名称（例如"Calibri"）|
|大小|double|字体大小（例如 11）|
|underline|string|应用于字体的下划线类型。可能的值是：`None`、`Single`。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartFont"
}-->

```json
{
  "bold": true,
  "color": "string",
  "italic": true,
  "name": "string",
  "size": 1024,
  "underline": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->