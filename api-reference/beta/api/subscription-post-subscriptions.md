---
title: 创建订阅
description: 订阅侦听器应用程序, 以在 Microsoft Graph 资源的数据发生更改时接收通知。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: a8b8189780ac0b820551fb885adcf843c9ebe8f4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140164"
---
# <a name="create-subscription"></a>创建订阅

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

订阅侦听器应用程序, 以便在 Microsoft Graph 中的指定资源发生所请求的更改类型时接收通知。

## <a name="permissions"></a>权限

创建订阅时需要对资源使用读取作用域。 例如, 若要获取有关邮件的通知, 您的应用`Mail.Read`程序需要该权限。 
 
 根据所请求的资源和权限类型 (委派或应用程序), 下表中指定的权限是调用此 API 所需的最低特权。 若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 支持的资源 | 委派（工作或学校帐户） | 委派（个人 Microsoft 帐户） | 应用程序 |
|:-----|:-----|:-----|:-----|
|[联系人](../resources/contact.md) | Contacts.Read | Contacts.Read | Contacts.Read |
|[driveItem](../resources/driveitem.md)(用户的个人 OneDrive) | 不支持 | Files.ReadWrite | 不支持 |
|[driveItem](../resources/driveitem.md)(OneDrive for business) | Files.ReadWrite.All | 不支持 | Files.ReadWrite.All |
|[event](../resources/event.md) | Calendars.Read | Calendars.Read | Calendars.Read |
|[group](../resources/group.md) | Group.Read.All | 不支持 | Group.Read.All |
|[组对话](../resources/conversation.md) | Group.Read.All | 不支持 | 不支持 |
|[message](../resources/message.md) | Mail.Read | Mail.Read | Mail.Read |
|[安全警报](../resources/alert.md) | SecurityEvents.ReadWrite.All | 不支持 | SecurityEvents.ReadWrite.All |
|[user](../resources/user.md) | User.Read.All | User.Read.All | User.Read.All |

> **注意:** 对 OneDrive 和 Outlook 项目的订阅有其他限制。 这些限制适用于创建和管理订阅 (获取、更新和删除订阅)。

- 在个人 OneDrive 上, 您可以订阅该驱动器中的根文件夹或任何子文件夹。 在 OneDrive for business 中, 只能订阅根文件夹。 将为订阅的文件夹中的所请求类型的更改发送通知, 或在其层次结构中的任何文件、文件夹或其他**driveItem**实例上发送通知。 您无法订阅不是文件夹的**驱动器**或**driveItem**实例, 例如单个文件。

- 在 Outlook 中, 委派权限仅支持订阅登录用户的邮箱中的文件夹中的项目。 这意味着, 您不能使用委派的权限日历。读取它可订阅其他用户的邮箱中的事件。
- 若要订阅_共享或委托_文件夹中的 Outlook 联系人、事件或邮件的更改通知, 请执行以下操作:

  - 使用相应的应用程序权限订阅租户中_任何_用户的文件夹或邮箱中的项目更改。
  - 请勿使用 Outlook 共享权限 ("联系人"、"共享"、"日历"、"共享"、"邮件"、"已读/写" 等), 因为它们**不**支持对共享或委派文件夹中的项目的更改通知进行订阅。

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

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [subscription](../resources/subscription.md) 对象。

## <a name="example"></a>示例

##### <a name="request"></a>请求

在请求正文中, 提供[订阅](../resources/subscription.md)对象的 JSON 表示形式。
该`clientState`字段是可选的。

此示例请求创建一个订阅, 用于通知当前登录用户接收到的新邮件。
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```

以下是 resource 属性的有效值:

| 资源类型 | 示例 |
|:------ |:----- |
|邮件|me/mailfolders('inbox')/messages<br />me/messages|
|联系人|me/contacts|
|日历|me/events|
|用户|users|
|组|组|
|对话|groups('*{id}*')/conversations|
|驱动器|me/drive/root|
|安全警报|安全/警报？ $filter = 状态 eq ' New '|

##### <a name="response"></a>响应

下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
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
  "changeType": "created,updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

## <a name="notification-endpoint-validation"></a>通知终结点验证

订阅通知终结点 (在`notificationUrl`属性中指定) 必须能够响应验证请求, 如为用户数据中的[更改通知设置通知](/graph/webhooks#notification-endpoint-validation)中所述。 如果验证失败, 则创建订阅的请求将返回400错误的请求错误。

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
    "Error: /api-reference/beta/api/subscription-post-subscriptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
