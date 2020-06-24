---
title: 聊天资源类型
description: 聊天是一个或多个参与者之间的 Chatmessages 集合的集合。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 43ed088889a4b81d59cb9e1361ed978c9cb61141
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864201"
---
# <a name="chat-resource-type"></a>聊天资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

聊天是一个或多个参与者之间的[chatmessages 集合](chatmessage.md)的集合。 参与者可以是用户或应用程序。

## <a name="methods"></a>Methods

|  方法       |  返回类型  | 说明| 权限 |
|:---------------|:--------|:----------|-----------|
|[列出聊天](../api/chat-list.md) | [聊天](channel.md)收藏 | 获取用户所属的聊天列表。| **仅委派** |
|[获取聊天](../api/chat-get.md) | [参与](channel.md) | 读取聊天的属性和关系。| **仅委派** |
|[列出聊天成员](../api/conversationmember-list.md) | [conversationmember](conversationmember.md) 集合 | 获取聊天中所有用户的列表。| 委派和应用程序 * |
|[获取聊天成员](../api/conversationmember-get.md) | [conversationmember](conversationmember.md) | 获取聊天中的单个用户。| 委派和应用程序 * |
|[列出聊天中的消息](../api/chatmessage-list.md)  | [chatMessage](../resources/chatmessage.md) | 获取一对一聊天或群组聊天中的消息。 | 委派和应用程序 * |
|[获取聊天中的消息](../api/chatmessage-get.md)  | [chatMessage](../resources/chatmessage.md) | 获取聊天中的单个消息。 | 委派和应用程序 * |

\*> **注意：** 使用应用程序权限时，请务必了解如何获取聊天 ID。 由于不支持列出具有应用程序权限的聊天，因此并非所有方案都可行。 可以获取具有委派权限的聊天 Id，也可以通过应用程序权限获取[/chats/allMessages 的更改通知](../api/subscription-post-subscriptions.md)。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
| id| String| 聊天的唯一标识符。 只读。|
| topic| String|  Optional聊天的主题或主题。 仅适用于组聊天。|
| createdDateTime| dateTimeOffset|  聊天的创建日期和时间。 只读。|
| lastUpdatedDateTime| dateTimeOffset|  更新聊天的日期和时间。 只读。|

## <a name="relationships"></a>关系

| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
| installedApps | [teamsAppInstallation](teamsappinstallation.md) 集合 | 聊天中所有应用的集合。 可为 Null。 |
| 成员 | [conversationMember](conversationmember.md) 集合 | 聊天中所有人员的集合。 可为 NULL。 |
| messages | [chatMessage](chatmessage.md) 集合 | 聊天中所有邮件的集合。 可为 Null。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chat"
}-->

```json
{
  "id": "string (identifier)",
  "topic": "string",
  "createdDateTime": "dateTimeOffset",
  "lastUpdatedDateTime": "dateTimeOffset"
}

```

## <a name="see-also"></a>另请参阅

- [频道](channel.md)
- [chatMessage](chatmessage.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
