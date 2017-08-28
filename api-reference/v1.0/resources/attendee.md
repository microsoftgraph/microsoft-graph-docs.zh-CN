# <a name="attendee-resource-type"></a>与会者资源类型

会议与会者。

由 [attendeeBase](attendeebase.md) 派生。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|状态|[ResponseStatus](responsestatus.md)|事件与会者的响应（无、接受、拒绝等）和发送响应的日期时间。|
|类型|String|与会者类型：`Required`、`Optional`、`Resource`。|
|emailAddress|[emailAddress](emailAddress.md)|添加与会者姓名和 SMTP 地址。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendee"
}-->

```json
{
  "status": {"@odata.type": "microsoft.graph.responseStatus"},
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->