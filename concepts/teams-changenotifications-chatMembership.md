---
title: 使用 Microsoft Graph 获取聊天成员资格的更改通知
description: 了解如何使用 Microsoft Graph API 获取聊天成员身份更改的通知。
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: aa8fa5ddea9c8e0df8eb8bf81558840392bdd306
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/10/2021
ms.locfileid: "53367016"
---
# <a name="get-change-notifications-for-chat-membership-using-microsoft-graph"></a><span data-ttu-id="4d9a7-103">使用 Microsoft Graph 获取聊天成员资格的更改通知</span><span class="sxs-lookup"><span data-stu-id="4d9a7-103">Get change notifications for chat membership using Microsoft Graph</span></span>

<span data-ttu-id="4d9a7-104">通过更改通知，你可以订阅聊天成员资格的更改（创建、更新、删除）。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-104">Change notifications enable you to subscribe to changes (create and delete) in chats membership.</span></span> <span data-ttu-id="4d9a7-105">每当在聊天中添加或删除成员时，你都可以收到通知。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-105">You can get notified whenever a member is added or removed from a chat.</span></span> <span data-ttu-id="4d9a7-106">你还可以在通知中获取资源数据，因此避免调用 API 来获取有效负载。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

## <a name="subscribe-to-changes-in-membership-of-any-chat-at-tenant-level"></a><span data-ttu-id="4d9a7-107">在租户级别订阅任何聊天的成员身份更改</span><span class="sxs-lookup"><span data-stu-id="4d9a7-107">Subscribe to changes in membership of any chat at tenant level</span></span>

<span data-ttu-id="4d9a7-108">若要获取租户中任何聊天中成员身份更改的更改通知，请订阅 `/chats/getAllMembers`。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-108">To get change notifications for membership changes in any chat across the tenant, subscribe to `/chats/getAllMembers`.</span></span> <span data-ttu-id="4d9a7-109">此资源支持在通知中[包括资源数据](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-109">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

### <a name="permissions"></a><span data-ttu-id="4d9a7-110">权限</span><span class="sxs-lookup"><span data-stu-id="4d9a7-110">Permissions</span></span>

|<span data-ttu-id="4d9a7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d9a7-111">Permission type</span></span>      | <span data-ttu-id="4d9a7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4d9a7-112">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="4d9a7-113">支持的版本</span><span class="sxs-lookup"><span data-stu-id="4d9a7-113">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="4d9a7-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d9a7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4d9a7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-115">Not supported.</span></span> | <span data-ttu-id="4d9a7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-116">Not supported.</span></span> |
|<span data-ttu-id="4d9a7-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4d9a7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d9a7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-118">Not supported.</span></span>    | <span data-ttu-id="4d9a7-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-119">Not supported.</span></span> |
|<span data-ttu-id="4d9a7-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="4d9a7-120">Application</span></span> | <span data-ttu-id="4d9a7-121">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="4d9a7-121">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span>  | <span data-ttu-id="4d9a7-122">beta 版</span><span class="sxs-lookup"><span data-stu-id="4d9a7-122">beta</span></span>|

### <a name="example"></a><span data-ttu-id="4d9a7-123">示例</span><span class="sxs-lookup"><span data-stu-id="4d9a7-123">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/getAllMembers",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-changes-in-membership-of-a-particular-chat"></a><span data-ttu-id="4d9a7-124">订阅特定聊天的成员资格更改</span><span class="sxs-lookup"><span data-stu-id="4d9a7-124">Subscribe to changes in membership of a particular chat</span></span>

<span data-ttu-id="4d9a7-125">若要获取特定聊天中成员资格更改的更改通知，请订阅 `/chats/{id}/members`。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-125">To get change notifications for membership changes in a particular chat, subscribe to `/chats/{id}/members`.</span></span> <span data-ttu-id="4d9a7-126">此资源支持在通知中[包括资源数据](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-126">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

### <a name="permissions"></a><span data-ttu-id="4d9a7-127">权限</span><span class="sxs-lookup"><span data-stu-id="4d9a7-127">Permissions</span></span>

|<span data-ttu-id="4d9a7-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d9a7-128">Permission type</span></span>      | <span data-ttu-id="4d9a7-129">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4d9a7-129">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="4d9a7-130">支持的版本</span><span class="sxs-lookup"><span data-stu-id="4d9a7-130">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="4d9a7-131">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d9a7-131">Delegated (work or school account)</span></span> | <span data-ttu-id="4d9a7-132">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d9a7-132">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="4d9a7-133">beta 版</span><span class="sxs-lookup"><span data-stu-id="4d9a7-133">beta</span></span> |
|<span data-ttu-id="4d9a7-134">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4d9a7-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d9a7-135">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-135">Not supported.</span></span>    | <span data-ttu-id="4d9a7-136">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-136">Not supported.</span></span> |
|<span data-ttu-id="4d9a7-137">应用程序</span><span class="sxs-lookup"><span data-stu-id="4d9a7-137">Application</span></span> | <span data-ttu-id="4d9a7-138">ChatMember.Read.Chat *、Chat.Manage.Chat*、ChatMember.Read.All、ChatMember.ReadWrite.All、Chat.ReadBasic.All、Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d9a7-138">ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span>  | <span data-ttu-id="4d9a7-139">beta</span><span class="sxs-lookup"><span data-stu-id="4d9a7-139">beta</span></span> |

> <span data-ttu-id="4d9a7-140">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-140">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="example"></a><span data-ttu-id="4d9a7-141">示例</span><span class="sxs-lookup"><span data-stu-id="4d9a7-141">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}/members",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```



### <a name="notifications-with-resource-data"></a><span data-ttu-id="4d9a7-142">包含资源数据的通知</span><span class="sxs-lookup"><span data-stu-id="4d9a7-142">Notifications with resource data</span></span>

<span data-ttu-id="4d9a7-143">对于包含资源数据的通知，负载如下所示。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-143">For notifications with resource data, the payload looks like the following.</span></span> <span data-ttu-id="4d9a7-144">此有效负载用于聊天中的成员资格更改。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-144">This payload is for a membership change in a chat.</span></span>

```json
{
    "value": [{
        "subscriptionId": "c0125ef2-7a87-4e94-aa71-b995510f369b",
        "changeType": "Created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-06-03T11:04:58.5537601+00:00",
        "resource": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')/members('MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyMyZmM2MDY2My0xOWEyLTRhYTQtODUyYy1mN2JhNGU5MGFkYTI=')",
        "resourceData": {
            "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyMyZmM2MDY2My0xOWEyLTRhYTQtODUyYy1mN2JhNGU5MGFkYTI=",
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "@odata.id": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')/members('MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyMyZmM2MDY2My0xOWEyLTRhYTQtODUyYy1mN2JhNGU5MGFkYTI=')"
        },
        "EncryptedContent": {
            "data": "<<--EncryptedContent-->>",
            "dataKey": "<<--EnryptedDataKeyUsedForEncryptingContent-->>",
            "encryptionCertificateId": "<<--IdOfTheCertificateUsedForEncryptingDataKey-->>",
            "encryptionCertificateThumbprint": "<<--ThumbprintOfTheCertificateUsedForEncryptingDataKey-->>"
        },
        "tenantId": "<<--TenantForWhichNotificationWasSent-->>"
    }],
    "validationTokens": ["<<--ValidationTokens-->>"]
}
```

<span data-ttu-id="4d9a7-145">有关如何验证令牌和解密负载的详细信息，请参阅[设置包含资源数据的更改通知](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-145">For details about how to validate tokens and decrypt the payload, see [Set up change notifications that include resource data](webhooks-with-resource-data.md).</span></span>

<span data-ttu-id="4d9a7-146">解密的通知负载如下所示。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-146">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="4d9a7-147">有效负载符合 [aaduserconversationmember](/graph/api/resources/aaduserconversationmember?preserve-view=true) 架构。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-147">The payload conforms to the [aaduserconversationmember](/graph/api/resources/aaduserconversationmember?preserve-view=true) schema.</span></span> <span data-ttu-id="4d9a7-148">该负载类似于 GET 操作返回的负载。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-148">The payload is similar to that returned by GET operations.</span></span>

```json
{
    "userId": "2fc60663-19a2-4aa4-852c-f7ba4e90ada2",
    "email": null,
    "tenantId": "2432b57b-0abd-43db-aa7b-16eadd115d34",
    "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyMyZmM2MDY2My0xOWEyLTRhYTQtODUyYy1mN2JhNGU5MGFkYTI=",
    "roles": [
    "Owner"
    ],
    "displayName": null,
    "visibleHistoryStartDateTime": "1970-01-01T00:00:00Z",
    "user": null
}
```

### <a name="notifications-without-resource-data"></a><span data-ttu-id="4d9a7-149">不含资源数据的通知</span><span class="sxs-lookup"><span data-stu-id="4d9a7-149">Notifications without resource data</span></span>

<span data-ttu-id="4d9a7-150">以下有效负载描述在请求中发送的信息，以获取不含资源数据的通知。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-150">The following payload describes the information sent in the request for notifications without resource data.</span></span> <span data-ttu-id="4d9a7-151">此特定有效负载表示已将用户添加到聊天中。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-151">This particular payload signifies that a user has been added to a chat.</span></span>

```json
{
    "subscriptionId": "cae901f1-ad1d-41b1-95b7-37029ed327bf",
    "changeType": "Created",
    "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
    "clientState": "<<--SpecifiedClientState-->>",
    "subscriptionExpirationDateTime": "2021-06-03T10:58:54.7656077+00:00",
    "resource": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')/members('MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyMyZmM2MDY2My0xOWEyLTRhYTQtODUyYy1mN2JhNGU5MGFkYTI=')",
    "resourceData": {
        "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyMyZmM2MDY2My0xOWEyLTRhYTQtODUyYy1mN2JhNGU5MGFkYTI=",
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "@odata.id": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')/members('MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyMyZmM2MDY2My0xOWEyLTRhYTQtODUyYy1mN2JhNGU5MGFkYTI=')"
    }
}
```

<span data-ttu-id="4d9a7-152">**resource** 和 **@odata.id** 属性可用于对 Microsoft Graph 进行调用以获取聊天成员详细信息负载。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-152">The **resource** and **@odata.id** properties can be used to make calls to Microsoft Graph to get the payload for the chat member details.</span></span> <span data-ttu-id="4d9a7-153">GET 调用将始终返回聊天成员详细信息的当前状态。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-153">GET calls will always return the current state of the chat member details.</span></span> <span data-ttu-id="4d9a7-154">如果聊天成员详细信息在发送通知和检索它们的详细信息之间发生了更改，则该操作将返回更新的聊天成员详细信息。</span><span class="sxs-lookup"><span data-stu-id="4d9a7-154">If the chat member details has changed between when the notification is sent and when the chat member details were retrieved, the operation will return the updated chat member details.</span></span>

## <a name="see-also"></a><span data-ttu-id="4d9a7-155">另请参阅</span><span class="sxs-lookup"><span data-stu-id="4d9a7-155">See also</span></span>
- [<span data-ttu-id="4d9a7-156">Microsoft Graph 更改通知</span><span class="sxs-lookup"><span data-stu-id="4d9a7-156">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="4d9a7-157">Microsoft Teams API 概述</span><span class="sxs-lookup"><span data-stu-id="4d9a7-157">Microsoft Teams API overview</span></span>](teams-concept-overview.md)