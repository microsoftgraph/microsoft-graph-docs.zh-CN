---
title: 创建订阅
description: 订阅侦听器应用程序上的 Microsoft Graph 资源的数据更改时收到通知。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 0640a8de441a07e1abcc02a152f5a9812832db27
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916542"
---
# <a name="create-subscription"></a>创建订阅

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

订阅侦听器应用程序上的 Microsoft Graph 资源的数据更改时收到通知。

## <a name="permissions"></a>权限

创建订阅需要应用程序将为其接收通知的资源的读取的权限。 例如，若要获取有关邮件的通知，您的应用程序需要`Mail.Read`权限。 下表列出了对各个资源所需权限的建议。 若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 资源类型/项        | 权限          |
|-----------------------------|---------------------|
| 联系人                    | Contacts.Read       |
| Conversations               | Group.Read.All      |
| Events                      | Calendars.Read      |
| Messages                    | Mail.Read           |
| 组                      | Group.Read.All      |
| 用户                       | User.Read.All       |
| Drive（用户的 OneDrive）    | Files.ReadWrite     |
| 驱动器 （共享的 SharePoint 内容和驱动器） | Files.ReadWrite.All |
| 安全警报              | SecurityEvents.ReadWrite.All |

> **注意：**/Beta 终结点允许资源最多的应用程序权限。 应用程序权限不支持对话组和 OneDrive 驱动器根项目。

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

在请求正文中，提供[订阅](../resources/subscription.md)对象的 JSON 表示形式。
`clientState`字段是可选的。

此示例请求创建有关当前登录用户接收的新邮件通知的订阅。
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

资源属性的有效值如下：

| 资源类型 | 示例 |
|:------ |:----- |
|邮件|me/mailfolders('inbox')/messages<br />me/messages|
|联系人|me/contacts|
|日历|me/events|
|用户|users|
|组|组|
|对话|groups('*{id}*')/conversations|
|驱动器|me/drive/root|
|安全警报|安全/警告？ $filter = 状态 eq 新建|

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

订阅通知终结点 (中指定`notificationUrl`属性) 必须能够响应验证请求，[设置的用户数据更改的通知](/graph/webhooks#notification-endpoint-validation)中所述。 如果验证失败，请求创建订阅，将返回一个 400 错误请求错误。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
