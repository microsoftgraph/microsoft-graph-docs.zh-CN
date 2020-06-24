---
title: conversationThread 资源类型
description: conversationThread 是 帖子 集合。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 8608ea72c8c136b54f94c73f99ca0f79fbc7ec0b
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845265"
---
# <a name="conversationthread-resource-type"></a>conversationThread 资源类型

命名空间：microsoft.graph

conversationThread 是 [帖子](post.md) 集合。

The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients.
A new thread is created when a recipient is removed from the thread.

## <a name="methods"></a>Methods

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出线程](../api/group-list-threads.md) | [conversationThread](conversationthread.md) 集合 |获取组的所有线程。|
|[创建线程](../api/group-post-threads.md) | [conversationThread](conversationthread.md) |Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.|
|[获取 conversationThread](../api/conversationthread-get.md) | [conversationThread](conversationthread.md) |获取属于某个组的特定线程。 |
|[更新](../api/conversationthread-update.md) | [conversationThread](conversationthread.md)  |更新 conversationThread 对象 |
|[删除](../api/conversationthread-delete.md) | 无 |删除 conversationThread 对象 |
|[答复](../api/conversationthread-reply.md)|无|通过新建 Post 实体答复此线程。|
|[列出帖子](../api/conversationthread-list-posts.md) |[帖子](post.md) 集合| 获取指定线程的帖子。 |

## <a name="properties"></a>属性
| 属性              | 类型                                 | 说明                                                                                                                                                                                      |
|:----------------------|:-------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| id                    | String                               | 只读。                                                                                                                                                                                       |
| toRecipients          | [recipient](recipient.md) collection | 收件人：线程的收件人。                                                                                                                                                               |
| ccRecipients          | [recipient](recipient.md) collection | 抄送：线程的收件人。                                                                                                                                                               |
| topic                 | String                               | The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.                                                                              |
| hasAttachments        | Boolean                              | 指示此线程中的任意帖子是否至少具有一个附件。                                                                                                               |
| lastDeliveredDateTime | DateTimeOffset                       | The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'` |
| uniqueSenders         | String collection                    | 向此线程发送邮件的所有用户。                                                                                                                                                |
| preview               | String                               | 本对话中最新帖子的正文中的简短摘要。                                                                                                                           |
| Resource.islocked              | Boolean                              | 指示线程是否已锁定。                                                                                                                                                               |

## <a name="relationships"></a>关系
| 关系 | 类型   |Description|
|:---------------|:--------|:----------|
|posts|[帖子](post.md) 集合| Read-only. Nullable.|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.conversationThread",
  "@odata.annotations": [
    {
      "property": "posts",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
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
