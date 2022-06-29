---
title: 创建订阅
description: 订阅侦听器应用程序，以便在 Microsoft Graph 资源上的数据发生更改时接收更改通知。
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: e64abb2c70c0f51a8b2942ba0b165f047a596c01
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445207"
---
# <a name="create-subscription"></a>创建订阅

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi-sharedfeature](../includes/todo-deprecate-basetaskapi-sharedfeature.md)]

订阅侦听器应用程序，以在 Microsoft Graph 中指定资源发生的更改属于请求的更改类型时接收更改通知。

请参阅" [权限](#permissions) 部分中的表格，了解支持订阅以更改通知的资源列表。

某些资源支持在更改通知中包括加密资源数据的选项。 这些资源包括 [chatMessage](../resources/chatmessage.md)、 [联系](../resources/contact.md)人、 [事件](../resources/event.md)、 [消息](../resources/message.md)、 [onlineMeetings](../resources/onlinemeeting.md) 和 [状态](../resources/presence.md)。 有关详细信息，请参阅[设置包含资源数据的更改通知](/graph/webhooks-with-resource-data)和 [Microsoft Graph 中 Outlook 资源的更改通知](/graph/outlook-change-notification-overview)。

## <a name="permissions"></a>权限

创建订阅需要对资源的读取权限。 例如，若要获取有关邮件的更改通知，应用需要 Mail.Read 权限。 

根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。 要了解详细信息，包括在选择权限之前的 [注意事项](/graph/auth/auth-concepts#best-practices-for-requesting-permissions)，可在 [权限](/graph/permissions-reference) 中搜索以下权限。

| 支持的资源 | 委派（工作或学校帐户） | 委派（个人 Microsoft 帐户） | 应用程序 |
|:-----|:-----|:-----|:-----|
|[baseTask](../resources/basetask.md) (已弃用)  | Tasks.ReadWrite | Tasks.ReadWrite | 不支持 |
|[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords) | 不支持 | 不支持 | CallRecords.Read.All  |
|[频道](../resources/channel.md)（/teams/getAllChannels – 组织中的所有频道） | 不支持  | 不支持 | Channel.ReadBasic.All，ChannelSettings.Read.All |
|[频道](../resources/channel.md) (/teams/{id}/channels) | Channel.ReadBasic.All，ChannelSettings.Read.All  | 不支持 | Channel.ReadBasic.All，ChannelSettings.Read.All  |
|[聊天](../resources/chat.md)（/chats - 组织中的所有聊天） | 不支持 | 不支持 | Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All |
|[聊天](../resources/chat.md) (/chats/{id}) | Chat.ReadBasic, Chat.Read, Chat.ReadWrite | 不支持 | ChatSettings.Read.Chat *、ChatSettings.ReadWrite.Chat*、Chat.Manage.Chat*、Chat.ReadBasic.All、Chat.Read.All、Chat.ReadWrite.All |
|[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages) | ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All | 不支持 | ChannelMessage.Read.Group*、ChannelMessage.Read.All  |
|[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息） | 不支持 | 不支持 | ChannelMessage.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages) | Chat.Read、Chat.ReadWrite | 不支持 | Chat.Read.All  |
|[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息） | 不支持 | 不支持 | Chat.Read.All  |
|[chatMessage](../resources/chatmessage.md)（/users/{id}/chats/getAllMessages - 特定用户所属所有聊天的聊天消息） | Chat.Read、Chat.ReadWrite | 不支持 | Chat.Read.All、Chat.ReadWrite.All |
|[联系人](../resources/contact.md) | Contacts.Read | Contacts.Read | Contacts.Read |
|[conversationMember](../resources/conversationmember.md) (/chats/getAllMembers) | 不支持 | 不支持 | ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All. |
|[conversationMember](../resources/conversationmember.md) (/chats/{id}/members) | ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite | 不支持 | ChatMember.Read.Chat *、Chat.Manage.Chat*、ChatMember.Read.All、ChatMember.ReadWrite.All、Chat.ReadBasic.All、Chat.Read.All、Chat.ReadWrite.All |
|[conversationMember](../resources/conversationmember.md) (/teams/getAllMembers)  | 不支持 | 不支持 | TeamMember.Read.All, TeamMember.ReadWrite.All |
|[conversationMember](../resources/conversationmember.md) (/teams/{id}/members) | TeamMember.Read.All | 不支持 | TeamMember.Read.All |
|[conversationMember](../resources/conversationmember.md) (/teams/{id}/channels/getAllMembers) | 不支持 | 不支持 | ChannelMember.Read.All |
|[driveItem](../resources/driveitem.md)（用户的个人 OneDrive） | 不支持 | Files.ReadWrite | 不支持 |
|[driveItem](../resources/driveitem.md) (OneDrive for Business) | Files.ReadWrite.All | 不支持 | Files.ReadWrite.All |
|[事件](../resources/event.md) | Calendars.Read | Calendars.Read | Calendars.Read |
|[组](../resources/group.md) | Group.Read.All | 不支持 | Group.Read.All |
|[组对话](../resources/conversation.md) | Group.Read.All | 不支持 | 不支持 |
|[列表](../resources/list.md) | Sites.ReadWrite.All | 不支持 | Sites.ReadWrite.All |
|[邮件](../resources/message.md) | Mail.ReadBasic、Mail.Read | Mail.ReadBasic、Mail.Read | Mail.Read |
|[联机会议](../resources/onlinemeeting.md) | 不支持 | 不支持 | OnlineMeetings.Read.All、OnlineMeetings.ReadWrite.All |
|[状态](../resources/presence.md) | Presence.Read.All | 不支持 | 不支持 |
|[打印机](../resources/printer.md) | 不支持 | 不支持 | 打印机。阅读.All，Printer.ReadWrite.All |
|[printTaskDefinition](../resources/printtaskdefinition.md) | 不支持 | 不支持 | PrintTaskDefinition.ReadWrite.All |
|安全[警报](../resources/alert.md) | SecurityEvents.ReadWrite.All | 不支持 | SecurityEvents.ReadWrite.All |
|[团队](../resources/team.md)（/teams - 组织中的所有团队） | 不支持 | 不支持 | Team.ReadBasic.All，TeamSettings.Read.All |
|[团队](../resources/team.md) (/teams/{id}) | Team.ReadBasic.All，TeamSettings.Read.All | 不支持 | Team.ReadBasic.All，TeamSettings.Read.All |
|[todoTask](../resources/todotask.md) | Tasks.ReadWrite | Tasks.ReadWrite | 不支持 |
|[user](../resources/user.md) | User.Read.All | User.Read.All | User.Read.All |

建议使用上表中记载的权限。 由于安全限制，Microsoft Graph 订阅在只需要读取访问权限时将不支持写入访问权限。

> **注意**：标有 * 的权限用于 [特定于资源的同意](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)。

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a>driveItem

其他限制适用于 OneDrive 项目的订阅。 这些限制适用于订阅的创建和管理（获取、更新和删除）。

在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。 在 OneDrive for Business 上，只可以订阅根文件夹。 对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。 无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。

OneDrive for Business 和 SharePoint 支持向应用程序发送有关在 **driveItem** 上发生的安全事件通知。 若要订阅这些事件，请为请求添加 `prefer:includesecuritywebhooks` 标头以创建订阅。 创建订阅后，当项目权限更改时，你将收到通知。 此标头适用于 SharePoint 和 OneDrive for Business 帐户，但不适用于 OneDrive 消费者版本的帐户。

### <a name="contact-event-and-message"></a>联系人、事件和消息

可以订阅 Outlook **联系人**、 **事件** 或 **消息** 资源中的更改，并在 POST 请求有效负载中选择性地指定是否在通知中包含加密的资源数据。

[!INCLUDE [outlook-subscription-notes](../../includes/outlook-subscription-notes.md)]

### <a name="onlinemeetings-presence"></a>onlineMeetings，状态

在使用加密资源数据 [创建通知订阅](/graph/webhooks-with-resource-data#creating-a-subscription)时，**OnlineMeetings** 和 **状态** 上的订阅需要 **encryptionCertificate** 和 **encryptionCertificateId** 属性。 有关详细信息，请参阅 [设置更改通知以包含资源数据](/graph/webhooks-with-resource-data)。
有关联机会议订阅的详细信息，请参阅 [获取联机会议的更改通知](/graph/changenotifications-for-onlinemeeting)。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a>请求标头

| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [订阅](../resources/subscription.md) 对象。

要详细了解错误返回方式，请参阅[错误响应][error-response]。

## <a name="example"></a>示例

### <a name="request"></a>请求

在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。
`clientState` 和 `latestSupportedTlsVersion` 是可选字段。

此请求为当前已登录用户收到的新邮件的更改通知创建订阅。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "created",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue",
   "latestSupportedTlsVersion": "v1_2"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-subscription-from-subscriptions-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-subscription-from-subscriptions-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。`clientState` 和 `latestSupportedTlsVersion` 字段是可选的。

#### <a name="resources-examples"></a>资源示例

下面是资源属性的有效值。

| 资源类型 | 示例 |
|:------ |:----- |
|[baseTask](../resources/basetask.md) (已弃用)  | `/me/tasks/lists/{Id}/tasks`
|[通话记录](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[渠道](../resources/channel.md)|`/teams/getAllChannels`, `/teams/{id}/channels`|
|[聊天](../resources/chat.md)|`/chats`, `/chats/{id}`|
|[聊天消息](../resources/chatmessage.md) | `chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages` |
|[联系人](../resources/contact.md)|`me/contacts`|
|[ConversationMember](../resources/conversationmember.md)|`/chats/{id}/members`, `/chats/getAllMembers`, `/teams/{id}/members`, `/teams/getAllMembers`, `/teams/{id}/channels/getAllMembers`|
|[对话](../resources/conversation.md)|`groups('{id}')/conversations`|
|[驱动器](../resources/driveitem.md)|`me/drive/root`|
|[事件](../resources/event.md)|`me/events`|
|[组](../resources/group.md)|`groups`|
|[列表](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[邮件](../resources/message.md)|`me/mailfolders('inbox')/messages`, `me/messages`|
|[OnlineMeetings](../resources/onlinemeeting.md)|`/communications/onlineMeetings/?$filter=JoinWebUrl eq '{JoinWebUrl}'`|
|[状态](../resources/presence.md)| `/communications/presences/{id}`（单个用户），`/communications/presences?$filter=id in ('{id}','{id}',…)`（多个用户）|
|[打印机](../resources/printer.md) |`print/printers/{id}/jobs`|
|[PrintTaskDefinition](../resources/printtaskdefinition.md)|`print/taskDefinitions/{id}/tasks`|
|[Teams](../resources/team.md)|`/teams`, `/teams/{id}`|
|[用户](../resources/user.md)|`users`|
|[todoTask](../resources/todotask.md) | `/me/todo/lists/{todoTaskListId}/tasks`
|[安全警报](../resources/alert.md)|`security/alerts?$filter=status eq 'NewAlert'`|

> **注意：** 以 `me` 开头的任何路径也可与 `users/{id}`（而不是 `me`）一起使用，从而以特定用户为目标，而不是以当前用户为目标。

### <a name="response"></a>响应

以下示例显示了相应的响应。 

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2",
  "notificationContentType": "application/json"
}
```

#### <a name="notification-endpoint-validation"></a>通知终结点验证

**notificationUrl** 属性中指定的订阅通知终结点 () 必须能够响应验证请求，如 [为用户数据更改设置通知中](/graph/webhooks#notification-endpoint-validation)所述。 如果验证失败，创建订阅请求返回错误“400 请求无效”。

[error-response]: /graph/errors

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

