---
title: 使用 Microsoft Graph 获取聊天的更改通知
description: 了解如何使用 Microsoft Graph API 获取聊天更改（创建和更新）的通知。
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 246a0236b705f98835a4c8131a04e28d3d8c846c
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/10/2021
ms.locfileid: "53367025"
---
# <a name="get-change-notifications-for-chats-using-microsoft-graph"></a><span data-ttu-id="9bef8-103">使用 Microsoft Graph 获取聊天的更改通知</span><span class="sxs-lookup"><span data-stu-id="9bef8-103">Get change notifications for chats using Microsoft Graph</span></span>

<span data-ttu-id="9bef8-104">更改通知使你能够订阅聊天的更改（创建和更新）。</span><span class="sxs-lookup"><span data-stu-id="9bef8-104">Change notifications enable you to subscribe to changes (create and update) to chats.</span></span> <span data-ttu-id="9bef8-105">每当创建或更新聊天时，你都可以收到通知。</span><span class="sxs-lookup"><span data-stu-id="9bef8-105">You can get notified whenever a chat is created or updated.</span></span> <span data-ttu-id="9bef8-106">你还可以在通知中获取资源数据，因此避免调用 API 来获取有效负载。</span><span class="sxs-lookup"><span data-stu-id="9bef8-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

## <a name="subscribe-to-changes-in-any-chat-at-tenant-level"></a><span data-ttu-id="9bef8-107">在租户级别订阅任何聊天中的更改</span><span class="sxs-lookup"><span data-stu-id="9bef8-107">Subscribe to changes in any chat at tenant level</span></span>

<span data-ttu-id="9bef8-108">要获取与租户中任何聊天相关的所有更改（创建、更新和删除）的更改通知，请订阅 `/chats`。</span><span class="sxs-lookup"><span data-stu-id="9bef8-108">To get change notifications for all changes (create and update) related to any chat in a tenant, subscribe to `/chats`.</span></span> <span data-ttu-id="9bef8-109">此资源支持在通知中[包括资源数据](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="9bef8-109">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

### <a name="permissions"></a><span data-ttu-id="9bef8-110">权限</span><span class="sxs-lookup"><span data-stu-id="9bef8-110">Permissions</span></span>

|<span data-ttu-id="9bef8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9bef8-111">Permission type</span></span>      | <span data-ttu-id="9bef8-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9bef8-112">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="9bef8-113">支持的版本</span><span class="sxs-lookup"><span data-stu-id="9bef8-113">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="9bef8-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9bef8-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9bef8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9bef8-115">Not supported.</span></span> | <span data-ttu-id="9bef8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9bef8-116">Not supported.</span></span> |
|<span data-ttu-id="9bef8-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9bef8-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bef8-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9bef8-118">Not supported.</span></span>    | <span data-ttu-id="9bef8-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="9bef8-119">Not supported.</span></span> |
|<span data-ttu-id="9bef8-120">Application</span><span class="sxs-lookup"><span data-stu-id="9bef8-120">Application</span></span> | <span data-ttu-id="9bef8-121">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bef8-121">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span>   | <span data-ttu-id="9bef8-122">beta 版</span><span class="sxs-lookup"><span data-stu-id="9bef8-122">beta</span></span>|

### <a name="example"></a><span data-ttu-id="9bef8-123">示例</span><span class="sxs-lookup"><span data-stu-id="9bef8-123">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-changes-in-a-particular-chat"></a><span data-ttu-id="9bef8-124">订阅特定聊天中的更改</span><span class="sxs-lookup"><span data-stu-id="9bef8-124">Subscribe to changes in a particular chat</span></span>


<span data-ttu-id="9bef8-125">要获取特定聊天相关的所有更改的更改通知，请订阅 `/chats/{id}`。</span><span class="sxs-lookup"><span data-stu-id="9bef8-125">To get change notifications for all changes related to a particular chat, subscribe to `/chats/{id}`.</span></span> <span data-ttu-id="9bef8-126">此资源支持在通知中[包括资源数据](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="9bef8-126">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

### <a name="permissions"></a><span data-ttu-id="9bef8-127">权限</span><span class="sxs-lookup"><span data-stu-id="9bef8-127">Permissions</span></span>

|<span data-ttu-id="9bef8-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="9bef8-128">Permission type</span></span>      | <span data-ttu-id="9bef8-129">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9bef8-129">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="9bef8-130">支持的版本</span><span class="sxs-lookup"><span data-stu-id="9bef8-130">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="9bef8-131">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9bef8-131">Delegated (work or school account)</span></span> | <span data-ttu-id="9bef8-132">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9bef8-132">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="9bef8-133">beta 版</span><span class="sxs-lookup"><span data-stu-id="9bef8-133">beta</span></span> |
|<span data-ttu-id="9bef8-134">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9bef8-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bef8-135">不支持。</span><span class="sxs-lookup"><span data-stu-id="9bef8-135">Not supported.</span></span>    | <span data-ttu-id="9bef8-136">不支持。</span><span class="sxs-lookup"><span data-stu-id="9bef8-136">Not supported.</span></span> |
|<span data-ttu-id="9bef8-137">应用程序</span><span class="sxs-lookup"><span data-stu-id="9bef8-137">Application</span></span> | <span data-ttu-id="9bef8-138">ChatSettings.Read.Chat *、ChatSettings.ReadWrite.Chat*、Chat.Manage.Chat\*、Chat.ReadBasic.All、Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bef8-138">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> | <span data-ttu-id="9bef8-139">beta</span><span class="sxs-lookup"><span data-stu-id="9bef8-139">beta</span></span> |

> <span data-ttu-id="9bef8-140">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="9bef8-140">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="example"></a><span data-ttu-id="9bef8-141">示例</span><span class="sxs-lookup"><span data-stu-id="9bef8-141">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```


### <a name="notifications-with-resource-data"></a><span data-ttu-id="9bef8-142">包含资源数据的通知</span><span class="sxs-lookup"><span data-stu-id="9bef8-142">Notifications with resource data</span></span>

<span data-ttu-id="9bef8-143">对于包含资源数据的通知，负载如下所示。</span><span class="sxs-lookup"><span data-stu-id="9bef8-143">For notifications with resource data, the payload looks like the following.</span></span> <span data-ttu-id="9bef8-144">此有效负载用于聊天中的属性更改。</span><span class="sxs-lookup"><span data-stu-id="9bef8-144">This payload is for a property change in a chat.</span></span>

```json
{
    "value": [{
        "subscriptionId": "352887e3-9be0-4b6f-a4e6-dec118d857db",
        "changeType": "Created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-06-03T09:50:37.719033+00:00",
        "resource": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')",
        "resourceData": {
            "id": "19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces",
            "@odata.type": "#microsoft.graph.chat",
            "@odata.id": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')"
        },
        "EncryptedContent": {
            "data": "<<--EncryptedContent-->>",
            "dataKey": "<<--EnryptedDataKeyUsedForEncryptingContent-->>",
            "encryptionCertificateId": "<<--IdOfTheCertificateUsedForEncryptingDataKey-->>",
            "encryptionCertificateThumbprint": "<<--ThumbprintOfTheCertificateUsedForEncryptingDataKey-->>"
        }
            "tenantId": "<<--TenantForWhichNotificationWasSent-->>"
        }],
    "validationTokens": ["<<--ValidationTokens-->>"]
}
```

<span data-ttu-id="9bef8-145">有关如何验证令牌和解密负载的详细信息，请参阅[设置包含资源数据的更改通知](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="9bef8-145">For details about how to validate tokens and decrypt the payload, see [Set up change notifications that include resource data](webhooks-with-resource-data.md).</span></span>

<span data-ttu-id="9bef8-146">解密的通知负载如下所示。</span><span class="sxs-lookup"><span data-stu-id="9bef8-146">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="9bef8-147">有效负载符合 [聊天](/graph/api/resources/chat?preserve-view=true) 架构。</span><span class="sxs-lookup"><span data-stu-id="9bef8-147">The payload conforms to the [chats](/graph/api/resources/chat?preserve-view=true) schema.</span></span> <span data-ttu-id="9bef8-148">该负载类似于 GET 操作返回的负载。</span><span class="sxs-lookup"><span data-stu-id="9bef8-148">The payload is similar to that returned by GET operations.</span></span>

```json
{
  "id": "19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces",
  "topic": null,
  "createdDateTime": "2021-06-03T14:25:04+05:30",
  "lastUpdatedDateTime": "2021-06-03T14:25:04.387Z",
  "chatType": "oneOnOne",
  "members": [
    {
      "userId": "976f4b31-fd01-4e0b-9178-29cc40c14438",
      "email": null,
      "tenantId": "2432b57b-0abd-43db-aa7b-16eadd115d34",
      "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyM5NzZmNGIzMS1mZDAxLTRlMGItOTE3OC0yOWNjNDBjMTQ0Mzg=",
      "roles": [],
      "displayName": null,
      "visibleHistoryStartDateTime": "1970-01-01T00:00:00Z",
      "user": null
    },
    {
      "userId": "ee723d3d-22d0-4394-9c32-5764d68f4672",
      "email": null,
      "tenantId": "2432b57b-0abd-43db-aa7b-16eadd115d34",
      "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyNlZTcyM2QzZC0yMmQwLTQzOTQtOWMzMi01NzY0ZDY4ZjQ2NzI=",
      "roles": [],
      "displayName": null,
      "visibleHistoryStartDateTime": "1970-01-01T00:00:00Z",
      "user": null
    }
  ],
  "messages": [],
  "installedApps": [],
  "tabs": [],
  "permissionGrants": [],
  "operations": []
}
```

### <a name="notifications-without-resource-data"></a><span data-ttu-id="9bef8-149">不含资源数据的通知</span><span class="sxs-lookup"><span data-stu-id="9bef8-149">Notifications without resource data</span></span>

<span data-ttu-id="9bef8-150">以下有效负载描述在请求中发送的信息，以获取不含资源数据的通知。</span><span class="sxs-lookup"><span data-stu-id="9bef8-150">The following payload describes the information sent in the request for notifications without resource data.</span></span> <span data-ttu-id="9bef8-151">此特定有效负载表示已创建新的聊天。</span><span class="sxs-lookup"><span data-stu-id="9bef8-151">This particular payload signifies that a new chat has been created.</span></span>

```json
{
    "subscriptionId": "8d85051d-779d-45bc-be92-e433f0a5d8ac",
    "changeType": "Created",
    "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
    "clientState": "<<--SpecifiedClientState-->>",
    "subscriptionExpirationDateTime": "2021-06-03T10:26:09.8959595+00:00",
    "resource": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')",
    "resourceData": {
        "id": "19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces",
        "@odata.type": "#microsoft.graph.chat",
        "@odata.id": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')"
    }
}
```

<span data-ttu-id="9bef8-152">**resource** 和 **@odata.id** 属性可用于对 Microsoft Graph 进行调用以获取消息详细信息负载。</span><span class="sxs-lookup"><span data-stu-id="9bef8-152">The **resource** and **@odata.id** properties can be used to make calls to Microsoft Graph to get the payload for the chat details.</span></span> <span data-ttu-id="9bef8-153">GET 调用将始终返回聊天详细信息的当前状态。</span><span class="sxs-lookup"><span data-stu-id="9bef8-153">GET calls will always return the current state of the chat details.</span></span> <span data-ttu-id="9bef8-154">如果聊天详细信息在发送通知和检索聊天详细信息之间更新了，则该操作将返回更新的聊天详细信息。</span><span class="sxs-lookup"><span data-stu-id="9bef8-154">If the chat details were updated between when the notification is sent and when the chat details were retrieved, the operation will return the updated chat details.</span></span>

## <a name="see-also"></a><span data-ttu-id="9bef8-155">另请参阅</span><span class="sxs-lookup"><span data-stu-id="9bef8-155">See also</span></span>
- [<span data-ttu-id="9bef8-156">Microsoft Graph 更改通知</span><span class="sxs-lookup"><span data-stu-id="9bef8-156">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="9bef8-157">Microsoft Teams API 概述</span><span class="sxs-lookup"><span data-stu-id="9bef8-157">Microsoft Teams API overview</span></span>](teams-concept-overview.md)