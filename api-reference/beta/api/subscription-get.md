---
title: 获取订阅
description: 检索订阅的属性和关系。
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: f84d68b62e60c1eb321dafde76bd3712991b956a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013984"
---
# <a name="get-subscription"></a><span data-ttu-id="ebf6b-103">获取订阅</span><span class="sxs-lookup"><span data-stu-id="ebf6b-103">Get subscription</span></span>

<span data-ttu-id="ebf6b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebf6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebf6b-105">检索订阅的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-105">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="ebf6b-106">权限</span><span class="sxs-lookup"><span data-stu-id="ebf6b-106">Permissions</span></span>

<span data-ttu-id="ebf6b-107">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="ebf6b-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ebf6b-109">支持的资源</span><span class="sxs-lookup"><span data-stu-id="ebf6b-109">Supported resource</span></span> | <span data-ttu-id="ebf6b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ebf6b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ebf6b-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ebf6b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebf6b-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="ebf6b-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="ebf6b-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="ebf6b-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="ebf6b-114">不支持</span><span class="sxs-lookup"><span data-stu-id="ebf6b-114">Not supported</span></span> | <span data-ttu-id="ebf6b-115">不支持</span><span class="sxs-lookup"><span data-stu-id="ebf6b-115">Not supported</span></span> | <span data-ttu-id="ebf6b-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="ebf6b-116">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="ebf6b-117">[了 chatmessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages) </span><span class="sxs-lookup"><span data-stu-id="ebf6b-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="ebf6b-118">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebf6b-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="ebf6b-119">不支持</span><span class="sxs-lookup"><span data-stu-id="ebf6b-119">Not supported</span></span> | <span data-ttu-id="ebf6b-120">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="ebf6b-120">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="ebf6b-121">[了 chatmessage](../resources/chatmessage.md) (/teams/allmessages--组织中的所有频道邮件) </span><span class="sxs-lookup"><span data-stu-id="ebf6b-121">[chatMessage](../resources/chatmessage.md) (/teams/allMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="ebf6b-122">不支持</span><span class="sxs-lookup"><span data-stu-id="ebf6b-122">Not supported</span></span> | <span data-ttu-id="ebf6b-123">不支持</span><span class="sxs-lookup"><span data-stu-id="ebf6b-123">Not supported</span></span> | <span data-ttu-id="ebf6b-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="ebf6b-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="ebf6b-125">[了 chatmessage](../resources/chatmessage.md) (/chats/{id}/messages) </span><span class="sxs-lookup"><span data-stu-id="ebf6b-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="ebf6b-126">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebf6b-126">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="ebf6b-127">不支持</span><span class="sxs-lookup"><span data-stu-id="ebf6b-127">Not supported</span></span> | <span data-ttu-id="ebf6b-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="ebf6b-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="ebf6b-129">[了 chatmessage](../resources/chatmessage.md) (/chats/allmessages--组织中的所有聊天邮件) </span><span class="sxs-lookup"><span data-stu-id="ebf6b-129">[chatMessage](../resources/chatmessage.md) (/chats/allMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="ebf6b-130">不支持</span><span class="sxs-lookup"><span data-stu-id="ebf6b-130">Not supported</span></span> | <span data-ttu-id="ebf6b-131">不支持</span><span class="sxs-lookup"><span data-stu-id="ebf6b-131">Not supported</span></span> | <span data-ttu-id="ebf6b-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="ebf6b-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="ebf6b-133">联系人</span><span class="sxs-lookup"><span data-stu-id="ebf6b-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="ebf6b-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ebf6b-134">Contacts.Read</span></span> | <span data-ttu-id="ebf6b-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ebf6b-135">Contacts.Read</span></span> | <span data-ttu-id="ebf6b-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ebf6b-136">Contacts.Read</span></span> |
|<span data-ttu-id="ebf6b-137">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="ebf6b-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="ebf6b-138">不支持</span><span class="sxs-lookup"><span data-stu-id="ebf6b-138">Not supported</span></span> | <span data-ttu-id="ebf6b-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebf6b-139">Files.ReadWrite</span></span> | <span data-ttu-id="ebf6b-140">不支持</span><span class="sxs-lookup"><span data-stu-id="ebf6b-140">Not supported</span></span> |
|<span data-ttu-id="ebf6b-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="ebf6b-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="ebf6b-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebf6b-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="ebf6b-143">不支持</span><span class="sxs-lookup"><span data-stu-id="ebf6b-143">Not supported</span></span> | <span data-ttu-id="ebf6b-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebf6b-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="ebf6b-145">事件</span><span class="sxs-lookup"><span data-stu-id="ebf6b-145">event</span></span>](../resources/event.md) | <span data-ttu-id="ebf6b-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ebf6b-146">Calendars.Read</span></span> | <span data-ttu-id="ebf6b-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ebf6b-147">Calendars.Read</span></span> | <span data-ttu-id="ebf6b-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ebf6b-148">Calendars.Read</span></span> |
|[<span data-ttu-id="ebf6b-149">组</span><span class="sxs-lookup"><span data-stu-id="ebf6b-149">group</span></span>](../resources/group.md) | <span data-ttu-id="ebf6b-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ebf6b-150">Group.Read.All</span></span> | <span data-ttu-id="ebf6b-151">不支持</span><span class="sxs-lookup"><span data-stu-id="ebf6b-151">Not supported</span></span> | <span data-ttu-id="ebf6b-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ebf6b-152">Group.Read.All</span></span> |
|[<span data-ttu-id="ebf6b-153">组对话</span><span class="sxs-lookup"><span data-stu-id="ebf6b-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="ebf6b-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ebf6b-154">Group.Read.All</span></span> | <span data-ttu-id="ebf6b-155">不支持</span><span class="sxs-lookup"><span data-stu-id="ebf6b-155">Not supported</span></span> | <span data-ttu-id="ebf6b-156">不支持</span><span class="sxs-lookup"><span data-stu-id="ebf6b-156">Not supported</span></span> |
|[<span data-ttu-id="ebf6b-157">列表</span><span class="sxs-lookup"><span data-stu-id="ebf6b-157">list</span></span>](../resources/list.md) | <span data-ttu-id="ebf6b-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebf6b-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="ebf6b-159">不支持</span><span class="sxs-lookup"><span data-stu-id="ebf6b-159">Not supported</span></span> | <span data-ttu-id="ebf6b-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebf6b-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="ebf6b-161">邮件</span><span class="sxs-lookup"><span data-stu-id="ebf6b-161">message</span></span>](../resources/message.md) | <span data-ttu-id="ebf6b-162">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ebf6b-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="ebf6b-163">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ebf6b-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="ebf6b-164">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ebf6b-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="ebf6b-165">状态</span><span class="sxs-lookup"><span data-stu-id="ebf6b-165">presence</span></span>](../resources/presence.md) | <span data-ttu-id="ebf6b-166">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="ebf6b-166">Presence.Read.All</span></span> | <span data-ttu-id="ebf6b-167">不支持</span><span class="sxs-lookup"><span data-stu-id="ebf6b-167">Not supported</span></span> | <span data-ttu-id="ebf6b-168">不支持</span><span class="sxs-lookup"><span data-stu-id="ebf6b-168">Not supported</span></span> |
|<span data-ttu-id="ebf6b-169">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="ebf6b-169">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="ebf6b-170">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebf6b-170">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="ebf6b-171">不支持</span><span class="sxs-lookup"><span data-stu-id="ebf6b-171">Not supported</span></span> | <span data-ttu-id="ebf6b-172">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebf6b-172">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="ebf6b-173">用户</span><span class="sxs-lookup"><span data-stu-id="ebf6b-173">user</span></span>](../resources/user.md) | <span data-ttu-id="ebf6b-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ebf6b-174">User.Read.All</span></span> | <span data-ttu-id="ebf6b-175">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ebf6b-175">User.Read.All</span></span> | <span data-ttu-id="ebf6b-176">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ebf6b-176">User.Read.All</span></span> |

### <a name="chatmessage"></a><span data-ttu-id="ebf6b-177">chatMessage</span><span class="sxs-lookup"><span data-stu-id="ebf6b-177">chatMessage</span></span>

<span data-ttu-id="ebf6b-178">具有委派权限的**了 chatmessage**订阅不支持资源数据 (**includeResourceData**必须 `false`) ，并且不需要[加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-178">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="ebf6b-179">具有应用程序权限的**了 chatmessage**订阅包括资源数据，并需要[加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-179">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="ebf6b-180">如果未指定 [encryptionCertificate](../resources/subscription.md) ，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-180">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="ebf6b-181">在创建 **了 chatmessage** 订阅之前，您必须请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-181">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="ebf6b-182">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-182">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="ebf6b-183">**注意：** `/teams/allMessages` ，并且 `/chats/allMessages` 当前处于预览阶段。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-183">**Note:** `/teams/allMessages` and `/chats/allMessages` are currently in preview.</span></span> <span data-ttu-id="ebf6b-184">在预览过程中，可以在不付费的情况下使用此 API，这取决于 [Microsoft Api 使用条款](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context)。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-184">During the preview, you may use this API without fees, subject to the [Microsoft APIs Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span></span> <span data-ttu-id="ebf6b-185">但是，使用 API 的应用程序的用户可能需要订阅特定 Microsoft 365 产品。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-185">However, users of apps that use the API might be required to have subscriptions to specific Microsoft 365 offerings.</span></span> <span data-ttu-id="ebf6b-186">在正式发行时，Microsoft 可能会要求您或您的客户根据通过 API 访问的数据量支付额外费用。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-186">Upon general availability, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>

### <a name="driveitem"></a><span data-ttu-id="ebf6b-187">driveItem</span><span class="sxs-lookup"><span data-stu-id="ebf6b-187">driveItem</span></span>

<span data-ttu-id="ebf6b-188">对 OneDrive 项目的订阅适用其他限制。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-188">Additional limitations apply for subscriptions on OneDrive  items.</span></span> <span data-ttu-id="ebf6b-189">这些限制适用于创建以及管理 (获取、更新和删除) 订阅。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-189">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="ebf6b-190">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-190">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="ebf6b-191">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-191">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="ebf6b-192">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-192">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="ebf6b-193">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-193">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="ebf6b-194">联系人、事件和邮件</span><span class="sxs-lookup"><span data-stu-id="ebf6b-194">contact, event, and message</span></span>

<span data-ttu-id="ebf6b-195">对 Outlook 项目的订阅适用其他限制。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-195">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="ebf6b-196">这些限制适用于创建以及管理 (获取、更新和删除) 订阅。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-196">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="ebf6b-197">委派权限仅支持订阅登录用户的邮箱中的文件夹中的项目。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-197">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="ebf6b-198">也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-198">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="ebf6b-199">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="ebf6b-199">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="ebf6b-200">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-200">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="ebf6b-201">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-201">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="ebf6b-202">状态</span><span class="sxs-lookup"><span data-stu-id="ebf6b-202">presence</span></span>

<span data-ttu-id="ebf6b-203">**状态** 订阅需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-203">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="ebf6b-204">如果未指定 [encryptionCertificate](../resources/subscription.md) ，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-204">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="ebf6b-205">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ebf6b-205">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ebf6b-206">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ebf6b-206">Optional query parameters</span></span>

<span data-ttu-id="ebf6b-207">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-207">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ebf6b-208">请求标头</span><span class="sxs-lookup"><span data-stu-id="ebf6b-208">Request headers</span></span>

| <span data-ttu-id="ebf6b-209">名称</span><span class="sxs-lookup"><span data-stu-id="ebf6b-209">Name</span></span>       | <span data-ttu-id="ebf6b-210">类型</span><span class="sxs-lookup"><span data-stu-id="ebf6b-210">Type</span></span> | <span data-ttu-id="ebf6b-211">说明</span><span class="sxs-lookup"><span data-stu-id="ebf6b-211">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="ebf6b-212">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebf6b-212">Authorization</span></span>  | <span data-ttu-id="ebf6b-213">string</span><span class="sxs-lookup"><span data-stu-id="ebf6b-213">string</span></span>  | <span data-ttu-id="ebf6b-p109">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-p109">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ebf6b-216">请求正文</span><span class="sxs-lookup"><span data-stu-id="ebf6b-216">Request body</span></span>

<span data-ttu-id="ebf6b-217">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-217">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebf6b-218">响应</span><span class="sxs-lookup"><span data-stu-id="ebf6b-218">Response</span></span>

<span data-ttu-id="ebf6b-219">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-219">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebf6b-220">示例</span><span class="sxs-lookup"><span data-stu-id="ebf6b-220">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ebf6b-221">请求</span><span class="sxs-lookup"><span data-stu-id="ebf6b-221">Request</span></span>

<span data-ttu-id="ebf6b-222">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-222">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ebf6b-223">HTTP</span><span class="sxs-lookup"><span data-stu-id="ebf6b-223">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="ebf6b-224">C#</span><span class="sxs-lookup"><span data-stu-id="ebf6b-224">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ebf6b-225">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ebf6b-225">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ebf6b-226">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebf6b-226">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ebf6b-227">响应</span><span class="sxs-lookup"><span data-stu-id="ebf6b-227">Response</span></span>

<span data-ttu-id="ebf6b-228">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ebf6b-228">Here is an example of the response.</span></span>
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
  "applicationId" : "string",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string",
  "latestSupportedTlsVersion": "v1_2"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


