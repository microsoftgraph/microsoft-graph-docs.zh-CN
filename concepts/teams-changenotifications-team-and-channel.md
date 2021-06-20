---
title: 使用 Microsoft Graph 获取团队和频道的更改通知
description: 了解如何使用 Microsoft Graph API 获取团队和频道的更改（创建、更新和删除）通知。
author: anandab
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 44f07661309da100ef65cf691ccfe30261467d52
ms.sourcegitcommit: 39a8c6eccc07ead237dac17387cd269733a86abd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53025017"
---
# <a name="get-change-notifications-for-teams-and-channels-using-microsoft-graph"></a><span data-ttu-id="09047-103">使用 Microsoft Graph 获取团队和频道的更改通知</span><span class="sxs-lookup"><span data-stu-id="09047-103">Get change notifications for teams and channels using Microsoft Graph</span></span>

<span data-ttu-id="09047-104">通过更改通知，可以订阅对团队和频道所做的更改（创建、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="09047-104">Change notifications enable you to subscribe to changes (create, update, and delete) to teams and channels.</span></span> <span data-ttu-id="09047-105">每当创建、更新或删除团队或频道时，你都可以收到通知。</span><span class="sxs-lookup"><span data-stu-id="09047-105">You can get notified whenever a team or channel is created, updated, or deleted.</span></span> <span data-ttu-id="09047-106">你还可以在通知中获取资源数据，因此避免调用 API 来获取有效负载。</span><span class="sxs-lookup"><span data-stu-id="09047-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

## <a name="subscribe-to-changes-in-any-team-at-tenant-level"></a><span data-ttu-id="09047-107">订阅租户级别上任何团队中的更改</span><span class="sxs-lookup"><span data-stu-id="09047-107">Subscribe to changes in any team at tenant level</span></span>

<span data-ttu-id="09047-108">要获取与租户中的任何团队相关的所有更改（创建、更新和删除）的更改通知，请订阅 `/teams`。</span><span class="sxs-lookup"><span data-stu-id="09047-108">To get change notifications for all changes (create, update, and delete) related to any team in a tenant, subscribe to `/teams`.</span></span> <span data-ttu-id="09047-109">此资源支持在通知中[包括资源数据](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="09047-109">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

### <a name="permissions"></a><span data-ttu-id="09047-110">权限</span><span class="sxs-lookup"><span data-stu-id="09047-110">Permissions</span></span>

|<span data-ttu-id="09047-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="09047-111">Permission type</span></span>      | <span data-ttu-id="09047-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="09047-112">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="09047-113">支持的版本</span><span class="sxs-lookup"><span data-stu-id="09047-113">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="09047-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09047-114">Delegated (work or school account)</span></span> | <span data-ttu-id="09047-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="09047-115">Not supported.</span></span> | <span data-ttu-id="09047-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="09047-116">Not supported.</span></span> |
|<span data-ttu-id="09047-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09047-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09047-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="09047-118">Not supported.</span></span>    | <span data-ttu-id="09047-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="09047-119">Not supported.</span></span> |
|<span data-ttu-id="09047-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="09047-120">Application</span></span> | <span data-ttu-id="09047-121">Team.ReadBasic.All，TeamSettings.Read.All，TeamSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09047-121">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All</span></span>   | <span data-ttu-id="09047-122">beta 版</span><span class="sxs-lookup"><span data-stu-id="09047-122">beta</span></span>|

### <a name="example"></a><span data-ttu-id="09047-123">示例</span><span class="sxs-lookup"><span data-stu-id="09047-123">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-changes-in-a-particular-team"></a><span data-ttu-id="09047-124">订阅特定团队中的更改</span><span class="sxs-lookup"><span data-stu-id="09047-124">Subscribe to changes in a particular team</span></span>


<span data-ttu-id="09047-125">要获取与租户中特定团队相关的所有更改的更改通知，请订阅 `/teams/{team-id}`。</span><span class="sxs-lookup"><span data-stu-id="09047-125">To get change notifications for all changes related to a particular team in a tenant, subscribe to `/teams/{team-id}`.</span></span> <span data-ttu-id="09047-126">此资源支持在通知中[包括资源数据](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="09047-126">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

### <a name="permissions"></a><span data-ttu-id="09047-127">权限</span><span class="sxs-lookup"><span data-stu-id="09047-127">Permissions</span></span>

|<span data-ttu-id="09047-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="09047-128">Permission type</span></span>      | <span data-ttu-id="09047-129">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="09047-129">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="09047-130">支持的版本</span><span class="sxs-lookup"><span data-stu-id="09047-130">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="09047-131">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09047-131">Delegated (work or school account)</span></span> | <span data-ttu-id="09047-132">Team.ReadBasic.All，TeamSettings.Read.All，TeamSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09047-132">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All</span></span> | <span data-ttu-id="09047-133">beta 版</span><span class="sxs-lookup"><span data-stu-id="09047-133">beta</span></span> |
|<span data-ttu-id="09047-134">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09047-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09047-135">不支持。</span><span class="sxs-lookup"><span data-stu-id="09047-135">Not supported.</span></span>    | <span data-ttu-id="09047-136">不支持。</span><span class="sxs-lookup"><span data-stu-id="09047-136">Not supported.</span></span> |
|<span data-ttu-id="09047-137">应用程序</span><span class="sxs-lookup"><span data-stu-id="09047-137">Application</span></span> | <span data-ttu-id="09047-138">TeamSettings.Read.Group *、TeamSettings.ReadWrite.Group*、Team.ReadBasic.All、TeamSettings.Read.All、TeamSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09047-138">TeamSettings.Read.Group *, TeamSettings.ReadWrite.Group*, Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All</span></span>    | <span data-ttu-id="09047-139">beta 版</span><span class="sxs-lookup"><span data-stu-id="09047-139">beta</span></span> |

><span data-ttu-id="09047-140">**注意：** 带有 \* 标记的权限作为 [ 资源特定的许可](/microsoftteams/platform/graph-api/rsc/resource-specific-consent) 的一部分受到支持。</span><span class="sxs-lookup"><span data-stu-id="09047-140">**Note:** Permissions marked with \* are supported as part of [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span></span>

### <a name="example"></a><span data-ttu-id="09047-141">示例</span><span class="sxs-lookup"><span data-stu-id="09047-141">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{team-id}",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```


## <a name="subscribe-to-changes-in-any-channel-at-tenant-level"></a><span data-ttu-id="09047-142">订阅租户级别上任何频道中的更改</span><span class="sxs-lookup"><span data-stu-id="09047-142">Subscribe to changes in any channel at tenant level</span></span>

<span data-ttu-id="09047-143">要获取与租户中任何频道相关的所有更改（创建、更新和删除）的更改通知，请订阅 `/teams/getAllChannels`。</span><span class="sxs-lookup"><span data-stu-id="09047-143">To get change notifications for all changes (create, update, and delete) related to any channel in a tenant, subscribe to `/teams/getAllChannels`.</span></span> <span data-ttu-id="09047-144">此资源支持在通知中 [包括资源数据](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="09047-144">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

><span data-ttu-id="09047-145">**注意：** 不支持专用频道。</span><span class="sxs-lookup"><span data-stu-id="09047-145">**Note:** Private channels aren't supported.</span></span>

### <a name="permissions"></a><span data-ttu-id="09047-146">权限</span><span class="sxs-lookup"><span data-stu-id="09047-146">Permissions</span></span>

|<span data-ttu-id="09047-147">权限类型</span><span class="sxs-lookup"><span data-stu-id="09047-147">Permission type</span></span>      | <span data-ttu-id="09047-148">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="09047-148">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="09047-149">支持的版本</span><span class="sxs-lookup"><span data-stu-id="09047-149">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="09047-150">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09047-150">Delegated (work or school account)</span></span> | <span data-ttu-id="09047-151">不支持。</span><span class="sxs-lookup"><span data-stu-id="09047-151">Not supported.</span></span> | <span data-ttu-id="09047-152">不支持。</span><span class="sxs-lookup"><span data-stu-id="09047-152">Not supported.</span></span> |
|<span data-ttu-id="09047-153">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09047-153">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09047-154">不支持。</span><span class="sxs-lookup"><span data-stu-id="09047-154">Not supported.</span></span>    | <span data-ttu-id="09047-155">不支持。</span><span class="sxs-lookup"><span data-stu-id="09047-155">Not supported.</span></span> |
|<span data-ttu-id="09047-156">应用程序</span><span class="sxs-lookup"><span data-stu-id="09047-156">Application</span></span> | <span data-ttu-id="09047-157">Channel.ReadBasic.All、ChannelSettings.Read.All、ChannelSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09047-157">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All</span></span> | <span data-ttu-id="09047-158">beta 版</span><span class="sxs-lookup"><span data-stu-id="09047-158">beta</span></span> |

### <a name="example"></a><span data-ttu-id="09047-159">示例</span><span class="sxs-lookup"><span data-stu-id="09047-159">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/getAllChannels",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-changes-in-any-channel-of-a-particular-team"></a><span data-ttu-id="09047-160">订阅特定团队的任何频道中的更改</span><span class="sxs-lookup"><span data-stu-id="09047-160">Subscribe to changes in any channel of a particular team</span></span>


<span data-ttu-id="09047-161">要获取与特定团队中任何频道相关的所有更改的更改通知，请订阅 `/teams/{team-id}/channels`。</span><span class="sxs-lookup"><span data-stu-id="09047-161">To get change notifications for all changes related to any channel in a particular team, subscribe to `/teams/{team-id}/channels`.</span></span> <span data-ttu-id="09047-162">此资源支持在通知中[包括资源数据](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="09047-162">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

### <a name="permissions"></a><span data-ttu-id="09047-163">权限</span><span class="sxs-lookup"><span data-stu-id="09047-163">Permissions</span></span>

|<span data-ttu-id="09047-164">权限类型</span><span class="sxs-lookup"><span data-stu-id="09047-164">Permission type</span></span>      | <span data-ttu-id="09047-165">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="09047-165">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="09047-166">支持的版本</span><span class="sxs-lookup"><span data-stu-id="09047-166">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="09047-167">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09047-167">Delegated (work or school account)</span></span> | <span data-ttu-id="09047-168">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09047-168">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All</span></span> | <span data-ttu-id="09047-169">beta 版</span><span class="sxs-lookup"><span data-stu-id="09047-169">beta</span></span> |
|<span data-ttu-id="09047-170">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09047-170">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09047-171">不支持。</span><span class="sxs-lookup"><span data-stu-id="09047-171">Not supported.</span></span>    | <span data-ttu-id="09047-172">不支持。</span><span class="sxs-lookup"><span data-stu-id="09047-172">Not supported.</span></span> |
|<span data-ttu-id="09047-173">应用程序</span><span class="sxs-lookup"><span data-stu-id="09047-173">Application</span></span> | <span data-ttu-id="09047-174">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09047-174">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All</span></span>   | <span data-ttu-id="09047-175">beta 版</span><span class="sxs-lookup"><span data-stu-id="09047-175">beta</span></span> |

><span data-ttu-id="09047-176">**注意：** 带有 \* 标记的权限作为 [ 资源特定的许可](/microsoftteams/platform/graph-api/rsc/resource-specific-consent) 的一部分受到支持。</span><span class="sxs-lookup"><span data-stu-id="09047-176">**Note:** Permissions marked with \* are supported as part of [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span></span>

### <a name="example"></a><span data-ttu-id="09047-177">示例</span><span class="sxs-lookup"><span data-stu-id="09047-177">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{team-id}/channels",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```


### <a name="notifications-with-resource-data"></a><span data-ttu-id="09047-178">包含资源数据的通知</span><span class="sxs-lookup"><span data-stu-id="09047-178">Notifications with resource data</span></span>

<span data-ttu-id="09047-179">对于包含资源数据的通知，负载如下所示。</span><span class="sxs-lookup"><span data-stu-id="09047-179">For notifications with resource data, the payload looks like the following.</span></span> <span data-ttu-id="09047-180">此有效负载用于团队中的属性更改。</span><span class="sxs-lookup"><span data-stu-id="09047-180">This payload is for a property change in a team.</span></span>

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "teams('fb82c19a-0f6d-41ed-90f0-cbb29a476ede')",
        "resourceData": {
            "id": "1612289765949",
            "@odata.type": "#Microsoft.Graph.Team",
            "@odata.id": "teams('fb82c19a-0f6d-41ed-90f0-cbb29a476ede')"
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



<span data-ttu-id="09047-181">已解密的通知有效负载如下所示。</span><span class="sxs-lookup"><span data-stu-id="09047-181">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="09047-182">有效负载符合 [团队](/graph/api/resources/team?preserve-view=true) 架构。</span><span class="sxs-lookup"><span data-stu-id="09047-182">The payload conforms to the [teams](/graph/api/resources/team?preserve-view=true) schema.</span></span> <span data-ttu-id="09047-183">该有效负载类似于 GET 操作返回的负载。</span><span class="sxs-lookup"><span data-stu-id="09047-183">The payload is similar to that returned by GET operations.</span></span>

><span data-ttu-id="09047-184">**注意：** [discoverySettings](/graph/api/resources/teamdiscoverysettings?preserve-view=true) 和 [classSettings](/graph/api/resources/teamclasssettings?preserve-view=true) 不会在有效负载数据中公开。</span><span class="sxs-lookup"><span data-stu-id="09047-184">**Note:** [discoverySettings](/graph/api/resources/teamdiscoverysettings?preserve-view=true) and [classSettings](/graph/api/resources/teamclasssettings?preserve-view=true) aren't exposed in payload data.</span></span>

```json
{
  "id": "4c533ad3-e1dd-4277-a672-92ab64ed225c",
  "createdDateTime": "2021-03-18T10:31:14.597Z",
  "displayName": "Sample name",
  "description": "Sample description",
  "internalId": "19:2077546f765a42c1ba71236f4df70aa2@thread.tacv2",
  "specialization": "none",
  "visibility": "public",
  "webUrl": "https://teams.microsoft.com/l/team/19:2077546f724a42c1ba71236f4df79aa2%40thread.tacv2/conversations?groupId=4c533ad3-e1dd-4277-a672-92ab64ed225c&tenantId=0f2e8f59-862a-483b-9ca8-82a10665e17d",
  "isArchived": false,
  "isMembershipLimitedToOwners": false,
  "memberSettings": {
    "allowCreateUpdateChannels": true,
    "allowCreatePrivateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true
  },
  "guestSettings": {
    "allowCreateUpdateChannels": false,
    "allowDeleteChannels": false
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true,
    "allowOwnerDeleteMessages": true,
    "allowTeamMentions": true,
    "allowChannelMentions": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "moderate",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  }
}
```


<span data-ttu-id="09047-185">对于包含资源数据的通知，有效负载如下所示。</span><span class="sxs-lookup"><span data-stu-id="09047-185">For notifications with resource data, the payload looks like the following.</span></span> <span data-ttu-id="09047-186">此有效负载用于频道中的属性更改。</span><span class="sxs-lookup"><span data-stu-id="09047-186">This payload is for a property change in a channel.</span></span>

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "teams('fb82c19a-0f6d-41ed-90f0-cbb29a476ede')/channels('19:01f39f5ac52f45fb9a7ce01cedd57b1f@thread.tacv2')",
        "resourceData": {
            "id": "19:01f39f5ac52f45fb9a7ce01cedd57b1f@thread.tacv2",
            "@odata.type": "#Microsoft.Graph.Channel",
            "@odata.id": "teams('fb82c19a-0f6d-41ed-90f0-cbb29a476ede')/channels('19:01f39f5ac52f45fb9a7ce01cedd57b1f@thread.tacv2')"
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
  

<span data-ttu-id="09047-187">已解密的通知有效负载如下所示。</span><span class="sxs-lookup"><span data-stu-id="09047-187">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="09047-188">有效负载符合 [频道](/graph/api/resources/channel?preserve-view=true) 架构。</span><span class="sxs-lookup"><span data-stu-id="09047-188">The payload conforms to the [channel](/graph/api/resources/channel?preserve-view=true) schema.</span></span> <span data-ttu-id="09047-189">该负载类似于 GET 操作返回的负载。</span><span class="sxs-lookup"><span data-stu-id="09047-189">The payload is similar to that returned by GET operations.</span></span>

```json
{
  "id": "19:a3f841d969cd4ae0a7cbe847fc10b371@thread.tacv2",
  "createdDateTime": "2020-02-14T01:10:03.592Z",
  "displayName": "General",
  "description": "Sample Channel description",
  "isFavoriteByDefault": true,
  "email": "",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3Aa3f841d969cd4ae0a7cbe847fc10b371%40thread.tacv2/General?groupId=7ed9bdab-9c7d-4c10-a25d-3f4ff0e34577&tenantId=0f2d8f49-862a-493b-9ca8-82a10637e17d",
  "membershipType": "standard",
  "moderationSettings": null
}
```


### <a name="notifications-without-resource-data"></a><span data-ttu-id="09047-190">不含资源数据的通知</span><span class="sxs-lookup"><span data-stu-id="09047-190">Notifications without resource data</span></span>

<span data-ttu-id="09047-191">不含资源数据的通知为你提供了足够的信息来进行 GET 调用以获取消息内容。</span><span class="sxs-lookup"><span data-stu-id="09047-191">Notifications without resource data give you enough information to make GET calls to get the message content.</span></span> <span data-ttu-id="09047-192">订阅不含资源数据的通知不需要加密证书（因为不会发送实际资源数据）。</span><span class="sxs-lookup"><span data-stu-id="09047-192">Subscriptions for notifications without resource data don't require an encryption certificate (because actual resource data is not sent over).</span></span>

<span data-ttu-id="09047-193">对于不包含资源数据的通知，有效负载如下所示。</span><span class="sxs-lookup"><span data-stu-id="09047-193">For notifications without resource data, the payload looks like the following.</span></span> <span data-ttu-id="09047-194">此有效负载用于团队中的属性更改。</span><span class="sxs-lookup"><span data-stu-id="09047-194">This payload is for a property change in a team.</span></span>

```json
{
  "subscriptionId": "9f9d1ed0-c9cc-42e7-8d80-a7fc4b0cda3c",
  "changeType": "created",
  "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
  "clientState": "<<--SpecifiedClientState-->>",
  "subscriptionExpirationDateTime": "2021-02-02T11:26:41.0537895-08:00",
  "resource": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')",
  "resourceData": {
    "id": "1612293113399",
    "@odata.type": "#Microsoft.Graph.Teams",
    "@odata.id": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')"
  }
}
```

<span data-ttu-id="09047-195">**resource** 和 **@odata.id** 属性可用于对 Microsoft Graph 进行调用以获取消息负载。</span><span class="sxs-lookup"><span data-stu-id="09047-195">The **resource** and **@odata.id** properties can be used to make calls to Microsoft Graph to get the payload for the message.</span></span> <span data-ttu-id="09047-196">GET 调用将始终返回消息的当前状态。</span><span class="sxs-lookup"><span data-stu-id="09047-196">GET calls will always return the current state of the message.</span></span> <span data-ttu-id="09047-197">如果在发送通知和检索消息之间更改了消息，则该操作将返回更新的消息。</span><span class="sxs-lookup"><span data-stu-id="09047-197">If the message is changed between when the notification is sent and when the message is retrieved, the operation will return the updated message.</span></span>


><span data-ttu-id="09047-198">**注意：** 有效负载中不返回频道电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="09047-198">**Note:** Channel email address isn't returned in the payload.</span></span>

<span data-ttu-id="09047-199">对于不包含资源数据的通知，有效负载如下所示。</span><span class="sxs-lookup"><span data-stu-id="09047-199">For notifications without resource data, the payload looks like the following.</span></span> <span data-ttu-id="09047-200">此有效负载用于团队中的属性更改。</span><span class="sxs-lookup"><span data-stu-id="09047-200">This payload is for a property change in a team.</span></span>

```json
{
  "id": "19:a3f841d969cd4ae0a7cbe847fc10b371@thread.tacv2",
  "createdDateTime": "2020-02-14T01:10:03.592Z",
  "displayName": "General",
  "description": "Sample Channel description",
  "isFavoriteByDefault": true,
  "email": "",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3Aa3f841d969cd4ae0a7cbe847fc10b371%40thread.tacv2/General?groupId=7ed9bdab-9c7d-4c10-a25d-3f4ff0e34577&tenantId=0f2d8f49-862a-493b-9ca8-82a10637e17d",
  "membershipType": "standard",
  "moderationSettings": null
}
```


## <a name="see-also"></a><span data-ttu-id="09047-201">另请参阅</span><span class="sxs-lookup"><span data-stu-id="09047-201">See also</span></span>
- [<span data-ttu-id="09047-202">Microsoft Graph 更改通知</span><span class="sxs-lookup"><span data-stu-id="09047-202">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="09047-203">Microsoft Teams API 概述</span><span class="sxs-lookup"><span data-stu-id="09047-203">Microsoft Teams API overview</span></span>](teams-concept-overview.md)
