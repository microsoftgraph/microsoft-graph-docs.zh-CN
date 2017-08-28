# <a name="conversationthread-resource-type"></a>conversationThread 资源类型
conversationThread 是 [帖子](post.md) 集合。

最后一个帖子收件人集合聚合了整个线程的收件人。线程的收件人集合可以不断扩大。从线程中移除某个收件人时将创建一个新的线程。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出线程](../api/group_list_threads.md) | [conversationThread](conversationthread.md) 集合 |获取某个组的所有线程。|
|[创建线程](../api/group_post_threads.md) | [conversationThread](conversationthread.md) |通过首先创建一个线程，启动一个新对话。在组中创建新对话、对话线程和帖子。|
|[获取 conversationThread](../api/conversationthread_get.md) | [conversationThread](conversationthread.md) |获取属于某个组的特定线程。 |
|[更新](../api/conversationthread_update.md) | [conversationThread](conversationthread.md)  |更新 conversationThread 对象 |
|[删除](../api/conversationthread_delete.md) | 无 |删除 conversationThread 对象 |
|[答复](../api/conversationthread_reply.md)|无|通过新建 Post 实体答复此线程。|
|[列出帖子](../api/conversationthread_list_posts.md) |[帖子](post.md) 集合| 获取指定线程的帖子。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。|
|toRecipients|[recipient](recipient.md) collection|收件人：线程的收件人。|
|ccRecipients|[recipient](recipient.md) collection|抄送：线程的收件人。|
|topic|String|对话的主题。在创建对话时可设置此属性，但无法对其进行更新。||
|hasAttachments|Boolean|指示此线程中的任意帖子是否至少具有一个附件。|
|lastDeliveredDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`|
|uniqueSenders|String collection|向此线程发送邮件的所有用户。|
|preview|String|来自此对话中最新帖子的正文的简短摘要。|
|isLocked|Boolean|指示线程是否已锁定。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|posts|[帖子](post.md) 集合| 只读。可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversationThread"
}-->

```json
{
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "hasAttachments": true,
  "id": "string (identifier)",
  "isLocked": true,
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "topic": "string",
  "uniqueSenders": ["string"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
