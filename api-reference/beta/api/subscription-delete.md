---
title: 删除订阅
description: 删除订阅。
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 57237a3fe5bdbfd76c518e0359ddd03d1eccd252
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447343"
---
# <a name="delete-subscription"></a>删除订阅

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi-sharedfeature](../includes/todo-deprecate-basetaskapi-sharedfeature.md)]

删除订阅。

有关支持订阅更改通知的资源列表，请参阅“ [权限](#permissions) ”部分中的表。

## <a name="permissions"></a>权限

根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。 若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。

| 支持的资源 | 委派（工作或学校帐户） | 委派（个人 Microsoft 帐户） | 应用程序 |
|:-----|:-----|:-----|:-----|
|[baseTask](../resources/todotask.md) (已弃用)  | Tasks.ReadWrite | Tasks.ReadWrite | 不支持。 |
|[callRecord](../resources/callrecords-callrecord.md) | 不支持。 | 不支持。 | CallRecords.Read.All  |
|[频道](../resources/channel.md)（/teams/getAllChannels – 组织中的所有频道） | 不支持。  | 不支持。 | Channel.ReadBasic.All，ChannelSettings.Read.All |
|[频道](../resources/channel.md) (/teams/{id}/channels) | Channel.ReadBasic.All，ChannelSettings.Read.All  | 不支持。 | Channel.ReadBasic.All，ChannelSettings.Read.All  |
|[聊天](../resources/chat.md)（/chats - 组织中的所有聊天） | 不支持。 | 不支持。 | Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All |
|[聊天](../resources/chat.md) (/chats/{id}) | Chat.ReadBasic, Chat.Read, Chat.ReadWrite | 不支持。 | ChatSettings.Read.Chat *、ChatSettings.ReadWrite.Chat*、Chat.Manage.Chat*、Chat.ReadBasic.All、Chat.Read.All、Chat.ReadWrite.All |
|[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages) | ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All | 不支持。 | ChannelMessage.Read.Group*、ChannelMessage.Read.All  |
|[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息） | 不支持。 | 不支持。 | ChannelMessage.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages) | Chat.Read、Chat.ReadWrite | 不支持。 | Chat.Read.All  |
|[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息） | 不支持。 | 不支持。 | Chat.Read.All  |
|[chatMessage](../resources/chatmessage.md)（/users/{id}/chats/getAllMessages - 特定用户所属所有聊天的聊天消息） | Chat.Read、Chat.ReadWrite | 不支持。 | Chat.Read.All、Chat.ReadWrite.All |
|[联系人](../resources/contact.md) | Contacts.Read | Contacts.Read | Contacts.Read |
|[conversationMember](../resources/conversationmember.md) (/chats/getAllMembers) | 不支持。 | 不支持。 | ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All. |
|[conversationMember](../resources/conversationmember.md) (/chats/{id}/members) | ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite | 不支持。 | ChatMember.Read.Chat *、Chat.Manage.Chat*、ChatMember.Read.All、ChatMember.ReadWrite.All、Chat.ReadBasic.All、Chat.Read.All、Chat.ReadWrite.All |
|[conversationMember](../resources/conversationmember.md) (/teams/getAllMembers)  | 不支持。 | 不支持。 | TeamMember.Read.All, TeamMember.ReadWrite.All |
|[conversationMember](../resources/conversationmember.md) (/teams/{id}/members) | TeamMember.Read.All | 不支持。 | TeamMember.Read.All |
|[conversationMember](../resources/conversationmember.md) (/teams/{id}/channels/getAllMembers) | 不支持。 | 不支持。 | ChannelMember.Read.All |
|[driveItem](../resources/driveitem.md)（用户的个人 OneDrive） | 不支持。 | Files.ReadWrite | 不支持。 |
|[driveItem](../resources/driveitem.md) (OneDrive for Business) | Files.ReadWrite.All | 不支持。 | Files.ReadWrite.All |
|[事件](../resources/event.md) | Calendars.Read | Calendars.Read | Calendars.Read |
|[组](../resources/group.md) | Group.Read.All | 不支持。 | Group.Read.All |
|[组对话](../resources/conversation.md) | Group.Read.All | 不支持。 | 不支持。 |
|[列表](../resources/list.md) | Sites.ReadWrite.All | 不支持。 | Sites.ReadWrite.All |
|[邮件](../resources/message.md) | Mail.ReadBasic、Mail.Read | Mail.ReadBasic、Mail.Read | Mail.Read |
|[联机会议](../resources/onlinemeeting.md) | 不支持 | 不支持 | OnlineMeetings.Read.All、OnlineMeetings.ReadWrite.All |
|[状态](../resources/presence.md) | Presence.Read.All | 不支持。 | 不支持。 |
|[打印机](../resources/printer.md) | 不支持。 | 不支持。 | 打印机。阅读.All，Printer.ReadWrite.All |
|[printTaskDefinition](../resources/printtaskdefinition.md) | 不支持。 | 不支持。 | PrintTaskDefinition.ReadWrite.All |
|安全[警报](../resources/alert.md) | SecurityEvents.ReadWrite.All | 不支持。 | SecurityEvents.ReadWrite.All |
|[团队](../resources/team.md)（/teams - 组织中的所有团队） | 不支持。 | 不支持。 | Team.ReadBasic.All，TeamSettings.Read.All |
|[团队](../resources/team.md) (/teams/{id}) | Team.ReadBasic.All，TeamSettings.Read.All | 不支持。 | Team.ReadBasic.All，TeamSettings.Read.All |
|[todoTask](../resources/todotask.md) | Tasks.ReadWrite | Tasks.ReadWrite | 不支持。 |
|[user](../resources/user.md) | User.Read.All | User.Read.All | User.Read.All |

> **注意**：标有 * 的权限用于 [特定于资源的同意](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)。

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a>driveItem

其他限制适用于 OneDrive 项目的订阅。 这些限制适用于订阅的创建和管理（获取、更新和删除）。

在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。 在 OneDrive for Business 上，只可以订阅根文件夹。 对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。 无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。

### <a name="contact-event-and-message"></a>联系人、事件和消息

可以订阅 Outlook **联系人**、 **事件** 或 **消息** 资源中的更改，并在 POST 请求有效负载中选择性地指定是否在通知中包含加密的资源数据。

[!INCLUDE [outlook-subscription-notes](../../includes/outlook-subscription-notes.md)]

### <a name="onlinemeetings-presence"></a>onlineMeetings，状态

**onlineMeetings** 和 **状态** 订阅需要对包含资源数据的通知进行 [加密](/graph/webhooks-with-resource-data) 。 如果在通知中需要资源数据，则未指定 [encryptionCertificate](../resources/subscription.md) 和 [encryptionCertificateId](../resources/subscription.md) ，则订阅创建将失败。
有关联机会议订阅的详细信息，请参阅 [获取联机会议的更改通知](/graph/changenotifications-for-onlinemeeting)。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a>请求标头

| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

要详细了解错误返回方式，请参阅[错误响应][error-response]。

## <a name="example"></a>示例

### <a name="request"></a>请求

请求示例如下所示。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/delete-subscription-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/delete-subscription-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

