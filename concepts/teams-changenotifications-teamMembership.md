---
title: 使用 Microsoft Graph 获取 Teams 成员资格任何更改的更改通知
description: 使用 Microsoft Graph 获取 Teams 成员资格任何更改（创建、更新和删除）的更改通知
author: anandab
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 8f9d0a654f3105c7d365bc92f774ab66be34f35d
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971460"
---
# <a name="get-change-notifications-for-changes-in-teams-membership-using-microsoft-graph"></a><span data-ttu-id="0536d-103">使用 Microsoft Graph 获取 Teams 成员资格更改的更改通知</span><span class="sxs-lookup"><span data-stu-id="0536d-103">Get change notifications for changes in Teams membership using Microsoft Graph</span></span>

<span data-ttu-id="0536d-104">通过更改通知，你可以订阅 Teams 成员资格更改（创建、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="0536d-104">Change notifications enable you to subscribe to changes (create, update, and delete) in teams membership.</span></span> <span data-ttu-id="0536d-105">每当在团队中添加、删除或更新成员时，你都可以收到通知。</span><span class="sxs-lookup"><span data-stu-id="0536d-105">You can get notified whenever member is added, removed or updated in a team.</span></span> <span data-ttu-id="0536d-106">你还可以在通知中获取资源数据，因此避免调用 API 来获取有效负载。</span><span class="sxs-lookup"><span data-stu-id="0536d-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

## <a name="subscribe-to-changes-in-membership-of-a-particular-team"></a><span data-ttu-id="0536d-107">订阅特定团队的成员资格更改</span><span class="sxs-lookup"><span data-stu-id="0536d-107">Subscribe to changes in membership of a particular team</span></span>

<span data-ttu-id="0536d-108">若要获取特定团队中成员资格更改的更改通知，请订阅 `/teams/{id}/members`。</span><span class="sxs-lookup"><span data-stu-id="0536d-108">To get change notifications for membership changes in a particular team, subscribe to `/teams/{id}/members`.</span></span> <span data-ttu-id="0536d-109">此资源支持在通知中[包括资源数据](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="0536d-109">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="0536d-110">权限</span><span class="sxs-lookup"><span data-stu-id="0536d-110">Permissions</span></span>

|<span data-ttu-id="0536d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0536d-111">Permission type</span></span>      | <span data-ttu-id="0536d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0536d-112">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="0536d-113">支持的版本</span><span class="sxs-lookup"><span data-stu-id="0536d-113">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="0536d-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0536d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0536d-115">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="0536d-115">TeamMember.Read.All</span></span> | <span data-ttu-id="0536d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0536d-116">Not supported.</span></span> |
|<span data-ttu-id="0536d-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0536d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0536d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0536d-118">Not supported.</span></span>    | <span data-ttu-id="0536d-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="0536d-119">Not supported.</span></span> |
|<span data-ttu-id="0536d-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="0536d-120">Application</span></span> | <span data-ttu-id="0536d-121">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="0536d-121">TeamMember.Read.All</span></span>   | <span data-ttu-id="0536d-122">beta 版</span><span class="sxs-lookup"><span data-stu-id="0536d-122">beta</span></span> |

#### <a name="example"></a><span data-ttu-id="0536d-123">示例</span><span class="sxs-lookup"><span data-stu-id="0536d-123">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/members",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```



### <a name="notifications-with-resource-data"></a><span data-ttu-id="0536d-124">包含资源数据的通知</span><span class="sxs-lookup"><span data-stu-id="0536d-124">Notifications with resource data</span></span>

<span data-ttu-id="0536d-125">对于包含资源数据的通知，负载如下所示。</span><span class="sxs-lookup"><span data-stu-id="0536d-125">For notifications with resource data, the payload looks like the following.</span></span> <span data-ttu-id="0536d-126">此有效负载用于团队中的成员资格更改。</span><span class="sxs-lookup"><span data-stu-id="0536d-126">This payload is for a membership change in a team.</span></span>

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members('ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')",
        "resourceData": {
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
            "@odata.type": "#Microsoft.Graph.aadUserConversationMember",
            "@odata.id": "teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members('ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')"
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

<span data-ttu-id="0536d-127">有关如何验证令牌和解密负载的详细信息，请参阅[设置包含资源数据的更改通知](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="0536d-127">For details about how to validate tokens and decrypt the payload, see [Set up change notifications that include resource data](webhooks-with-resource-data.md).</span></span>

<span data-ttu-id="0536d-128">解密的通知负载如下所示。</span><span class="sxs-lookup"><span data-stu-id="0536d-128">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="0536d-129">有效负载符合 [aaduserconversationmember](/graph/api/resources/aaduserconversationmember?preserve-view=true) 架构。</span><span class="sxs-lookup"><span data-stu-id="0536d-129">The payload conforms to the [aaduserconversationmember](/graph/api/resources/aaduserconversationmember?preserve-view=true) schema.</span></span> <span data-ttu-id="0536d-130">该负载类似于 GET 操作返回的负载。</span><span class="sxs-lookup"><span data-stu-id="0536d-130">The payload is similar to that returned by GET operations.</span></span>

```json
{
  "id": "/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
  "roles": [
    "owner"
  ],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```

### <a name="notifications-without-resource-data"></a><span data-ttu-id="0536d-131">不含资源数据的通知</span><span class="sxs-lookup"><span data-stu-id="0536d-131">Notifications without resource data</span></span>

<span data-ttu-id="0536d-132">不含资源数据的通知为你提供了足够的信息来进行 GET 调用以获取消息内容。</span><span class="sxs-lookup"><span data-stu-id="0536d-132">Notifications without resource data give you enough information to make GET calls to get the message content.</span></span> <span data-ttu-id="0536d-133">订阅不含资源数据的通知不需要加密证书（因为不会发送实际资源数据）。</span><span class="sxs-lookup"><span data-stu-id="0536d-133">Subscriptions for notifications without resource data don't require an encryption certificate (because actual resource data is not sent over).</span></span>

<span data-ttu-id="0536d-134">对于不包含资源数据的通知，有效负载如下所示。</span><span class="sxs-lookup"><span data-stu-id="0536d-134">For notifications without resource data, the payload looks like the following.</span></span> <span data-ttu-id="0536d-135">此有效负载用于团队中的成员资格更改。</span><span class="sxs-lookup"><span data-stu-id="0536d-135">This payload is for a membership change in a team.</span></span>

```json
{
  "subscriptionId": "9f9d1ed0-c9cc-42e7-8d80-a7fc4b0cda3c",
  "changeType": "created",
  "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
  "clientState": "<<--SpecifiedClientState-->>",
  "subscriptionExpirationDateTime": "2021-02-02T11:26:41.0537895-08:00",
  "resource": "teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members('ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')",
  "resourceData": {
    "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk",
    "@odata.type": "#Microsoft.Graph.aadUserConversationMember",
    "@odata.id": "teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members('ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')"
  }
}
```

<span data-ttu-id="0536d-136">**resource** 和 **@odata.id** 属性可用于对 Microsoft Graph 进行调用以获取消息负载。</span><span class="sxs-lookup"><span data-stu-id="0536d-136">The **resource** and **@odata.id** properties can be used to make calls to Microsoft Graph to get the payload for the message.</span></span> <span data-ttu-id="0536d-137">GET 调用将始终返回消息的当前状态。</span><span class="sxs-lookup"><span data-stu-id="0536d-137">GET calls will always return the current state of the message.</span></span> <span data-ttu-id="0536d-138">如果在发送通知和检索消息之间更改了消息，则该操作将返回更新的消息。</span><span class="sxs-lookup"><span data-stu-id="0536d-138">If the message is changed between when the notification is sent and when the message is retrieved, the operation will return the updated message.</span></span>

## <a name="see-also"></a><span data-ttu-id="0536d-139">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0536d-139">See also</span></span>
- [<span data-ttu-id="0536d-140">Microsoft Graph 更改通知</span><span class="sxs-lookup"><span data-stu-id="0536d-140">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="0536d-141">Microsoft Teams API 概述</span><span class="sxs-lookup"><span data-stu-id="0536d-141">Microsoft Teams API overview</span></span>](teams-concept-overview.md)