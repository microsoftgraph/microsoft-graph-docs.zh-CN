# <a name="recurrencepattern-resource-type"></a>recurrencePattern 资源类型

事件发生的频率。


## <a name="properties"></a>属性
| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|dayOfMonth|Int32|事件发生的日期。|
|daysOfWeek|String collection|事件发生的星期几的集合。可能的值是：`Sunday`、`Monday`、`Tuesday`、`Wednesday`、`Thursday`、`Friday`、`Saturday`。|
|firstDayOfWeek|String|定期开始的星期几。可能的值是：`Sunday`、`Monday`、`Tuesday`、`Wednesday`、`Thursday`、`Friday`、`Saturday`。|
|index|String|定期发生的星期的索引：`First`、`Second`、`Third`、`Fourth`、`Last`。|
|interval|Int32|两次发生之间的指定定期类型的单位数量。|
|month|Int32|事件发生的月份。这是一个 1 到 12 的数字。|
|type|String|定期模式类型是：`Daily`、`Weekly`、`AbsoluteMonthly`、`RelativeMonthly`、`AbsoluteYearly`、`RelativeYearly`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrencepattern"
}-->

```json
{
  "dayOfMonth": 1024,
  "daysOfWeek": ["String"],
  "firstDayOfWeek": "String",
  "index": "String",
  "interval": 1024,
  "month": 1024,
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recurrencePattern resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->