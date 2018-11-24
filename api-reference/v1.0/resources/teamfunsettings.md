# <a name="teamfunsettings-resource-type"></a>teamFunSettings 资源类型



要配置的设置使用 Giphy、 memes 和[团队](team.md)中的标签。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowGiphy|布尔|如果设置为 true，则启用 Giphy 使用。|
|giphyContentRating|字符串 (enum)|Giphy 内容评级。 可取值为：`moderate`、`strict`。|
|allowStickersAndMemes|布尔|如果设置为 true，使用户能够包括标签和 memes。|
|allowCustomMemes|布尔|如果设置为 true，使用户能够包括自定义 memes。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamFunSettings"
}-->

```json
{
  "allowGiphy": true,
  "giphyContentRating": "strict",
  "allowStickersAndMemes": true,
  "allowCustomMemes": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
