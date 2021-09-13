---
title: conversationThread 资源类型
description: conversationThread 是 帖子 集合。
author: dkershaw10
ms.localizationpriority: medium
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: b559ce1ee1d6f0a79734e65b3a491a047fbb9cd8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59029092"
---
# <a name="conversationthread-resource-type"></a>conversationThread 资源类型

命名空间：microsoft.graph

conversationThread 是 [帖子](post.md) 集合。

最后一个帖子收件人集合聚合了整个线程的收件人。线程的收件人集合可以不断扩大。从线程中移除某个收件人时将创建一个新的线程。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出线程](../api/group-list-threads.md) | [conversationThread](conversationthread.md) 集合 |获取组的所有线程。|
|[创建线程](../api/group-post-threads.md) | [conversationThread](conversationthread.md) |通过首先创建一个线程，启动一个新对话。在组中创建新对话、对话线程和帖子。|
|[获取 conversationThread](../api/conversationthread-get.md) | [conversationThread](conversationthread.md) |获取属于某个组的特定线程。 |
|[更新](../api/conversationthread-update.md) | [conversationThread](conversationthread.md)  |更新 conversationThread 对象 |
|[删除](../api/conversationthread-delete.md) | None |删除 conversationThread 对象 |
|[答复](../api/conversationthread-reply.md)|无|通过新建 Post 实体答复此线程。|
|[列出帖子](../api/conversationthread-list-posts.md) |[帖子](post.md) 集合| 获取指定线程的帖子。 |

## <a name="properties"></a>属性
| 属性              | 类型                                 | 说明                                                                                                                                                                                      |
|:----------------------|:-------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| id                    | String                               | 只读。 <br/><br/>默认情况下返回。                                                                                                                                                                                      |
| toRecipients          | [recipient](recipient.md) collection | 收件人：线程的收件人。 <br/><br/>仅在 `$select` 上返回。                                                                                                                                                              |
| ccRecipients          | [recipient](recipient.md) collection | 抄送：线程的收件人。 <br/><br/>仅在 `$select` 上返回。                                                                                                                                                               |
| topic                 | String                               | 对话的主题。在创建对话时可设置此属性，但无法对其进行更新。 <br/><br/>默认情况下返回。                                                                              |
| hasAttachments        | Boolean                              | 指示此线程中的任意帖子是否至少具有一个附件。 <br/><br/>默认情况下返回。                                                                                                              |
| lastDeliveredDateTime | DateTimeOffset                       | 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。<br/><br/>默认情况下返回。 |
| uniqueSenders         | String collection                    | 向此线程发送邮件的所有用户。 <br/><br/>默认情况下返回。                                                                                                                                               |
| preview               | String                               | 此对话中最新文章正文的简短摘要。 <br/><br/>默认情况下返回。                                                                                                                           |
| isLocked              | Boolean                              | 指示线程是否已锁定。 <br/><br/>默认情况下返回。                                                                                                                                                              |

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|posts|[帖子](post.md) 集合| 只读。可为空。|

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

