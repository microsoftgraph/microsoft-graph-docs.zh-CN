# <a name="automaticrepliesmailtips-resource-type"></a>automaticRepliesMailTips 资源类型


与已在邮箱上设置的任何自动答复有关的[邮件提醒](../resources/mailtips.md) 。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:-----|:-----|:-----|
| message | String | 自动回复消息。 |
| messageLanguage | [localeInfo](../resources/localeinfo.md) | 自动回复消息所使用的语言。 |
| scheduledEndTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | 设置自动答复结束的日期和时间。 |
| scheduledStartTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | 设置自动答复开始的日期和时间。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messageLanguage",
    "scheduledEndTime",
    "scheduledStartTime"
  ],
  "@odata.type": "microsoft.graph.automaticRepliesMailTips"
}-->

```json
{
  "message": "string",
  "messageLanguage": {"@odata.type": "microsoft.graph.localeInfo"},
  "scheduledEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->