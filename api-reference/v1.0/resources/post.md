# <a name="post-resource-type"></a>帖子资源类型
表示 [conversationThread](conversationthread.md) 实体中的各个帖子项。

即使无法显式创建帖子，也可以执行以下任一操作来创建帖子：

- [答复现有帖子](../api/post_reply.md) 
- [答复现有线程](../api/conversationthread_reply.md) 
- [在新对话中创建线程](../api/group_post_threads.md)
- [创建新对话](../api/group_post_conversations.md)

通过该资源可以使用[扩展](../../../concepts/extensibility_overview.md)将自己的数据添加到自定义属性。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出帖子](../api/conversationthread_list_posts.md) | [帖子](post.md) |获取指定线程的帖子。 |
|[获取帖子](../api/post_get.md) | [帖子](post.md) |获取指定的线程中帖子的属性和关系。|
|[答复](../api/post_reply.md)|无|在组对话中答复帖子，并向指定线程中添加新帖子。|
|[转发](../api/post_forward.md)|无|将帖子转发给收件人。|
|**Attachments**| | |
|[列出附件](../api/post_list_attachments.md) |[attachment](attachment.md) 集合| 获取帖子的所有附件。|
|[Add attachment](../api/post_post_attachments.md) |[attachment](attachment.md)| 将附件添加到帖子中。 |
|**开放扩展**| | |
|[创建开放扩展](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并在新建或现有的资源实例中添加自定义属性。|
|[获取开放扩展](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取通过名称或完全限定的名称识别的一个或多个开放扩展对象。|
|**扩展属性**| | |
|[创建单值扩展属性](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[帖子](post.md)  |在新建或现有帖子中创建一个或多个单值扩展属性。   |
|[获取具有单值扩展属性的帖子](../api/singlevaluelegacyextendedproperty_get.md)  | [帖子](post.md) | 通过使用 `$expand` or `$filter` 获取包含单值扩展属性的帖子。 |
|[创建多值扩展属性](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [帖子](post.md) | 在新建或现有的帖子中创建一个或多个多值扩展属性。  |
|[获取具有多值扩展属性的帖子](../api/multivaluelegacyextendedproperty_get.md)  | [帖子](post.md) | 使用 `$expand` 获取包含一个多值扩展属性的帖子。 |

## <a name="properties"></a>属性
| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|body|[itemBody](itembody.md)|帖子的内容。这是默认属性。此属性可为 NULL。|
|类别|String collection|与帖子关联的类别。|
|changeKey|String|标识帖子的版本。每次帖子更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。|
|conversationId|String|对话的唯一 ID。只读。|
|conversationThreadId|String|对话线程的唯一 ID。只读。|
|createdDateTime|DateTimeOffset|创建帖子时指定。DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`|
|from|[recipient](recipient.md)|在委派访问方案中使用。指示代表另一用户发布了此邮件的帐户。这是默认属性。|
|hasAttachments|Boolean|指示帖子是否具有至少一个附件。这是默认属性。|
|id|String| 只读。|
|lastModifiedDateTime|DateTimeOffset|帖子上次修改时指定。DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`|
|newParticipants|[recipient](recipient.md) collection|添加到此线程作为帖子一部分的对话参与者。|
|receivedDateTime|DateTimeOffset|接收到帖子时指定。DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`|
|sender|[recipient](recipient.md)|包含发件人的地址未指定发件人时，发件人的值假定为已经过验证身份的用户的地址。这是默认属性。|

## <a name="relationships"></a>关系
| 关系 | 类型    |说明|
|:---------------|:--------|:----------|
|attachments|[附件](attachment.md) 集合| 只读。可为 NULL。|
|extensions|[扩展](extension.md)集合|为帖子定义的开放扩展集合。只读。可为 NULL。|
|inReplyTo|[帖子](post.md)| 只读。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合| 为帖子定义的多值扩展属性的集合。只读。可为 NULL。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| 为帖子定义的单值扩展属性的集合。只读。可为 NULL。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "inReplyTo",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.post"
}-->

```json
{
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "categories": ["string"],
  "changeKey": "string",
  "conversationId": "string",
  "conversationThreadId": "string",
  "createdDateTime": "String (timestamp)",
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "newParticipants": [{"@odata.type": "microsoft.graph.recipient"}],
  "receivedDateTime": "String (timestamp)",
  "sender": {"@odata.type": "microsoft.graph.recipient"}
}

```

## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](../../../concepts/extensibility_overview.md)
- [使用开放扩展向用户添加自定义数据（预览）](../../../concepts/extensibility_open_users.md)
- [使用架构扩展向组添加自定义数据（预览）](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
