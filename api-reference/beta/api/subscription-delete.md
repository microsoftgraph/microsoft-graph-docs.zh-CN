---
title: 删除订阅
description: 删除订阅。
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 8d4630f2141ae254461eb9faffce676a043476f0
ms.sourcegitcommit: 95c1cf4f70a9322d276dc84726457eeaf98169e2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2020
ms.locfileid: "46531468"
---
# <a name="delete-subscription"></a>删除订阅

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

删除订阅。

## <a name="permissions"></a>权限

根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。 若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 支持的资源 | 委派（工作或学校帐户） | 委派（个人 Microsoft 帐户） | 应用程序 |
|:-----|:-----|:-----|:-----|
|[callRecord](../resources/callrecords-callrecord.md) | 不支持 | 不支持 | CallRecords.Read.All  |
|[了 chatmessage](../resources/chatmessage.md) （/teams/{id}/channels/{id}/messages） | ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All | 不支持 | ChannelMessage.Read.All  |
|[了 chatmessage](../resources/chatmessage.md) （/teams/allMessages--组织中的所有频道邮件） | 不支持 | 不支持 | ChannelMessage.Read.All  |
|[了 chatmessage](../resources/chatmessage.md) （/chats/{id}/messages） | Chat.Read、Chat.ReadWrite | 不支持 | Chat.Read.All  |
|[了 chatmessage](../resources/chatmessage.md) （/chats/allMessages--组织中的所有聊天邮件） | 不支持 | 不支持 | Chat.Read.All  |
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

具有委派权限的**了 chatmessage**订阅不支持资源数据（**includeResourceData**必须为 `false` ），并且不需要[加密](/graph/webhooks-with-resource-data)。

具有应用程序权限的**了 chatmessage**订阅包括资源数据，并需要[加密](/graph/webhooks-with-resource-data)。 如果未指定[encryptionCertificate](../resources/subscription.md) ，则订阅创建将失败。 在创建**了 chatmessage**订阅之前，您必须请求访问权限。 有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。 

> **注意：** `/teams/allMessages`，并且 `/chats/allMessages` 当前处于预览阶段。 在预览过程中，可以在不付费的情况下使用此 API，这取决于[Microsoft Api 使用条款](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context)。 但是，使用 API 的应用程序的用户可能需要订阅特定 Microsoft 365 产品。 在正式发行时，Microsoft 可能会要求您或您的客户根据通过 API 访问的数据量支付额外费用。

### <a name="driveitem"></a>driveItem

对 OneDrive 项目的订阅适用其他限制。 这些限制适用于创建和管理（获取、更新和删除）订阅。

在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。 在 OneDrive for Business 上，只可以订阅根文件夹。 对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。 无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。

### <a name="contact-event-and-message"></a>联系人、事件和邮件

对 Outlook 项目的订阅适用其他限制。 这些限制适用于创建和管理（获取、更新和删除）订阅。

- 委派权限仅支持订阅登录用户的邮箱中的文件夹中的项目。 也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。
- 订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：

  - 使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。
  - 切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。

### <a name="presence"></a>状态

**状态**订阅需要[加密](/graph/webhooks-with-resource-data)。 如果未指定[encryptionCertificate](../resources/subscription.md) ，则订阅创建将失败。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
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

##### <a name="request"></a>请求

下面是一个请求示例。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
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

---


##### <a name="response"></a>响应

下面是一个响应示例。
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
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
