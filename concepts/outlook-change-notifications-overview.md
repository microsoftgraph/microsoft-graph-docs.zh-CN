---
title: Microsoft Graph 中 Outlook 资源的更改通知
description: 了解如何使用 Microsoft Graph API 获取 Outlook 中资源的更改（创建、更新和删除）通知
author: abheek-das
ms.localizationpriority: high
ms.prod: outlook
ms.custom: scenarios:getting-started
ms.openlocfilehash: 04361ff86fc4106d0792b43b2ea7638a41e04b7c
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337894"
---
# <a name="change-notifications-for-outlook-resources-in-microsoft-graph"></a>Microsoft Graph 中 Outlook 资源的更改通知

Microsoft Graph API 允许你订阅对资源的更改（包括资源的创建、更新或删除）以及通过 Webhook 接收通知。 [订阅](/graph/api/resources/webhooks)指定要监视的特定资源的所需更改类型，以及终结点接收这些更改通知的 URL。 设置订阅可减少开销，否则需要查询和比较资源来推断任何更改。 可以选择在订阅请求中指定要加密的资源数据，并在通知中包含已更改的资源数据，从而保存单独的后续 API 调用以获取资源有效负载。

对于所有应用程序，每个邮箱的 Outlook 资源活动订阅数上限为 1000 个。 你可以订阅邮箱中的联系人、事件或邮件中的更改。

## <a name="subscribe-to-changes-in-contacts-calendar-or-mail"></a>订阅联系人、日历或邮件中的更改

若要订阅 Outlook 资源的更改通知，请先创建 [订阅](/graph/api/resources/subscription)。

以下 Outlook 资源支持 [更改通知](/graph/api/resources/changenotification) 包含或不包含有效负载中资源数据的订阅。

- [联系人](/graph/api/resources/contact)
- [event](/graph/api/resources/event)
- [message](/graph/api/resources/message)

## <a name="create-a-subscription"></a>创建订阅

若要 [创建订阅](webhooks.md#creating-a-subscription)，请指定要接收通知的 Outlook 资源和更改类型（创建、更新或删除）。 请参阅[示例](#example-1-create-a-subscription-to-get-change-notifications-without-resource-data-when-the-user-receives-a-new-message)。

### <a name="request-permissions"></a>请求权限

[!INCLUDE [outlook-subscription-notes](../includes/outlook-subscription-notes.md)]

根据资源，下表中指定的权限是调用此 API 所需的最低权限。

| 资源| 支持的资源路径| 委派（工作或学校帐户）| 委派（个人 Microsoft 帐户）| 应用程序|
|:--------|:------------------------|:----------------------------------|:--------------------------------------|:-----------|
|[联系人](/graph/api/resources/contact) | 对用户邮箱中的所有个人联系人更改： <br>`/me/contacts`<br>`/users/{id}/contacts`<br>对用户 contactFolder 中的联系人的更改：<br>`/users/{id}/contactFolders/{id}/contacts` | Contacts.Read | Contacts.Read | Contacts.Read |
|[event](/graph/api/resources/event)     | 对用户邮箱中的所有事件更改： <br>`/me/events`<br>`/users/{id}/events` | Calendars.Read | Calendars.Read | Calendars.Read |
|[邮件](/graph/api/resources/message) | 对用户邮箱中的所有邮件更改： <br>`/me/messages`<br>`/users/{id}/messages`<br>对用户 mailFolder 中的邮件的更改：<br>`/users/{id}/mailFolders/{id}/messages` | Mail.ReadBasic、Mail.Read | Mail.ReadBasic、Mail.Read | Mail.ReadBasic、Mail.Read |

### <a name="include-resource-data-in-notification-payload-preview"></a>在通知有效负载中包括资源数据（预览版）

> [!NOTE]
> 包含 Outlook 资源的资源数据的通知目前仅在 Microsoft Graph beta 终结点中可用。 

若要在更改通知中包含资源数据，则 **必须** 指定以下属性，以及 [创建订阅](webhooks.md#creating-a-subscription)时通常包含的属性：

- **includeResourceData**：将此属性设置为 `true` 以显式请求资源数据。
- **resource**：此属性指定资源 URL。 请确保使用 `$select` 查询参数显式指定要包含在通知有效负载中的 Outlook 资源属性。
  > **注意：** 请勿在 URL 中包含除 **singleValueExtendedProperties** 或 **multiValueExtendedProperties** 之外的`$top`、`$skip`、`$orderby`、`$select=Body,UniqueBody`、`$expand`。
- **encryptionCertificate**： 此属性仅包含 Microsoft Graph 用于加密资源数据的公钥。 保留相应的私钥，以[解密内容](webhooks-with-resource-data.md#decrypting-resource-data-from-change-notifications)。
- **encryptionCertificateId**： 此属性是你自己的证书标识符。 使用此 ID 在每个更改通知中匹配用于解密的证书。

请参阅 [示例](#example-2-create-a-subscription-to-get-change-notifications-with-resource-data-when-the-user-receives-a-new-message-preview)，以订阅使用 **邮件** 资源的资源数据的更改通知。


### <a name="refine-the-conditions-for-a-notification"></a>优化通知的条件
可以使用 `$filter` 查询参数进一步优化通知的条件。 请参阅[示例](#example-3-create-a-subscription-to-get-change-notifications-with-resource-data-for-a-message-based-on-a-condition-preview)。

`$filter`的一个常见应用是在特定资源属性发生更改时收到通知。 例如，可以使用 `$filter` 订阅文件夹中的未读邮件（**isRead** 属性为 `false`），并包括所有更改类型：
- 将邮件添加到文件夹或将其标记为未读将触发 `Created` 通知。
- 读取文件夹中的邮件或将其标记为已读将触发 `Deleted` 通知。
- 更改文件夹中 **邮件** 资源的任何属性（**isRead** 除外）将触发`Updated`通知。

如果在创建订阅时不使用 `$filter` ：
- 将邮件添加到文件夹将生成 `Created` 通知。
- 读取文件夹中的邮件、将邮件标记为已读或更改该文件夹中邮件的任何其他属性将生成 `Updated` 通知。
- 删除邮件将生成 `Delete` 通知。

### <a name="subscribe-to-lifecycle-notifications"></a>订阅生命周期通知
Outlook **联系人**、**事件** 和 **邮件** 资源也支持订阅生命周期通知。 删除应用订阅或错过某些更改通知时，需要生命周期通知。 应用程序应实现逻辑以进行检测并恢复丢失的内容，以及恢复连续更改通知流程。 若要了解详细信息，请参阅[订阅生命周期通知](webhooks-lifecycle.md)。

### <a name="keep-track-of-subscription-lifetime"></a>跟踪订阅生命周期
请确保在订阅过期之前[延长](/graph/api/subscription-update)订阅。 没有 Outlook 资源数据的订阅的最大生命周期为 4230 分钟（不到 3 天），有资源数据的订阅的最大生命周期为 1 天。 

如果失去之前为订阅授予的权限，并且此时订阅过期，请再次请求权限以[创建](/graph/api/subscription-post-subscriptions)新订阅。

## <a name="receive-notification-payloads"></a>接收通知有效负载

根据订阅，通知可能包含资源数据。 具有资源数据的订阅允许你获取资源有效负载和通知，从而避免单独的 API 调用以获取更改的资源数据的开销。

### <a name="receive-notifications-with-resource-data-preview"></a>接收包含资源数据的通知（预览版）

下面是包含 **邮件** 资源的资源数据的通知有效负载示例。 **resource** 和 **resourceData** 属性对应于触发通知的 **邮件** 实例。 使用 **encryptedContent** 属性可解密资源数据。

```json
{
    "value": [
      {
        "subscriptionId": "dfd11b2f-8222-4189-9545-4205c95d6235",
        "subscriptionExpirationDateTime": "2021-12-31T16:16:44.9907405+05:30",
        "changeType": "created",
        "resource": "Users('722effaf-0433-4272-9ac4-d5ec11c3cd77')/messages('AAMkAGUwNjQ4ZjIxLTQ3Y2Y8AAA=')",
        "clientState": "<<--SpecifiedClientState-->>",
        "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
        "encryptedContent": {
          "data": "<<--EncryptedContent-->>",
          "dataKey": "<<--EnryptedDataKeyUsedForEncryptingContent-->>",        
          "dataSignature": "Qw/9ubWeUYJPWWXvNiGgct2FkNG2MXTRm/BLUpJM66k=",
          "encryptionCertificateId": "<<--IdOfTheCertificateUsedForEncryptingDataKey-->>",
          "encryptionCertificateThumbprint": "<<--ThumbprintOfTheCertificateUsedForEncryptingDataKey-->>"
        },
        "resourceData": {
          "@odata.type": "#microsoft.graph.message",
          "@odata.id": "Users('722effaf-0433-4272-9ac4-d5ec11c3cd77')/messages('AAMkAGUwNjQ4ZjIxLTQ3Y2Y8AAA=')",
          "@odata.etag": "W/\"CQAAABYAAACQ2fKdhq8oSKEDSVrdi3lRAAGDUR8n\"",
          "id": "AAMkAGUwNjQ4ZjIxLTQ3Y2Y8AAA="
        }
      }
    ]
    "validationTokens": ["<<--ValidationTokens-->>"]
}
```

有关如何验证令牌和解密负载的详细信息，请参阅[设置包含资源数据的更改通知](webhooks-with-resource-data.md)。

下面是解密的通知有效负载的示例。 解密的有效负载符合 Outlook [邮件](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true)架构。 该有效负载类似于[GET 邮件](/graph/api/message-get?view=graph-rest-beta&preserve-view=true)操作返回的负载。 但是，通知有效负载仅包含在订阅的 **资源** 属性中使用 `$select` 参数指定的属性。 其他 Outlook 资源（如[联系人](/graph/api/resources/contact?view=graph-rest-beta&preserve-view=true)和[事件](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true)）的通知有效负载遵循其各自的架构。 

```json
{
    "receivedDateTime@odata.type":"#DateTimeOffset",
    "receivedDateTime":"2021-12-30T10:53:35Z",
    "subject":"TEST MESSAGE FOR RICH NOTIFICATIONS",
    "bodyPreview":"Hello,\r\n\r\nWhat\u2019s up?\r\n\r\nThanks\r\nMegan",
    "importance@odata.type":"#microsoft.graph.importance",
    "importance":"normal",
    "from": {
        "@odata.type":"#microsoft.graph.recipient",
        "emailAddress": {
            "@odata.type":"#microsoft.graph.emailAddress",
            "name":"Megan Brown",
            "address":"Megan.Brown@microsoft.com"
        }
    }
}
```

### <a name="receive-notifications-without-resource-data"></a>接收不含资源数据的通知

不含资源数据的通知为你提供了足够的信息来进行 GET 调用以获取资源。 订阅不含资源数据的通知不需要加密证书，因为不会发送实际资源数据。

下一个示例显示与 Outlook **邮件** 资源对应的通知有效负载。 它包括 **resource** 和 **resourceData** 属性，这些属性表示触发通知的资源。 使用 **resource** 和 **@odata.id** 属性对 Microsoft Graph 进行调用以获取资源的有效负载。

> **注意** GET 调用始终返回资源的当前状态。 如果在发送通知和检索资源之间更改了资源，则操作会在检索时返回资源的状态。


```json
"value": [
 {
   "subscriptionId": "c6126aa3-0ed8-412f-a988-71e6cee627c4",
   "subscriptionExpirationDateTime": "2022-01-02T03:12:18.2257768+05:30",
   "changeType": "created",    
   "resource": "Users/622eaaff-0683-4862-9de4-f2ec83c2bd98/Messages/AAMkAGUwNjQ4ZjIxAAA=",
   "resourceData": {      
     "@odata.type": "#Microsoft.Graph.Message",
     "@odata.id": "Users/622eaaff-0683-4862-9de4-f2ec83c2bd98/Messages/AAMkAGUwNjQ4ZjIAAA=",
     "@odata.etag": "W/\"CQAAABYAAACQ2fKdhq8oSKEDSVrdi3lRAAGDUUXn\"",
     "id": "AAMkAGUwNjQ4ZjIxAAA="
   },
   "clientState": "<<--SpecifiedClientState-->>",
   "tenantId": "<<--TenantForWhichNotificationWasSent-->>"
 }
]
```


## <a name="examples"></a>示例

### <a name="example-1-create-a-subscription-to-get-change-notifications-without-resource-data-when-the-user-receives-a-new-message"></a>示例 1：创建订阅以在用户收到新消息时获取不含资源数据的更改通知
以下示例请求在用户邮箱中创建邮件的通知。

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_subscription_withoutresourcedata_for_message_resource"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
    "changeType": "created",
    "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
    "resource": "users/622eaaff-0683-4862-9de4-f2ec83c2bd98/messages",
    "expirationDateTime": "2021-07-07T21:42:18.2257768+00:00",
    "clientState": "secretClientState"
}
```

#### <a name="response"></a>响应
下面展示了示例响应。 
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
    "id": "5522bd62-7c96-4530-85b0-00b916f6151a",
    "resource": "users/622eaaff-0683-4862-9de4-f2ec83c2bd98/messages",
    "applicationId": "507c3b9a-67b8-463d-88a2-15a8cefb2111",
    "changeType": "created",
    "clientState": "secretClientState",
    "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
    "notificationQueryOptions": null,
    "notificationContentType": null,
    "lifecycleNotificationUrl": null,
    "expirationDateTime": "2022-01-01T21:42:18.2257768Z",
    "creatorId": "a4c7bd34-4f3b-46b7-a25d-b63c1e2a2842",
    "includeResourceData": null,
    "latestSupportedTlsVersion": "v1_2",
    "encryptionCertificate": null,
    "encryptionCertificateId": null,
    "notificationUrlAppId": null
}
```

### <a name="example-2-create-a-subscription-to-get-change-notifications-with-resource-data-when-the-user-receives-a-new-message-preview"></a>示例 2：创建订阅，以便在用户收到新邮件时获取包含资源数据的更改通知（预览版）
以下示例订阅在用户邮箱中创建邮件的带有资源数据的通知。 使用 `$select` 查询参数指定要包含在通知有效负载中的 **邮件** 资源的属性。

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_subscription_withresourcedata_for_message_resource"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{ 
    "changeType": "created",
    "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
    "resource": "users/622eaaff-0683-4862-9de4-f2ec83c2bd98/messages?$select=Subject,bodyPreview,importance,receivedDateTime,from",
    "expirationDateTime": "2022-01-01T21:42:18.2257768+00:00",
    "clientState": "secretClientValue",
    "includeResourceData": true,
    "encryptionCertificate": "MIIDMzCCAhugAwIBAgIQE7D+++Dk1hKQBqWA==",
    "encryptionCertificateId": "testCertificateId"
}
```

#### <a name="response"></a>响应
下面展示了示例响应。 
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
    "id": "178eec5f-cf3c-4e7e-8a9c-8640deb5b5c5",
    "resource": "users/622eaaff-0683-4862-9de4-f2ec83c2bd98/messages?$select=Subject,bodyPreview,importance,receivedDateTime,from",
    "applicationId": "507c3b9a-67b8-463d-88a2-15a8cefb2111",
    "changeType": "created",
    "clientState": "secretClientValue",
    "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
    "notificationQueryOptions": null,
    "notificationContentType": null,
    "lifecycleNotificationUrl": null,
    "expirationDateTime": "2022-01-01T12:32:35.1582696Z",
    "creatorId": "a4c7bd34-4f3b-46b7-a25d-b63c1e2a2842",
    "includeResourceData": true,
    "latestSupportedTlsVersion": "v1_2",
    "encryptionCertificate": "MIIDMzCCAhugAwIBAgIQE7D+++Dk1hKQBqWA==",
    "encryptionCertificateId": "testCertificateId",
    "notificationUrlAppId": null
}
```

### <a name="example-3-create-a-subscription-to-get-change-notifications-with-resource-data-for-a-message-based-on-a-condition-preview"></a>示例 3：创建订阅以获取包含基于条件的消息的资源数据的更改通知（预览版）
下面的示例使用资源数据订阅在草稿文件夹中创建包含一个或多个附件且具有高重要性的邮件的通知。

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "create_subscription_withresourcedata_for_message_resource_basedonfilter"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{ 
    "changeType": "created",
    "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
    "resource": "me/mailfolders('Drafts')/messages?$select=Subject,bodyPreview&$filter=hasAttachments eq true AND importance eq 'High'",
    "expirationDateTime": "2022-01-01T21:42:18.2257768+00:00",
    "clientState": "secretClientValue",
    "includeResourceData": true,
    "encryptionCertificate": "MIIDMzCCAhugAwIBAgIQE7D+++Dk1hKQBqWA==",
    "encryptionCertificateId": "testCertificateId"
}
```

#### <a name="response"></a>响应
下面展示了示例响应。 
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
    "id": "239dbc5f-cf3c-4e7e-8c9c-3340abc5b5c5",
    "resource": "me/mailfolders('Drafts')/messages?$select=Subject,bodyPreview&$filter=hasAttachments eq true AND importance eq 'High'",
    "applicationId": "507c3b9a-67b8-463d-88a2-15a8cefb2111",
    "changeType": "created",
    "clientState": "secretClientValue",
    "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
    "notificationQueryOptions": null,
    "notificationContentType": null,
    "lifecycleNotificationUrl": null,
    "expirationDateTime": "2022-01-20T12:32:35.1582696Z",
    "creatorId": "a4c7bd34-4f3b-46b7-a25d-b63c1e2a2842",
    "includeResourceData": true,
    "latestSupportedTlsVersion": "v1_2",
    "encryptionCertificate": "MIIDMzCCAhugAwIBAgIQE7D+++Dk1hKQBqWA==",
    "encryptionCertificateId": "testCertificateId",
    "notificationUrlAppId": null
}
```

## <a name="see-also"></a>另请参阅
- [Microsoft Graph 更改通知](webhooks.md)
- [设置包含资源数据的更改通知](webhooks-with-resource-data.md)
- [Outlook 邮件 API 概述](outlook-mail-concept-overview.md)
- [Outlook 联系人 API 概述](outlook-contacts-concept-overview.md)
- [Outlook 日历 API 概述](outlook-calendar-concept-overview.md)
