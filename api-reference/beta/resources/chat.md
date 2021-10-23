---
title: 聊天资源类型
description: 聊天是一个或多个参与者之间的 chatMessages 集合。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7d572051d0889add7f68cc868d410bf3dc702d65
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60560812"
---
# <a name="chat-resource-type"></a>聊天资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

聊天是一个或多个 [参与者之间的 chatMessages](chatmessage.md) 集合。 参与者可以是用户或应用。

> **注意**：如果聊天与 [onlineMeeting](../resources/onlinemeeting.md) 实例关联，则列出的一些方法将可传递影响会议。

## <a name="methods"></a>方法

|  方法       |  返回类型  | 说明| 
|:---------------|:--------|:----------|
| **聊天管理** |||
|[列出聊天](../api/chat-list.md) | [chat](chat.md) 集合 | 获取用户参与的聊天列表。| 
|[创建聊天](../api/chat-post.md) | [聊天](chat.md) | 创建新聊天。| 
|[获取聊天](../api/chat-get.md) | [聊天](chat.md) | 读取聊天的属性和关系。| 
|[更新聊天](../api/chat-patch.md) | [聊天](chat.md) | 更新聊天的属性。|
|[列出聊天成员](../api/chat-list-members.md) | [conversationMember](conversationmember.md) 集合 | 获取聊天中所有用户的列表。| 
|[添加聊天成员](../api/chat-post-members.md) | 位置标头 | 向聊天中添加用户。| 
|[获取聊天成员](../api/chat-get-members.md) | [conversationMember](conversationmember.md) | 获取聊天中的单个用户。| 
|[删除聊天成员](../api/chat-delete-members.md)|无|从聊天中删除用户。|
|[获取用户和应用之间的聊天](../api/userscopeteamsappinstallation-get-chat.md) | [聊天](chat.md)| 获取用户与应用之间的一对一聊天 |
| **邮件** |||
|[列出聊天中的消息](../api/chat-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | 获取聊天中的消息。 | 
|[获取聊天中的消息](../api/chatmessage-get.md)  | [chatMessage](../resources/chatmessage.md) | 获取聊天中的单个消息。 | 
|[为用户在所有聊天中获取消息](../api/chats-getallmessages.md)| [chat](chat.md) 集合| 从用户参与的所有聊天中获取消息。 |
| **应用** |||
|[列出聊天中的应用](../api/chat-list-installedapps.md) |[teamsAppInstallation](teamsappinstallation.md) 集合 | 列出聊天网站中安装 (关联的会议) 。|
|[在聊天中获取应用](../api/chat-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | 在聊天活动和相关会议 (安装特定) 。|
|[在聊天中添加应用](../api/chat-post-installedapps.md) | | 添加 (在) 会议及其关联的会议 (中安装) 。|
|[升级聊天中的应用](../api/chat-teamsappinstallation-upgrade.md) | 无 | 更新到聊天会话和关联会议 (安装的应用的) 。|
|[从聊天中卸载应用](../api/chat-delete-installedapps.md) | 无 | 从 (会议) 中删除 (应用) 。|
|[List permission grants](../api/chat-list-permissiongrants.md) | [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) 集合 | 列出已授予此聊天中的应用的权限。|
| **选项卡** |||
|[列出聊天中的选项卡](../api/chat-list-tabs.md) | [teamsTab](teamstab.md) | 列出固定到聊天 (关联的会议选项卡) 。|
|[在聊天中获取选项卡](../api/chat-get-tabs.md) | [teamsTab](teamstab.md) | 获取固定到聊天组和关联 (的特定选项卡) 。|
|[向聊天添加选项卡](../api/chat-post-tabs.md) | [teamsTab](teamstab.md) | 将 (固定) 选项卡添加到聊天 (关联的会议) 。|
|[聊天中的"更新"选项卡](../api/chat-patch-tabs.md) | [teamsTab](teamstab.md) | 更新聊天记录和相关会议 (选项卡) 。|
|[从聊天中删除选项卡](../api/chat-delete-tabs.md) | 无 | 从 (和) 会议记录中删除 (取消固定选项卡) 。|
| **Operations** |||
|[列出聊天操作](../api/chat-list-operations.md) | [teamsAsyncOperation](teamsAsyncOperation.md) 集合 | 获取在聊天中运行或运行的异步操作列表。|
|[获取聊天操作](../api/teamsasyncoperation-get.md#example-get-operation-on-chat) | [teamsAsyncOperation](teamsAsyncOperation.md) | 获取在聊天中运行或运行的单个异步操作。|

>**注意：** 使用应用程序权限时，请务必了解如何获取聊天 ID。 由于不支持列出具有应用程序权限的聊天，因此并非所有方案都可行。 可以获取具有委派权限的聊天 ID，以及获取具有应用程序权限的 [/chats/getAllMessages](../api/subscription-post-subscriptions.md) 更改通知。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
| chatType| [chatType](../resources/chat.md#chattype-values) | 指定聊天类型。 可取值为：`group`、`oneOnOne`、`meeting`、`unknownFutureValue`。|
| createdDateTime| dateTimeOffset|  创建聊天的日期和时间。 只读。|
| id| String| 聊天的唯一标识符。 只读。|
| lastUpdatedDateTime| dateTimeOffset|  上次更改聊天的日期和时间或成员列表。 只读。|
| onlineMeetingInfo | [teamworkOnlineMeetingInfo](../resources/teamworkonlinemeetinginfo.md) | 表示有关联机会议的详细信息。 如果聊天未与联机会议关联，则属性为空。 只读。|
| tenantId| String | 创建聊天的租户的标识符。 只读。|
| topic| String|   (可选) 聊天的主题或主题。 仅适用于群聊。|
| 一个|[chatViewpoint](../resources/chatviewpoint.md)|表示有关聊天的特定于呼叫者的信息，例如上次消息读取日期和时间。 只有在委托上下文中提出请求时，才填充此属性。|
| webUrl| String | 一个超链接，将转到 Microsoft Teams。 应将此 URL 视为不透明的 blob，而不对其进行解析。 只读。|


### <a name="chattype-values"></a>chatType 值 

| 成员             | 值 | 说明               |
| :----------------- | :---- | :------------------------ |
|oneOnOne            | 0     | 指示聊天为一对一聊天。 对于此类聊天，名单大小是固定的;无法删除/添加成员。|
|组               | 1     | 指示聊天是群聊。 可以针对 (聊天类型更新至少两) 名单大小。 稍后可以删除/添加成员。|
|meeting             | 2     | 指示聊天与联机会议相关联。 此类聊天仅在创建联机会议时创建。|
|unknownFutureValue  | 3     | 可发展枚举 sentinel 值。 请勿使用。 |

## <a name="relationships"></a>关系

| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
| installedApps | [teamsAppInstallation](teamsappinstallation.md) 集合 | 聊天中所有应用的集合。 可为 Null。 |
| members | [conversationMember](conversationmember.md) 集合 | 聊天中所有成员的集合。 可为 Null。 |
| messages | [chatMessage](chatmessage.md) 集合 | 聊天中所有消息的集合。 可为 NULL。 |
| permissionGrants| [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) 集合| 授予聊天应用的权限集合。|
| operations | [teamsAsyncOperation](teamsasyncoperation.md) 集合 | 在聊天中运行Teams运行的所有异步操作的集合。 可为 NULL。 
| lastMessagePreview | [chatMessageInfo](chatmessageinfo.md)| 预览聊天中发送的最后一条消息。 如果聊天中未发送任何消息，则其为 Null。 目前，仅 [列表聊天](../api/chat-list.md) 操作支持此属性。|

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
  "viewpoint": {
    "@odata.type": "microsoft.graph.chatViewpoint"
  },
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


