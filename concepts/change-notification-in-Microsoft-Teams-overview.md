---
title: 使用 Microsoft Graph 更改 Microsoft Teams 资源的通知
description: 了解如何使用 Microsoft Graph API 获取 Microsoft Teams 中资源的更改（创建、更新和删除）通知
author: anandab-msft
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 9433a4c5ee000fa34e125440168b865f1bb16172
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941558"
---
# <a name="change-notifications-for-microsoft-teams-resources-using-microsoft-graph"></a><span data-ttu-id="2196c-103">使用 Microsoft Graph 更改 Microsoft Teams 资源的通知</span><span class="sxs-lookup"><span data-stu-id="2196c-103">Change notifications for Microsoft Teams resources using Microsoft Graph</span></span>

<span data-ttu-id="2196c-104">通过更改通知，可以订阅资源的更改（创建、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="2196c-104">Change notifications enable you to subscribe to changes (create, update, and delete) to a resource.</span></span> <span data-ttu-id="2196c-105">更改通知允许你维护[订阅](/graph/api/resources/webhooks?preserve-view=true)，从而提供低延迟模式。</span><span class="sxs-lookup"><span data-stu-id="2196c-105">Change notifications provide a low latency model by allowing you to maintain a [subscription](/graph/api/resources/webhooks?preserve-view=true).</span></span> <span data-ttu-id="2196c-106">你还可以在通知中获取资源数据，因此避免调用 API 来获取有效负载。</span><span class="sxs-lookup"><span data-stu-id="2196c-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

> <span data-ttu-id="2196c-107">**注意：** 订阅的最长持续时间为 60 分钟；但是，订阅可以续订，直至呼叫方有权访问资源。</span><span class="sxs-lookup"><span data-stu-id="2196c-107">**Note:** The maximum time a subscription can last is 60 minutes; however, subscriptions can be renewed until the caller has permissions to access to resource.</span></span>

## <a name="change-notification-types"></a><span data-ttu-id="2196c-108">更改通知类型</span><span class="sxs-lookup"><span data-stu-id="2196c-108">Change notification types</span></span>
<span data-ttu-id="2196c-109">Microsoft Teams 支持两种类型的更改通知：</span><span class="sxs-lookup"><span data-stu-id="2196c-109">Microsoft Teams supports two types of change notifications:</span></span>
- <span data-ttu-id="2196c-110">**更改通知以跟踪与租户中的资源相关的所有更改** - 例如，你可以订阅租户范围内任何通道中的消息更改，并在租户中的任何通道中创建、更新或删除消息时收到通知。</span><span class="sxs-lookup"><span data-stu-id="2196c-110">**Change notification to track all changes related to a resource across the tenant** - for example, you can subscribe to changes in messages in any channel across the tenant and get notified whenever a message is created, updated, or deleted in any channel in the tenant.</span></span>
- <span data-ttu-id="2196c-111">**更改通知以跟踪特定资源的所有更改** - 例如，你可以订阅特定通道中的消息更改，并在该通道中创建、更新或删除消息时收到通知。</span><span class="sxs-lookup"><span data-stu-id="2196c-111">**Change notification to track all changes for a specific resource** - for example, you can subscribe to changes in messages in a particular channel and get notified whenever a message is created, updated, or deleted in that channel.</span></span>

<span data-ttu-id="2196c-112">有关哪些资源支持哪些类型的更改通知的详细信息，请参阅 [Microsoft Graph 更改通知](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="2196c-112">For details about which resources support which types of change notifications, see [Microsoft Graph change notifications](webhooks.md).</span></span>
 

## <a name="notification-payloads"></a><span data-ttu-id="2196c-113">通知有效负载</span><span class="sxs-lookup"><span data-stu-id="2196c-113">Notification payloads</span></span>

<span data-ttu-id="2196c-114">根据你的订阅，你可以获取包含或不含资源数据的通知。</span><span class="sxs-lookup"><span data-stu-id="2196c-114">Depending on your subscription, you can either get the notification with resource data, or without resource data.</span></span> <span data-ttu-id="2196c-115">通过订阅资源数据，可以在收到通知的同时获取消息有效负载，而无需回调并获取内容。</span><span class="sxs-lookup"><span data-stu-id="2196c-115">Subscribing with resource data allows you to get the message payload along with the notification, which removes the need to call back and get the content.</span></span>

### <a name="notifications-with-resource-data"></a><span data-ttu-id="2196c-116">包含资源数据的通知</span><span class="sxs-lookup"><span data-stu-id="2196c-116">Notifications with resource data</span></span>

<span data-ttu-id="2196c-117">对于包含资源数据的通知，负载如下所示。</span><span class="sxs-lookup"><span data-stu-id="2196c-117">For notifications with resource data, the payload looks like the following.</span></span>  <span data-ttu-id="2196c-118">此有效负载用于对应于聊天消息资源的通知。</span><span class="sxs-lookup"><span data-stu-id="2196c-118">This payload is for a notification corresponding to the chat message resource.</span></span> <span data-ttu-id="2196c-119">实际通知包括 **资源** 和表示已触发该通知的 **resourceData** 属性。</span><span class="sxs-lookup"><span data-stu-id="2196c-119">The actual notification includes the **resource** and **resourceData** properties, which represent the resource that has triggered the notification.</span></span>

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "chats('19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces')/messages('1612289765949')",
        "resourceData": {
            "id": "1612289765949",
            "@odata.type": "#Microsoft.Graph.chatMessage",
            "@odata.id": "chats('19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces')/messages('1612289765949')"
        },
        "encryptedContent": {
            "data": "<<--EncryptedContent-->",
            "dataKey": "<<--EnryptedDataKeyUsedForEncryptingContent-->>",
            "encryptionCertificateId": "<<--IdOfTheCertificateUsedForEncryptingDataKey-->>",
            "encryptionCertificateThumbprint": "<<--ThumbprintOfTheCertificateUsedForEncryptingDataKey-->>"
        },
        "tenantId": "<<--TenantForWhichNotificationWasSent-->>"
    }],
    "validationTokens": ["<<--ValidationTokens-->>"]
}
```

<span data-ttu-id="2196c-120">有关如何验证令牌和解密负载的详细信息，请参阅[设置包含资源数据的更改通知](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="2196c-120">For details about how to validate tokens and decrypt the payload, see [Set up change notifications that include resource data](webhooks-with-resource-data.md).</span></span>

<span data-ttu-id="2196c-121">解密的通知负载如下所示。</span><span class="sxs-lookup"><span data-stu-id="2196c-121">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="2196c-122">上一示例的已解密有效负载符合 [chatMessage](/graph/api/resources/chatMessage?preserve-view=true) 架构。</span><span class="sxs-lookup"><span data-stu-id="2196c-122">The decrypted payload for the previous example conforms to the [chatMessage](/graph/api/resources/chatMessage?preserve-view=true) schema.</span></span> <span data-ttu-id="2196c-123">该负载类似于 GET 操作返回的负载。</span><span class="sxs-lookup"><span data-stu-id="2196c-123">The payload is similar to that returned by GET operations.</span></span>

```json
{
  "id": "1612289992105",
  "replyToId": null,
  "etag": "1612289992105",
  "messageType": "message",
  "createdDateTime": "2021-02-02T18:19:52Z",
  "lastModifiedDateTime": "2021-02-02T18:19:52.105Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "from": {
    "application": null,
    "device": null,
    "user": {
      "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
      "displayName": "Ramjot Singh",
      "userIdentityType": "aadUser"
    },
    "conversation": null
  },
  "body": {
    "contentType": "text",
    "content": "test"
  },
  "channelIdentity": null,
  "attachments": [],
  "mentions": [],
  "policyViolation": null,
  "reactions": [],
  "replies": [],
  "hostedContents": []
}
```

### <a name="notifications-without-resource-data"></a><span data-ttu-id="2196c-124">不含资源数据的通知</span><span class="sxs-lookup"><span data-stu-id="2196c-124">Notifications without resource data</span></span>

<span data-ttu-id="2196c-125">不含资源数据的通知为你提供了足够的信息来进行 GET 调用以获取资源。</span><span class="sxs-lookup"><span data-stu-id="2196c-125">Notifications without resource data give you enough information to make GET calls to get the resource.</span></span> <span data-ttu-id="2196c-126">订阅不含资源数据的通知不需要加密证书（因为不会发送实际资源数据）。</span><span class="sxs-lookup"><span data-stu-id="2196c-126">Subscriptions for notifications without resource data don't require an encryption certificate (because actual resource data is not sent over).</span></span>

<span data-ttu-id="2196c-127">该负载如下所示。</span><span class="sxs-lookup"><span data-stu-id="2196c-127">The payload looks like the following.</span></span> <span data-ttu-id="2196c-128">此负载适用于在频道中发送的消息。</span><span class="sxs-lookup"><span data-stu-id="2196c-128">This payload is for a message sent in a channel.</span></span>

```json
{
  "subscriptionId": "9f9d1ed0-c9cc-42e7-8d80-a7fc4b0cda3c",
  "changeType": "created",
  "tenantId": "<<--TenantForWhichNotificationWasSent-->>",  
  "clientState": "<<--SpecifiedClientState-->>",
  "subscriptionExpirationDateTime": "2021-02-02T11:26:41.0537895-08:00",
  "resource": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2')/messages('1612293113399')",
  "resourceData": {
    "id": "1612293113399",
    "@odata.type": "#Microsoft.Graph.chatMessage",
    "@odata.id": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2')/messages('1612293113399')"
  }
}
```
<span data-ttu-id="2196c-129">上面的示例显示了对应于聊天消息资源的通知。</span><span class="sxs-lookup"><span data-stu-id="2196c-129">Previous example above shows a notification that corresponds to a chat message resource.</span></span> <span data-ttu-id="2196c-130">实际通知包括 **资源** 和表示已触发该通知的 **resourceData** 属性。</span><span class="sxs-lookup"><span data-stu-id="2196c-130">The actual notification includes the **resource** and **resourceData** properties, which represent the resource that has triggered the notification.</span></span> <span data-ttu-id="2196c-131">**资源** 和 **@odata.id** 属性可用于对 Microsoft Graph 进行调用以获取资源的有效负载。</span><span class="sxs-lookup"><span data-stu-id="2196c-131">The **resource** and **@odata.id** properties can be used to make calls to Microsoft Graph to get the payload of the resource.</span></span>

> <span data-ttu-id="2196c-132">**注意** GET 调用将始终返回资源的当前状态。</span><span class="sxs-lookup"><span data-stu-id="2196c-132">**Note** GET calls will always return the current state of the resource.</span></span> <span data-ttu-id="2196c-133">如果在发送通知和检索资源之间更改了资源，则该操作将返回已更新的资源。</span><span class="sxs-lookup"><span data-stu-id="2196c-133">If the resource is changed between when the notification is sent and when the resource is retrieved, the operation will return the updated resource.</span></span>

## <a name="see-also"></a><span data-ttu-id="2196c-134">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2196c-134">See also</span></span>
- [<span data-ttu-id="2196c-135">Microsoft Graph 更改通知</span><span class="sxs-lookup"><span data-stu-id="2196c-135">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="2196c-136">Microsoft Teams API 概述</span><span class="sxs-lookup"><span data-stu-id="2196c-136">Microsoft Teams API overview</span></span>](teams-concept-overview.md)
