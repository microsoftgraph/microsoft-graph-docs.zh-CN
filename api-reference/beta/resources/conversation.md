---
title: 对话资源类型
description: 对话是 线程 集合，而线程包含相应线程拥有的帖子。对话中的所有线程和帖子共享相同的主题。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 7d489a75f72a705a77231af940094b7aa2d18fe1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528646"
---
# <a name="conversation-resource-type"></a>对话资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

对话是 [线程](conversationthread.md) 集合，而线程包含相应线程拥有的帖子。对话中的所有线程和帖子共享相同的主题。

此资源支持订阅[更改通知](/graph/webhooks)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出对话](../api/group-list-conversations.md) | [对话](conversation.md) 集合 |获取此组中的对话列表。|
|[创建](../api/group-post-conversations.md) |[conversation](conversation.md)| 通过包括线程和帖子创建新对话。|
|[获取对话](../api/conversation-get.md) | [对话](conversation.md) |读取 conversation 对象的属性和关系。|
|[删除](../api/conversation-delete.md) | 无 |删除 conversation 对象 |
|[列出对话线程](../api/conversation-list-threads.md) |[conversationThread](conversationthread.md) 集合| 获取组对话中的所有线程。|
|[创建对话线程](../api/conversation-post-threads.md) |[conversationThread](conversationthread.md) 集合| 在指定会话中创建线程。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|hasAttachments|Boolean|指示此对话中的任意帖子是否至少有一个附件。|
|id|String|对话的唯一标识符。只读。|
|lastDeliveredDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`|
|preview|String|来自此对话中最新帖子的正文的简短摘要。|
|topic|String|对话的主题。在创建对话时可设置此属性，但无法对其进行更新。|
|uniqueSenders|String collection|发送消息到此对话的所有用户。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|线程|[conversationThread](conversationthread.md) 集合|对话中所有对话线程的集合。一种导航属性。只读。可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversation"
}-->

```json
{
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "topic": "string",
  "uniqueSenders": ["string"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/conversation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
