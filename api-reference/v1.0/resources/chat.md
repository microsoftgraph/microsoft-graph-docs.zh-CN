---
title: 聊天资源类型
description: 聊天是一个或多个参与者之间的 chatMessage 的集合。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5b77dc1d29107204172f3fd79ba9ae2a12d320bc
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2022
ms.locfileid: "66689984"
---
# <a name="chat-resource-type"></a>聊天资源类型

命名空间：microsoft.graph

聊天是一个或多个参与者之间的 [chatMessage 的](chatmessage.md) 集合。 参与者可以是用户或应用。

> **注意**：如果聊天与 [onlineMeeting](../resources/onlinemeeting.md) 实例相关联，则列出的一些方法将暂时影响会议。

## <a name="methods"></a>方法

|  方法       |  返回类型  | 说明| 
|:---------------|:--------|:----------|
| **聊天管理** |||
|[创建聊天](../api/chat-post.md) | [聊天](chat.md) | 创建新聊天。| 
|[获取聊天](../api/chat-get.md) | [聊天](chat.md) | 读取聊天的属性和关系。| 
|[更新聊天](../api/chat-patch.md) | [聊天](chat.md) | 更新聊天的属性。|
|[列出聊天成员](../api/chat-list-members.md) | [conversationMember](conversationmember.md) 集合 | 获取聊天中所有用户的列表。| 
|[添加聊天成员](../api/chat-post-members.md) | 位置标头 | 将用户添加到聊天。| 
|[获取聊天成员](../api/chat-get-members.md) | [conversationMember](conversationmember.md) | 获取聊天中的单个用户。| 
|[删除聊天成员](../api/chat-delete-members.md)|无|从聊天中删除用户。|
|[获取用户和应用之间的聊天](../api/userscopeteamsappinstallation-get-chat.md) | [聊天](chat.md)| 在用户和应用之间进行一对一聊天 |
| **邮件** |||
|[列出聊天中的消息](../api/chat-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | 在聊天中获取消息。 | 
|[获取聊天中的消息](../api/chatmessage-get.md)  | [chatMessage](../resources/chatmessage.md) | 获取聊天中的单个消息。 | 
|[为用户在所有聊天中获取消息](../api/chats-getallmessages.md)| [聊天](chat.md) 集合| 从用户参与的所有聊天中获取消息。 |
| **应用** |||
|[列出聊天中的应用](../api/chat-list-installedapps.md) |[teamsAppInstallation](teamsappinstallation.md) 集合 | 列出聊天 (和关联会议) 中安装的应用。|
|[在聊天中获取应用](../api/chat-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | 获取聊天 (和关联会议) 中安装的特定应用。|
|[在聊天中添加应用](../api/chat-post-installedapps.md) | | 在聊天 (和关联会议) 中添加 (安装) 应用。|
|[在聊天中升级应用](../api/chat-teamsappinstallation-upgrade.md) | 无 | 更新到聊天 (和关联会议) 中安装的最新版本的应用。|
|[从聊天中卸载应用](../api/chat-delete-installedapps.md) | 无 | 从聊天 (和关联会议) 中删除 (卸载) 应用。|
| **选项卡** |||
|[聊天中的列表选项卡](../api/chat-list-tabs.md) | [teamsTab](teamstab.md) | 固定到聊天 (和关联会议) 的列表选项卡。|
|[获取聊天中的选项卡](../api/chat-get-tabs.md) | [teamsTab](teamstab.md) | 获取固定到聊天 (和关联会议) 的特定选项卡。|
|[向聊天添加选项卡](../api/chat-post-tabs.md) | [teamsTab](teamstab.md) | 将 (固定) 选项卡添加到聊天 (和关联会议) 。|
|[聊天中的“更新”选项卡](../api/chat-patch-tabs.md) | [teamsTab](teamstab.md) | 更新聊天 (和关联会议) 中选项卡的属性。|
|[从聊天中删除选项卡](../api/chat-delete-tabs.md) | 无 | 从聊天 (和关联会议) 中删除 (取消固定) 选项卡。|

>**注意：** 使用应用程序权限时，请确保知道如何获取聊天 ID。 由于不支持列出具有应用程序权限的聊天，因此并非所有方案都是可能的。 可以获取具有委派权限的聊天 ID，也可以从具有应用程序权限的 [/chats/getAllMessage 的更改通知](../api/subscription-post-subscriptions.md) 中获取聊天 ID。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
| chatType| [chatType](../resources/chat.md#chattype-values) | 指定聊天的类型。 可能的值是：`group`、`oneOnOne`、`meeting`、`unknownFutureValue`。|
| createdDateTime| dateTimeOffset|  创建聊天的日期和时间。 只读。|
| id| String| 聊天的唯一标识符。 只读。|
| lastUpdatedDateTime| dateTimeOffset|  聊天重命名或成员列表上次更改的日期和时间。 只读。|
| onlineMeetingInfo | [teamworkOnlineMeetingInfo](../resources/teamworkonlinemeetinginfo.md) | 表示有关联机会议的详细信息。 如果聊天未与联机会议关联，则该属性为空。 只读。|
| tenantId| String | 在其中创建聊天的租户的标识符。 只读。|
| topic| String|   (聊天的可选) 主题或主题。 仅可用于群聊。|
| webUrl | String| Microsoft Teams 中聊天的 URL。 URL 应被视为不透明的 Blob，而不是分析的。 只读。 |

### <a name="chattype-values"></a>chatType 值 

| 成员             | 值 | 说明               |
| :----------------- | :---- | :------------------------ |
|oneOnOne            | 0     | 指示聊天是 1：1 聊天。 对于这种类型的聊天，名册大小是固定的;无法删除/添加成员。|
|组               | 1     | 指示聊天是群组聊天。 可以更新至少两个人) 的名册大小 (此类型的聊天。 可以稍后删除/添加成员。|
|会议             | 2     | 指示聊天与联机会议相关联。 这种类型的聊天仅在创建联机会议时创建。|
|unknownFutureValue  | 3     | 可变枚举 sentinel 值。 请勿使用。 |

## <a name="relationships"></a>关系

| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
| installedApps | [teamsAppInstallation](teamsappinstallation.md) 集合 | 聊天中所有应用的集合。 可为 Null。 |
| members | [conversationMember](conversationmember.md) 集合 | 聊天中所有成员的集合。 可为 Null。 |
| messages | [chatMessage](chatmessage.md) 集合 | 聊天中所有消息的集合。 可为 NULL。 |
| 选项卡 | [teamsTab](teamstab.md) 集合 | 聊天中所有选项卡的集合。 可为 Null。 |

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
  "lastUpdatedDateTime": "dateTimeOffset",
  "chatType": "string",
  "webUrl": "string",
  "tenantId": "string",
  "onlineMeetingInfo": {
    "@odata.type": "microsoft.graph.teamworkOnlineMeetingInfo"
  }
}
```

## <a name="see-also"></a>另请参阅

- [channel](channel.md)
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


