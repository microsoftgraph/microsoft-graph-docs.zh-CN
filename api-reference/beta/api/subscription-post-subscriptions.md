---
title: 创建订阅
description: 订阅侦听器应用程序，以便在 Microsoft Graph 资源上的数据发生更改时接收更改通知。
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 36555a946aa9092d5cab6e27548a16ba783d738e
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598134"
---
# <a name="create-subscription"></a>创建订阅

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

订阅侦听器应用程序，以在 Microsoft Graph 中指定资源发生的更改属于请求的更改类型时接收更改通知。

## <a name="permissions"></a>权限

创建订阅需要对资源具有读取权限。 例如，若要获取邮件的更改通知，您的应用程序需要具有邮件读取权限。 
 
 根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。 若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 支持的资源 | 委派（工作或学校帐户） | 委派（个人 Microsoft 帐户） | 应用程序 |
|:-----|:-----|:-----|:-----|
|[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords) | 不支持 | 不支持 | CallRecords.Read.All  |
|[了 chatmessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)  | ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All | 不支持 | ChannelMessage.Read.All  |
|[了 chatmessage](../resources/chatmessage.md) (/teams/allmessages--组织中的所有频道邮件)  | 不支持 | 不支持 | ChannelMessage.Read.All  |
|[了 chatmessage](../resources/chatmessage.md) (/chats/{id}/messages)  | Chat.Read、Chat.ReadWrite | 不支持 | Chat.Read.All  |
|[了 chatmessage](../resources/chatmessage.md) (/chats/allmessages--组织中的所有聊天邮件)  | 不支持 | 不支持 | Chat.Read.All  |
|[联系人](../resources/contact.md) | Contacts.Read | Contacts.Read | Contacts.Read |
|[driveItem](../resources/driveitem.md)（用户的个人 OneDrive） | 不支持 | Files.ReadWrite | 不支持 |
|[driveItem](../resources/driveitem.md) (OneDrive for Business) | Files.ReadWrite.All | 不支持 | Files.ReadWrite.All |
|[事件](../resources/event.md) | Calendars.Read | Calendars.Read | Calendars.Read |
|[组](../resources/group.md) | Group.Read.All | 不支持 | Group.Read.All |
|[组对话](../resources/conversation.md) | Group.Read.All | 不支持 | 不支持 |
|[列表](../resources/list.md) | Sites.ReadWrite.All | 不支持 | Sites.ReadWrite.All |
|[邮件](../resources/message.md) | Mail.ReadBasic、Mail.Read | Mail.ReadBasic、Mail.Read | Mail.ReadBasic、Mail.Read |
|[状态](../resources/presence.md) | Presence.Read.All | 不支持 | 不支持 |
|安全[警报](../resources/alert.md) | SecurityEvents.ReadWrite.All | 不支持 | SecurityEvents.ReadWrite.All |
|[用户](../resources/user.md) | User.Read.All | User.Read.All | User.Read.All |

### <a name="chatmessage"></a>chatMessage

具有委派权限的**了 chatmessage**订阅不支持资源数据 (**includeResourceData**必须 `false`) ，并且不需要[加密](/graph/webhooks-with-resource-data)。

具有应用程序权限的**了 chatmessage**订阅包括资源数据，并需要[加密](/graph/webhooks-with-resource-data)。 如果未指定[encryptionCertificate](../resources/subscription.md) ，则订阅创建将失败。 在创建**了 chatmessage**订阅之前，您必须请求访问权限。 有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。 

> **注意：** `/teams/allMessages`，并且 `/chats/allMessages` 当前处于预览阶段。 在预览过程中，可以在不付费的情况下使用此 API，这取决于[Microsoft Api 使用条款](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context)。 但是，使用 API 的应用程序的用户可能需要订阅特定 Microsoft 365 产品。 在正式发行时，Microsoft 可能会要求您或您的客户根据通过 API 访问的数据量支付额外费用。

### <a name="driveitem"></a>driveItem

对 OneDrive 项目的订阅适用其他限制。 这些限制适用于创建以及管理 (获取、更新和删除) 订阅。

在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。 在 OneDrive for Business 上，只可以订阅根文件夹。 对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。 无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。

### <a name="contact-event-and-message"></a>联系人、事件和邮件

对 Outlook 项目的订阅适用其他限制。 这些限制适用于创建以及管理 (获取、更新和删除) 订阅。

- 委派权限仅支持订阅登录用户的邮箱中的文件夹中的项目。 也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。
- 订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：

  - 使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。
  - 切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。

### <a name="presence"></a>状态

**状态**订阅需要[加密](/graph/webhooks-with-resource-data)。 如果未指定[encryptionCertificate](../resources/subscription.md) ，则订阅创建将失败。

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

如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[订阅](../resources/subscription.md)对象。

要详细了解错误返回方式，请参阅[错误响应][error-response]。

## <a name="example"></a>示例

### <a name="request"></a>请求

在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。
`clientState` 和 `latestSupportedTlsVersion` 是可选字段。

此请求创建订阅，以获取当前登录用户接收到的新邮件的更改通知。

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

---

以下是 resource 属性的有效值。

| 资源类型 | 示例 |
|:------ |:----- |
|[通话记录](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[聊天消息](../resources/chatmessage.md) | `chats/{id}/messages`, `chats/allMessages`, `teams/{id}/channels/{id}/messages`, `teams/allMessages` |
|[联系人](../resources/contact.md)|`me/contacts`|
|[对话](../resources/conversation.md)|`groups('{id}')/conversations`|
|[Drives](../resources/driveitem.md)|`me/drive/root`|
|[Events](../resources/event.md)|`me/events`|
|[组](../resources/group.md)|`groups`|
|[List](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[邮件](../resources/message.md)|`me/mailfolders('inbox')/messages`, `me/messages`|
|[Shell](../resources/presence.md)| `/communications/presences/{id}` (单个用户) ， `/communications/presences?$filter=id in ({id},{id}…)` (多个用户) |
|[用户](../resources/user.md)|`users`|
|[安全警报](../resources/alert.md)|`security/alerts?$filter=status eq 'New'`|

> **注意：** 以此开头的任何路径 `me` 也可以与 `users/{id}` `me` 特定用户而不是当前用户的目标一起使用。

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
  "latestSupportedTlsVersion": "v1_2"
}
```

## <a name="notification-endpoint-validation"></a>通知终结点验证

 (在**notificationUrl**属性中指定的订阅通知终结点) 必须能够响应验证请求，如[设置用户数据中的更改通知](/graph/webhooks#notification-endpoint-validation)中所述。 如果验证失败，创建订阅请求返回错误“400 请求无效”。

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
