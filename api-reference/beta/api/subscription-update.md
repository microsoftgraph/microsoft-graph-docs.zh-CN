---
title: 更新订阅
description: 通过延长到期时间续订订阅。
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 34a03b5e5305e62837e72559719995e2b6dae5e6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013977"
---
# <a name="update-subscription"></a><span data-ttu-id="81434-103">更新订阅</span><span class="sxs-lookup"><span data-stu-id="81434-103">Update subscription</span></span>

<span data-ttu-id="81434-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81434-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81434-105">通过延长到期时间续订订阅。</span><span class="sxs-lookup"><span data-stu-id="81434-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="81434-106">订阅将在因资源类型而异的一段时间后过期。</span><span class="sxs-lookup"><span data-stu-id="81434-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="81434-107">为了避免丢失更改通知，应用应在到期日期前提前续订其订阅。</span><span class="sxs-lookup"><span data-stu-id="81434-107">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="81434-108">有关每种资源类型的最大订阅长度，请参阅 [订阅](../resources/subscription.md) 。</span><span class="sxs-lookup"><span data-stu-id="81434-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="81434-109">权限</span><span class="sxs-lookup"><span data-stu-id="81434-109">Permissions</span></span>

<span data-ttu-id="81434-110">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="81434-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="81434-111">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="81434-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="81434-112">支持的资源</span><span class="sxs-lookup"><span data-stu-id="81434-112">Supported resource</span></span> | <span data-ttu-id="81434-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="81434-113">Delegated (work or school account)</span></span> | <span data-ttu-id="81434-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="81434-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81434-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="81434-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="81434-116">callRecord</span><span class="sxs-lookup"><span data-stu-id="81434-116">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="81434-117">不支持</span><span class="sxs-lookup"><span data-stu-id="81434-117">Not supported</span></span> | <span data-ttu-id="81434-118">不支持</span><span class="sxs-lookup"><span data-stu-id="81434-118">Not supported</span></span> | <span data-ttu-id="81434-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="81434-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="81434-120">[了 chatmessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages) </span><span class="sxs-lookup"><span data-stu-id="81434-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="81434-121">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81434-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="81434-122">不支持</span><span class="sxs-lookup"><span data-stu-id="81434-122">Not supported</span></span> | <span data-ttu-id="81434-123">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="81434-123">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="81434-124">[了 chatmessage](../resources/chatmessage.md) (/teams/allmessages--组织中的所有频道邮件) </span><span class="sxs-lookup"><span data-stu-id="81434-124">[chatMessage](../resources/chatmessage.md) (/teams/allMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="81434-125">不支持</span><span class="sxs-lookup"><span data-stu-id="81434-125">Not supported</span></span> | <span data-ttu-id="81434-126">不支持</span><span class="sxs-lookup"><span data-stu-id="81434-126">Not supported</span></span> | <span data-ttu-id="81434-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="81434-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="81434-128">[了 chatmessage](../resources/chatmessage.md) (/chats/{id}/messages) </span><span class="sxs-lookup"><span data-stu-id="81434-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="81434-129">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81434-129">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="81434-130">不支持</span><span class="sxs-lookup"><span data-stu-id="81434-130">Not supported</span></span> | <span data-ttu-id="81434-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="81434-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="81434-132">[了 chatmessage](../resources/chatmessage.md) (/chats/allmessages--组织中的所有聊天邮件) </span><span class="sxs-lookup"><span data-stu-id="81434-132">[chatMessage](../resources/chatmessage.md) (/chats/allMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="81434-133">不支持</span><span class="sxs-lookup"><span data-stu-id="81434-133">Not supported</span></span> | <span data-ttu-id="81434-134">不支持</span><span class="sxs-lookup"><span data-stu-id="81434-134">Not supported</span></span> | <span data-ttu-id="81434-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="81434-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="81434-136">联系人</span><span class="sxs-lookup"><span data-stu-id="81434-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="81434-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="81434-137">Contacts.Read</span></span> | <span data-ttu-id="81434-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="81434-138">Contacts.Read</span></span> | <span data-ttu-id="81434-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="81434-139">Contacts.Read</span></span> |
|<span data-ttu-id="81434-140">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="81434-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="81434-141">不支持</span><span class="sxs-lookup"><span data-stu-id="81434-141">Not supported</span></span> | <span data-ttu-id="81434-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81434-142">Files.ReadWrite</span></span> | <span data-ttu-id="81434-143">不支持</span><span class="sxs-lookup"><span data-stu-id="81434-143">Not supported</span></span> |
|<span data-ttu-id="81434-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="81434-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="81434-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81434-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="81434-146">不支持</span><span class="sxs-lookup"><span data-stu-id="81434-146">Not supported</span></span> | <span data-ttu-id="81434-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81434-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="81434-148">事件</span><span class="sxs-lookup"><span data-stu-id="81434-148">event</span></span>](../resources/event.md) | <span data-ttu-id="81434-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="81434-149">Calendars.Read</span></span> | <span data-ttu-id="81434-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="81434-150">Calendars.Read</span></span> | <span data-ttu-id="81434-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="81434-151">Calendars.Read</span></span> |
|[<span data-ttu-id="81434-152">组</span><span class="sxs-lookup"><span data-stu-id="81434-152">group</span></span>](../resources/group.md) | <span data-ttu-id="81434-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="81434-153">Group.Read.All</span></span> | <span data-ttu-id="81434-154">不支持</span><span class="sxs-lookup"><span data-stu-id="81434-154">Not supported</span></span> | <span data-ttu-id="81434-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="81434-155">Group.Read.All</span></span> |
|[<span data-ttu-id="81434-156">组对话</span><span class="sxs-lookup"><span data-stu-id="81434-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="81434-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="81434-157">Group.Read.All</span></span> | <span data-ttu-id="81434-158">不支持</span><span class="sxs-lookup"><span data-stu-id="81434-158">Not supported</span></span> | <span data-ttu-id="81434-159">不支持</span><span class="sxs-lookup"><span data-stu-id="81434-159">Not supported</span></span> |
|[<span data-ttu-id="81434-160">列表</span><span class="sxs-lookup"><span data-stu-id="81434-160">list</span></span>](../resources/list.md) | <span data-ttu-id="81434-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81434-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="81434-162">不支持</span><span class="sxs-lookup"><span data-stu-id="81434-162">Not supported</span></span> | <span data-ttu-id="81434-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81434-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="81434-164">邮件</span><span class="sxs-lookup"><span data-stu-id="81434-164">message</span></span>](../resources/message.md) | <span data-ttu-id="81434-165">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="81434-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="81434-166">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="81434-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="81434-167">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="81434-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="81434-168">状态</span><span class="sxs-lookup"><span data-stu-id="81434-168">presence</span></span>](../resources/presence.md) | <span data-ttu-id="81434-169">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="81434-169">Presence.Read.All</span></span> | <span data-ttu-id="81434-170">不支持</span><span class="sxs-lookup"><span data-stu-id="81434-170">Not supported</span></span> | <span data-ttu-id="81434-171">不支持</span><span class="sxs-lookup"><span data-stu-id="81434-171">Not supported</span></span> |
|<span data-ttu-id="81434-172">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="81434-172">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="81434-173">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81434-173">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="81434-174">不支持</span><span class="sxs-lookup"><span data-stu-id="81434-174">Not supported</span></span> | <span data-ttu-id="81434-175">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81434-175">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="81434-176">用户</span><span class="sxs-lookup"><span data-stu-id="81434-176">user</span></span>](../resources/user.md) | <span data-ttu-id="81434-177">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="81434-177">User.Read.All</span></span> | <span data-ttu-id="81434-178">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="81434-178">User.Read.All</span></span> | <span data-ttu-id="81434-179">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="81434-179">User.Read.All</span></span> |

### <a name="chatmessage"></a><span data-ttu-id="81434-180">chatMessage</span><span class="sxs-lookup"><span data-stu-id="81434-180">chatMessage</span></span>

<span data-ttu-id="81434-181">具有委派权限的**了 chatmessage**订阅不支持资源数据 (**includeResourceData**必须 `false`) ，并且不需要[加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="81434-181">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="81434-182">具有应用程序权限的**了 chatmessage**订阅包括资源数据，并需要[加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="81434-182">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="81434-183">如果未指定 [encryptionCertificate](../resources/subscription.md) ，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="81434-183">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="81434-184">在创建 **了 chatmessage** 订阅之前，您必须请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="81434-184">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="81434-185">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="81434-185">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="81434-186">**注意：** `/teams/allMessages` ，并且 `/chats/allMessages` 当前处于预览阶段。</span><span class="sxs-lookup"><span data-stu-id="81434-186">**Note:** `/teams/allMessages` and `/chats/allMessages` are currently in preview.</span></span> <span data-ttu-id="81434-187">在预览过程中，可以在不付费的情况下使用此 API，这取决于 [Microsoft Api 使用条款](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context)。</span><span class="sxs-lookup"><span data-stu-id="81434-187">During the preview, you may use this API without fees, subject to the [Microsoft APIs Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span></span> <span data-ttu-id="81434-188">但是，使用 API 的应用程序的用户可能需要订阅特定 Microsoft 365 产品。</span><span class="sxs-lookup"><span data-stu-id="81434-188">However, users of apps that use the API might be required to have subscriptions to specific Microsoft 365 offerings.</span></span> <span data-ttu-id="81434-189">在正式发行时，Microsoft 可能会要求您或您的客户根据通过 API 访问的数据量支付额外费用。</span><span class="sxs-lookup"><span data-stu-id="81434-189">Upon general availability, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>

### <a name="driveitem"></a><span data-ttu-id="81434-190">driveItem</span><span class="sxs-lookup"><span data-stu-id="81434-190">driveItem</span></span>

<span data-ttu-id="81434-191">对 OneDrive 项目的订阅适用其他限制。</span><span class="sxs-lookup"><span data-stu-id="81434-191">Additional limitations apply for subscriptions on OneDrive  items.</span></span> <span data-ttu-id="81434-192">这些限制适用于创建以及管理 (获取、更新和删除) 订阅。</span><span class="sxs-lookup"><span data-stu-id="81434-192">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="81434-193">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="81434-193">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="81434-194">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="81434-194">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="81434-195">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="81434-195">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="81434-196">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="81434-196">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="81434-197">联系人、事件和邮件</span><span class="sxs-lookup"><span data-stu-id="81434-197">contact, event, and message</span></span>

<span data-ttu-id="81434-198">对 Outlook 项目的订阅适用其他限制。</span><span class="sxs-lookup"><span data-stu-id="81434-198">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="81434-199">这些限制适用于创建以及管理 (获取、更新和删除) 订阅。</span><span class="sxs-lookup"><span data-stu-id="81434-199">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="81434-200">委派权限仅支持订阅登录用户的邮箱中的文件夹中的项目。</span><span class="sxs-lookup"><span data-stu-id="81434-200">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="81434-201">也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="81434-201">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="81434-202">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="81434-202">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="81434-203">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="81434-203">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="81434-204">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="81434-204">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="81434-205">状态</span><span class="sxs-lookup"><span data-stu-id="81434-205">presence</span></span>

<span data-ttu-id="81434-206">**状态** 订阅需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="81434-206">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="81434-207">如果未指定 [encryptionCertificate](../resources/subscription.md) ，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="81434-207">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="81434-208">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="81434-208">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="81434-209">请求标头</span><span class="sxs-lookup"><span data-stu-id="81434-209">Request headers</span></span>

| <span data-ttu-id="81434-210">名称</span><span class="sxs-lookup"><span data-stu-id="81434-210">Name</span></span>       | <span data-ttu-id="81434-211">类型</span><span class="sxs-lookup"><span data-stu-id="81434-211">Type</span></span> | <span data-ttu-id="81434-212">说明</span><span class="sxs-lookup"><span data-stu-id="81434-212">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="81434-213">Authorization</span><span class="sxs-lookup"><span data-stu-id="81434-213">Authorization</span></span>  | <span data-ttu-id="81434-214">string</span><span class="sxs-lookup"><span data-stu-id="81434-214">string</span></span>  | <span data-ttu-id="81434-p110">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="81434-p110">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="81434-217">响应</span><span class="sxs-lookup"><span data-stu-id="81434-217">Response</span></span>

<span data-ttu-id="81434-218">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="81434-218">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="81434-219">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="81434-219">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="81434-220">示例</span><span class="sxs-lookup"><span data-stu-id="81434-220">Example</span></span>

##### <a name="request"></a><span data-ttu-id="81434-221">请求</span><span class="sxs-lookup"><span data-stu-id="81434-221">Request</span></span>

<span data-ttu-id="81434-222">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="81434-222">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="81434-223">HTTP</span><span class="sxs-lookup"><span data-stu-id="81434-223">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/beta/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```
# <a name="c"></a>[<span data-ttu-id="81434-224">C#</span><span class="sxs-lookup"><span data-stu-id="81434-224">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81434-225">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81434-225">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81434-226">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81434-226">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="81434-227">响应</span><span class="sxs-lookup"><span data-stu-id="81434-227">Response</span></span>

<span data-ttu-id="81434-228">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="81434-228">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2"
}
```

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


