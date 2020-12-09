---
title: 聊天资源类型
description: 聊天是一个或多个参与者之间的 Chatmessages 集合的集合。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f1745f987577d94f14f81d79a9f8afb89c1ab793
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606935"
---
# <a name="chat-resource-type"></a>聊天资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

聊天是一个或多个参与者之间的 [chatmessages 集合](chatmessage.md) 的集合。 参与者可以是用户或应用程序。

## <a name="methods"></a>方法

|  方法       |  返回类型  | Description| 
|:---------------|:--------|:----------|
|[列出聊天](../api/chat-list.md) | [聊天](chat.md) 收藏 | 获取用户所属的聊天列表。| 
|[获取聊天](../api/chat-get.md) | [聊天](chat.md) | 读取聊天的属性和关系。| 
|[列出聊天成员](../api/conversationmember-list.md) | [conversationMember](conversationmember.md) 集合 | 获取聊天中所有用户的列表。| 
|[获取聊天成员](../api/conversationmember-get.md) | [conversationMember](conversationmember.md) | 获取聊天中的单个用户。| 
|[列出聊天中的消息](../api/chat-list-message.md)  | [chatMessage](../resources/chatmessage.md) | 获取一对一聊天或群组聊天中的消息。 | 
|[获取聊天中的消息](../api/chat-get-message.md)  | [chatMessage](../resources/chatmessage.md) | 获取聊天中的单个消息。 | 
|[在用户和应用之间获取聊天](../api/userscopeteamsappinstallation-get-chat.md) | [聊天](chat.md)| 在用户和应用之间获取一对一聊天 |
|[获取所有聊天消息](../api/chats-getallmessages.md)| [聊天](chat.md) 收藏| 从用户参与的所有聊天中获取邮件，包括一对一聊天、群研讨和会议聊天。 |
|[列出聊天中的应用程序](../api/chat-list-installedapps.md) |[teamsAppInstallation](teamsappinstallation.md) 集合 | 列出聊天中安装的应用程序。|
|[获取聊天中的应用程序](../api/chat-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | 获取聊天中安装的特定应用程序。|
|[在聊天中添加应用程序](../api/chat-post-installedapps.md) | | 添加 (在聊天中的应用程序) 安装。|
|[升级聊天中的应用程序](../api/chat-teamsappinstallation-upgrade.md) | 无 | 更新到聊天中安装的最新版本的应用程序。|
|[从聊天中卸载应用程序](../api/chat-delete-installedapps.md) | 无 | 从聊天中删除 (卸载) 应用程序。|
|[聊天中的列表选项卡](../api/chat-list-tabs.md) | [teamsTab](teamstab.md) | 固定到聊天的列表选项卡。|
|[聊天中的 "获取" 选项卡](../api/chat-get-tabs.md) | [teamsTab](teamstab.md) | 获取固定到聊天的特定选项卡。|
|[将选项卡添加到聊天](../api/chat-post-tabs.md) | [teamsTab](teamstab.md) | 向聊天添加 (pin) 选项卡。|
|[聊天中的更新选项卡](../api/chat-patch-tabs.md) | [teamsTab](teamstab.md) | 更新聊天中的选项卡的属性。|
|[从聊天中删除选项卡](../api/chat-delete-tabs.md) | 无 | ) 聊天中的选项卡删除 (的 "取消固定"。|

>**注意：** 使用应用程序权限时，请务必了解如何获取聊天 ID。 由于不支持列出具有应用程序权限的聊天，因此并非所有方案都可行。 可以获取具有委派权限的聊天 Id，也可以通过应用程序权限获取 [/chats/getAllMessages 的更改通知](../api/subscription-post-subscriptions.md) 。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
| id| String| 聊天的唯一标识符。 只读。|
| topic| String|   (聊天的可选) 主题或主题。 仅适用于组聊天。|
| createdDateTime| dateTimeOffset|  聊天的创建日期和时间。 只读。|
| lastUpdatedDateTime| dateTimeOffset|  重命名或更改成员身份时的聊天的日期和时间。 将邮件发送到聊天时，不会对 lastUpdatedDateTime 进行更新。 只读。|

## <a name="relationships"></a>关系

| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
| installedApps | [teamsAppInstallation](teamsappinstallation.md) 集合 | 聊天中所有应用的集合。 可为 Null。 |
| members | [conversationMember](conversationmember.md) 集合 | 聊天中所有人员的集合。 可为 Null。 |
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


