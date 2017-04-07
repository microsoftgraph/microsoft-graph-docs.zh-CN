# <a name="recurrencerange-resource-type"></a>recurrenceRange 资源类型

事件的持续时间。

## <a name="properties"></a>属性

| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|endDate|日期|系列的结束日期。|
|numberOfOccurrences|Int32|事件重复发生的次数。|
|recurrenceTimeZone|String |**startDate** 和 **endDate** 属性的时区。 |
|startDate|日期|序列的开始日期。|
|type|String|定期区域：EndDate = 0，NoEnd = 1，Numbered = 2。可能的值是：`EndDate`、`NoEnd`、`Numbered`。||


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrencerange"
}-->

```json
{
  "endDate": "String (timestamp)",
  "numberOfOccurrences": 1024,
  "recurrenceTimeZone": "string",
  "startDate": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recurrenceRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
