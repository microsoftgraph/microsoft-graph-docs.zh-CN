---
title: 创建订阅
description: 订阅侦听器应用程序，以在 Microsoft Graph 资源上的数据发生更改时接收更改通知。
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: f89720d18db554a8700e5d14b2bafd15d92d5f0f
ms.sourcegitcommit: 74a1fb3874e04c488e1b87dcee80d76cc586c1f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51031028"
---
# <a name="create-subscription"></a>创建订阅

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

订阅侦听器应用程序，以在 Microsoft Graph 中指定资源发生的更改属于请求的更改类型时接收更改通知。

请参阅" [权限](#permissions) 部分中的表格，了解支持订阅以更改通知的资源列表。

## <a name="permissions"></a>权限

创建订阅需要对资源的读取权限。 例如，若要获取邮件更改通知，您的应用程序需要 Mail.Read 权限。 

根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。 若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。

| 支持的资源 | 委派（工作或学校帐户） | 委派（个人 Microsoft 帐户） | 应用程序 |
|:-----|:-----|:-----|:-----|
|[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords) | 不支持 | 不支持 | CallRecords.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages) | ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All | 不支持 | ChannelMessage.Read.Group*、ChannelMessage.Read.All  |
|[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息） | 不支持 | 不支持 | ChannelMessage.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages) | Chat.Read、Chat.ReadWrite | 不支持 | Chat.Read.All  |
|[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息） | 不支持 | 不支持 | Chat.Read.All  |
|[contact](../resources/contact.md) | Contacts.Read | Contacts.Read | Contacts.Read |
|[driveItem](../resources/driveitem.md)（用户的个人 OneDrive） | 不支持 | Files.ReadWrite | 不支持 |
|[driveItem](../resources/driveitem.md) (OneDrive for Business) | Files.ReadWrite.All | 不支持 | Files.ReadWrite.All |
|[事件](../resources/event.md) | Calendars.Read | Calendars.Read | Calendars.Read |
|[组](../resources/group.md) | Group.Read.All | 不支持 | Group.Read.All |
|[组对话](../resources/conversation.md) | Group.Read.All | 不支持 | 不支持 |
|[列表](../resources/list.md) | Sites.ReadWrite.All | 不支持 | Sites.ReadWrite.All |
|[邮件](../resources/message.md) | Mail.ReadBasic、Mail.Read | Mail.ReadBasic、Mail.Read | Mail.ReadBasic、Mail.Read |
|[状态](../resources/presence.md) | Presence.Read.All | 不支持 | 不支持 |
|[打印机](../resources/printer.md) | 不支持 | 不支持 | Printer.Read.All、Printer.ReadWrite.All |
|[printTaskDefinition](../resources/printtaskdefinition.md) | 不支持 | 不支持 | PrintTaskDefinition.ReadWrite.All |
|安全[警报](../resources/alert.md) | SecurityEvents.ReadWrite.All | 不支持 | SecurityEvents.ReadWrite.All |
|[todoTask](../resources/todotask.md) | Tasks.ReadWrite | Tasks.ReadWrite | 不支持 |
|[用户](../resources/user.md) | User.Read.All | User.Read.All | User.Read.All |

> **注意**：标有 * 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a>driveItem

其他限制适用于 OneDrive 项目的订阅。 这些限制适用于订阅的创建和管理（获取、更新和删除）。

在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。 在 OneDrive for Business 上，只可以订阅根文件夹。 对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。 无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。

### <a name="contact-event-and-message"></a>联系人、事件和消息

其他限制适用于 Outlook 项目的订阅。 这些限制适用于订阅的创建和管理（获取、更新和删除）。

- 委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。 例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。
- 订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：

  - 使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。
  - 切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。

### <a name="presence"></a>状态

**状态** 订阅需要 [加密](/graph/webhooks-with-resource-data)。 如果未指定 [encryptionCertificate](../resources/subscription.md)，则订阅创建将失败。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a>请求标头

| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 [响应](../resources/subscription.md) 代码和 subscription 对象。

要详细了解错误返回方式，请参阅[错误响应][error-response]。

## <a name="example"></a>示例

### <a name="request"></a>请求

在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。
`clientState` 和 `latestSupportedTlsVersion` 是可选字段。

此请求为当前登录用户收到的新邮件更改通知创建订阅。

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

---

在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。
`clientState` 和 `latestSupportedTlsVersion` 是可选字段。

#### <a name="resources-examples"></a>资源示例

以下是资源属性的有效值。

| 资源类型 | 示例 |
|:------ |:----- |
|[通话记录](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[聊天消息](../resources/chatmessage.md) | `chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages` |
|[联系人](../resources/contact.md)|`me/contacts`|
|[对话](../resources/conversation.md)|`groups('{id}')/conversations`|
|[驱动器](../resources/driveitem.md)|`me/drive/root`|
|[事件](../resources/event.md)|`me/events`|
|[组](../resources/group.md)|`groups`|
|[列表](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[邮件](../resources/message.md)|`me/mailfolders('inbox')/messages`, `me/messages`|
|[状态](../resources/presence.md)| `/communications/presences/{id}` (单个用户) ， (`/communications/presences?$filter=id in ({id},{id}…)` 多个) |
|[打印机](../resources/printer.md) |`print/printers/{id}/jobs`|
|[PrintTaskDefinition](../resources/printtaskdefinition.md)|`print/taskDefinitions/{id}/tasks`|
|[用户](../resources/user.md)|`users`|
|[todoTask](../resources/todotask.md) | `/me/todo/lists/{todoTaskListId}/tasks`
|[安全警报](../resources/alert.md)|`security/alerts?$filter=status eq 'NewAlert'`|

> **注意：** 以 `me` 开头的任何路径也可与 `users/{id}`（而不是 `me`）一起使用，从而以特定用户为目标，而不是以当前用户为目标。

### <a name="response"></a>响应

以下示例显示了相应的响应。 

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 252

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

### <a name="notification-endpoint-validation"></a>通知终结点验证

notificationUrl (中指定的订阅通知终结点) 必须能够响应验证请求，如设置用户数据更改[的通知中所述](/graph/webhooks#notification-endpoint-validation)。 如果验证失败，创建订阅请求返回错误“400 请求无效”。

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


