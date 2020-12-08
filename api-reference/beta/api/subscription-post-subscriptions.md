---
title: 创建订阅
description: 订阅侦听器应用程序，以便在 Microsoft Graph 资源上的数据发生更改时接收更改通知。
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 850d0f893678ce51e502dcdeb560f816b5ff935c
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597429"
---
# <a name="create-subscription"></a><span data-ttu-id="f4c35-103">创建订阅</span><span class="sxs-lookup"><span data-stu-id="f4c35-103">Create subscription</span></span>

<span data-ttu-id="f4c35-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4c35-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4c35-105">订阅侦听器应用程序，以在 Microsoft Graph 中指定资源发生的更改属于请求的更改类型时接收更改通知。</span><span class="sxs-lookup"><span data-stu-id="f4c35-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4c35-106">权限</span><span class="sxs-lookup"><span data-stu-id="f4c35-106">Permissions</span></span>

<span data-ttu-id="f4c35-107">创建订阅需要对资源具有读取权限。</span><span class="sxs-lookup"><span data-stu-id="f4c35-107">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="f4c35-108">例如，若要获取邮件的更改通知，您的应用程序需要具有邮件读取权限。</span><span class="sxs-lookup"><span data-stu-id="f4c35-108">For example, to get change notifications on messages, your app needs the Mail.Read permission.</span></span> 

 <span data-ttu-id="f4c35-109">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="f4c35-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="f4c35-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4c35-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f4c35-111">支持的资源</span><span class="sxs-lookup"><span data-stu-id="f4c35-111">Supported resource</span></span> | <span data-ttu-id="f4c35-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4c35-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f4c35-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4c35-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4c35-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4c35-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="f4c35-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="f4c35-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="f4c35-116">不支持</span><span class="sxs-lookup"><span data-stu-id="f4c35-116">Not supported</span></span> | <span data-ttu-id="f4c35-117">不支持</span><span class="sxs-lookup"><span data-stu-id="f4c35-117">Not supported</span></span> | <span data-ttu-id="f4c35-118">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4c35-118">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="f4c35-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="f4c35-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="f4c35-120">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4c35-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="f4c35-121">不支持</span><span class="sxs-lookup"><span data-stu-id="f4c35-121">Not supported</span></span> | <span data-ttu-id="f4c35-122">ChannelMessage \*、ChannelMessage \*。</span><span class="sxs-lookup"><span data-stu-id="f4c35-122">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="f4c35-123">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="f4c35-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="f4c35-124">不支持</span><span class="sxs-lookup"><span data-stu-id="f4c35-124">Not supported</span></span> | <span data-ttu-id="f4c35-125">不支持</span><span class="sxs-lookup"><span data-stu-id="f4c35-125">Not supported</span></span> | <span data-ttu-id="f4c35-126">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4c35-126">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="f4c35-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="f4c35-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="f4c35-128">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4c35-128">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="f4c35-129">不支持</span><span class="sxs-lookup"><span data-stu-id="f4c35-129">Not supported</span></span> | <span data-ttu-id="f4c35-130">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4c35-130">Chat.Read.All</span></span>  |
|<span data-ttu-id="f4c35-131">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="f4c35-131">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="f4c35-132">不支持</span><span class="sxs-lookup"><span data-stu-id="f4c35-132">Not supported</span></span> | <span data-ttu-id="f4c35-133">不支持</span><span class="sxs-lookup"><span data-stu-id="f4c35-133">Not supported</span></span> | <span data-ttu-id="f4c35-134">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4c35-134">Chat.Read.All</span></span>  |
|[<span data-ttu-id="f4c35-135">contact</span><span class="sxs-lookup"><span data-stu-id="f4c35-135">contact</span></span>](../resources/contact.md) | <span data-ttu-id="f4c35-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f4c35-136">Contacts.Read</span></span> | <span data-ttu-id="f4c35-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f4c35-137">Contacts.Read</span></span> | <span data-ttu-id="f4c35-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f4c35-138">Contacts.Read</span></span> |
|<span data-ttu-id="f4c35-139">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="f4c35-139">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="f4c35-140">不支持</span><span class="sxs-lookup"><span data-stu-id="f4c35-140">Not supported</span></span> | <span data-ttu-id="f4c35-141">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4c35-141">Files.ReadWrite</span></span> | <span data-ttu-id="f4c35-142">不支持</span><span class="sxs-lookup"><span data-stu-id="f4c35-142">Not supported</span></span> |
|<span data-ttu-id="f4c35-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="f4c35-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="f4c35-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4c35-144">Files.ReadWrite.All</span></span> | <span data-ttu-id="f4c35-145">不支持</span><span class="sxs-lookup"><span data-stu-id="f4c35-145">Not supported</span></span> | <span data-ttu-id="f4c35-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4c35-146">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="f4c35-147">事件</span><span class="sxs-lookup"><span data-stu-id="f4c35-147">event</span></span>](../resources/event.md) | <span data-ttu-id="f4c35-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f4c35-148">Calendars.Read</span></span> | <span data-ttu-id="f4c35-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f4c35-149">Calendars.Read</span></span> | <span data-ttu-id="f4c35-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f4c35-150">Calendars.Read</span></span> |
|[<span data-ttu-id="f4c35-151">组</span><span class="sxs-lookup"><span data-stu-id="f4c35-151">group</span></span>](../resources/group.md) | <span data-ttu-id="f4c35-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4c35-152">Group.Read.All</span></span> | <span data-ttu-id="f4c35-153">不支持</span><span class="sxs-lookup"><span data-stu-id="f4c35-153">Not supported</span></span> | <span data-ttu-id="f4c35-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4c35-154">Group.Read.All</span></span> |
|[<span data-ttu-id="f4c35-155">组对话</span><span class="sxs-lookup"><span data-stu-id="f4c35-155">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="f4c35-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4c35-156">Group.Read.All</span></span> | <span data-ttu-id="f4c35-157">不支持</span><span class="sxs-lookup"><span data-stu-id="f4c35-157">Not supported</span></span> | <span data-ttu-id="f4c35-158">不支持</span><span class="sxs-lookup"><span data-stu-id="f4c35-158">Not supported</span></span> |
|[<span data-ttu-id="f4c35-159">列表</span><span class="sxs-lookup"><span data-stu-id="f4c35-159">list</span></span>](../resources/list.md) | <span data-ttu-id="f4c35-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4c35-160">Sites.ReadWrite.All</span></span> | <span data-ttu-id="f4c35-161">不支持</span><span class="sxs-lookup"><span data-stu-id="f4c35-161">Not supported</span></span> | <span data-ttu-id="f4c35-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4c35-162">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="f4c35-163">邮件</span><span class="sxs-lookup"><span data-stu-id="f4c35-163">message</span></span>](../resources/message.md) | <span data-ttu-id="f4c35-164">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f4c35-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="f4c35-165">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f4c35-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="f4c35-166">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f4c35-166">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="f4c35-167">状态</span><span class="sxs-lookup"><span data-stu-id="f4c35-167">presence</span></span>](../resources/presence.md) | <span data-ttu-id="f4c35-168">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4c35-168">Presence.Read.All</span></span> | <span data-ttu-id="f4c35-169">不支持</span><span class="sxs-lookup"><span data-stu-id="f4c35-169">Not supported</span></span> | <span data-ttu-id="f4c35-170">不支持</span><span class="sxs-lookup"><span data-stu-id="f4c35-170">Not supported</span></span> |
|[<span data-ttu-id="f4c35-171">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="f4c35-171">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="f4c35-172">不支持</span><span class="sxs-lookup"><span data-stu-id="f4c35-172">Not supported</span></span> | <span data-ttu-id="f4c35-173">不支持</span><span class="sxs-lookup"><span data-stu-id="f4c35-173">Not supported</span></span> | <span data-ttu-id="f4c35-174">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4c35-174">PrintTaskDefinition.ReadWrite.All</span></span> |
|<span data-ttu-id="f4c35-175">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="f4c35-175">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="f4c35-176">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4c35-176">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="f4c35-177">不支持</span><span class="sxs-lookup"><span data-stu-id="f4c35-177">Not supported</span></span> | <span data-ttu-id="f4c35-178">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4c35-178">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="f4c35-179">todoTask</span><span class="sxs-lookup"><span data-stu-id="f4c35-179">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="f4c35-180">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4c35-180">Tasks.ReadWrite</span></span> | <span data-ttu-id="f4c35-181">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4c35-181">Tasks.ReadWrite</span></span> | <span data-ttu-id="f4c35-182">不支持</span><span class="sxs-lookup"><span data-stu-id="f4c35-182">Not supported</span></span> |
|[<span data-ttu-id="f4c35-183">用户</span><span class="sxs-lookup"><span data-stu-id="f4c35-183">user</span></span>](../resources/user.md) | <span data-ttu-id="f4c35-184">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4c35-184">User.Read.All</span></span> | <span data-ttu-id="f4c35-185">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4c35-185">User.Read.All</span></span> | <span data-ttu-id="f4c35-186">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4c35-186">User.Read.All</span></span> |

> <span data-ttu-id="f4c35-187">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="f4c35-187">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="f4c35-188">chatMessage</span><span class="sxs-lookup"><span data-stu-id="f4c35-188">chatMessage</span></span>

<span data-ttu-id="f4c35-189">具有委派权限的 **了 chatmessage** 订阅不支持资源数据 (**includeResourceData** 必须 `false`) ，并且不需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="f4c35-189">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="f4c35-190">具有应用程序权限的 **chatMessage** 订阅包含资源数据，并且需要进行 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="f4c35-190">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="f4c35-191">如果未指定 [encryptionCertificate](../resources/subscription.md)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="f4c35-191">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="f4c35-192">创建 **chatMessage** 订阅前，必须请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="f4c35-192">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="f4c35-193">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="f4c35-193">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="f4c35-194">**注意：** `/teams/getAllMessages` 和 `/chats/getAllMessages` 可供拥有 [所需许可证](https://aka.ms/teams-changenotification-licenses)的用户使用。</span><span class="sxs-lookup"><span data-stu-id="f4c35-194">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

> <span data-ttu-id="f4c35-195">**注意：** `/chats/getAllMessages` 仅返回租户所拥有的来自聊天的邮件。</span><span class="sxs-lookup"><span data-stu-id="f4c35-195">**Note:** `/chats/getAllMessages` only returns messages from chats owned by the tenant.</span></span> <span data-ttu-id="f4c35-196">如果由租户外部的用户启动聊天线程，则该聊天线程不归租户所有，并且不会创建更改通知。</span><span class="sxs-lookup"><span data-stu-id="f4c35-196">If a chat thread is initiated by a user outside the tenant, that chat thread is not owned by the tenant, and does not create change notifications.</span></span>

### <a name="driveitem"></a><span data-ttu-id="f4c35-197">driveItem</span><span class="sxs-lookup"><span data-stu-id="f4c35-197">driveItem</span></span>

<span data-ttu-id="f4c35-198">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="f4c35-198">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="f4c35-199">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="f4c35-199">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="f4c35-200">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="f4c35-200">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="f4c35-201">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="f4c35-201">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="f4c35-202">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="f4c35-202">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="f4c35-203">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="f4c35-203">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="f4c35-204">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="f4c35-204">contact, event, and message</span></span>

<span data-ttu-id="f4c35-205">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="f4c35-205">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="f4c35-206">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="f4c35-206">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="f4c35-207">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="f4c35-207">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="f4c35-208">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="f4c35-208">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="f4c35-209">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="f4c35-209">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="f4c35-210">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="f4c35-210">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="f4c35-211">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="f4c35-211">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="f4c35-212">状态</span><span class="sxs-lookup"><span data-stu-id="f4c35-212">presence</span></span>

<span data-ttu-id="f4c35-213">**状态** 订阅需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="f4c35-213">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="f4c35-214">如果未指定 [encryptionCertificate](../resources/subscription.md)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="f4c35-214">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="f4c35-215">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4c35-215">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="f4c35-216">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4c35-216">Request headers</span></span>

| <span data-ttu-id="f4c35-217">名称</span><span class="sxs-lookup"><span data-stu-id="f4c35-217">Name</span></span>       | <span data-ttu-id="f4c35-218">类型</span><span class="sxs-lookup"><span data-stu-id="f4c35-218">Type</span></span> | <span data-ttu-id="f4c35-219">说明</span><span class="sxs-lookup"><span data-stu-id="f4c35-219">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f4c35-220">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4c35-220">Authorization</span></span>  | <span data-ttu-id="f4c35-221">string</span><span class="sxs-lookup"><span data-stu-id="f4c35-221">string</span></span>  | <span data-ttu-id="f4c35-p110">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f4c35-p110">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f4c35-224">响应</span><span class="sxs-lookup"><span data-stu-id="f4c35-224">Response</span></span>

<span data-ttu-id="f4c35-225">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [订阅](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f4c35-225">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="f4c35-226">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="f4c35-226">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="f4c35-227">示例</span><span class="sxs-lookup"><span data-stu-id="f4c35-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4c35-228">请求</span><span class="sxs-lookup"><span data-stu-id="f4c35-228">Request</span></span>

<span data-ttu-id="f4c35-229">在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4c35-229">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="f4c35-230">`clientState` 和 `latestSupportedTlsVersion` 是可选字段。</span><span class="sxs-lookup"><span data-stu-id="f4c35-230">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="f4c35-231">此请求创建订阅，以获取当前登录用户接收到的新邮件的更改通知。</span><span class="sxs-lookup"><span data-stu-id="f4c35-231">This request creates a subscription for change notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="f4c35-232">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4c35-232">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "created",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue",
   "latestSupportedTlsVersion": "v1_2"
}
```
# <a name="c"></a>[<span data-ttu-id="f4c35-233">C#</span><span class="sxs-lookup"><span data-stu-id="f4c35-233">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4c35-234">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4c35-234">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4c35-235">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4c35-235">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f4c35-236">Java</span><span class="sxs-lookup"><span data-stu-id="f4c35-236">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="f4c35-237">在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4c35-237">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="f4c35-238">`clientState` 和 `latestSupportedTlsVersion` 是可选字段。</span><span class="sxs-lookup"><span data-stu-id="f4c35-238">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

#### <a name="resources-examples"></a><span data-ttu-id="f4c35-239">资源示例</span><span class="sxs-lookup"><span data-stu-id="f4c35-239">Resources examples</span></span>

<span data-ttu-id="f4c35-240">以下是 resource 属性的有效值。</span><span class="sxs-lookup"><span data-stu-id="f4c35-240">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="f4c35-241">资源类型</span><span class="sxs-lookup"><span data-stu-id="f4c35-241">Resource type</span></span> | <span data-ttu-id="f4c35-242">示例</span><span class="sxs-lookup"><span data-stu-id="f4c35-242">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="f4c35-243">通话记录</span><span class="sxs-lookup"><span data-stu-id="f4c35-243">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="f4c35-244">聊天消息</span><span class="sxs-lookup"><span data-stu-id="f4c35-244">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="f4c35-245">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="f4c35-245">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="f4c35-246">联系人</span><span class="sxs-lookup"><span data-stu-id="f4c35-246">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="f4c35-247">对话</span><span class="sxs-lookup"><span data-stu-id="f4c35-247">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="f4c35-248">驱动器</span><span class="sxs-lookup"><span data-stu-id="f4c35-248">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="f4c35-249">事件</span><span class="sxs-lookup"><span data-stu-id="f4c35-249">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="f4c35-250">组</span><span class="sxs-lookup"><span data-stu-id="f4c35-250">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="f4c35-251">列表</span><span class="sxs-lookup"><span data-stu-id="f4c35-251">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="f4c35-252">邮件</span><span class="sxs-lookup"><span data-stu-id="f4c35-252">Mail</span></span>](../resources/message.md)|<span data-ttu-id="f4c35-253">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="f4c35-253">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="f4c35-254">Shell</span><span class="sxs-lookup"><span data-stu-id="f4c35-254">Presence</span></span>](../resources/presence.md)| <span data-ttu-id="f4c35-255">`/communications/presences/{id}` (单个用户) ， `/communications/presences?$filter=id in ({id},{id}…)` (多个用户) </span><span class="sxs-lookup"><span data-stu-id="f4c35-255">`/communications/presences/{id}` (single user), `/communications/presences?$filter=id in ({id},{id}…)` (multiple users)</span></span>|
|[<span data-ttu-id="f4c35-256">PrintTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="f4c35-256">PrintTaskDefinition</span></span>](../resources/printtaskdefinition.md)|`print/taskDefinitions/{id}/tasks`|
|[<span data-ttu-id="f4c35-257">用户</span><span class="sxs-lookup"><span data-stu-id="f4c35-257">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="f4c35-258">todoTask</span><span class="sxs-lookup"><span data-stu-id="f4c35-258">todoTask</span></span>](../resources/todotask.md) | `/me/todo/lists/{todoTaskListId}/tasks`
|[<span data-ttu-id="f4c35-259">安全警报</span><span class="sxs-lookup"><span data-stu-id="f4c35-259">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'NewAlert'`|

> <span data-ttu-id="f4c35-260">**注意：** 以 `me` 开头的任何路径也可与 `users/{id}`（而不是 `me`）一起使用，从而以特定用户为目标，而不是以当前用户为目标。</span><span class="sxs-lookup"><span data-stu-id="f4c35-260">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

### <a name="response"></a><span data-ttu-id="f4c35-261">响应</span><span class="sxs-lookup"><span data-stu-id="f4c35-261">Response</span></span>

<span data-ttu-id="f4c35-262">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="f4c35-262">The following example shows the response.</span></span> 

><span data-ttu-id="f4c35-p113">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f4c35-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "changeType": "created",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2"
}
```

### <a name="notification-endpoint-validation"></a><span data-ttu-id="f4c35-265">通知终结点验证</span><span class="sxs-lookup"><span data-stu-id="f4c35-265">Notification endpoint validation</span></span>

<span data-ttu-id="f4c35-266"> (在 **notificationUrl** 属性中指定的订阅通知终结点) 必须能够响应验证请求，如 [设置用户数据中的更改通知](/graph/webhooks#notification-endpoint-validation)中所述。</span><span class="sxs-lookup"><span data-stu-id="f4c35-266">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="f4c35-267">如果验证失败，创建订阅请求返回错误“400 请求无效”。</span><span class="sxs-lookup"><span data-stu-id="f4c35-267">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

[error-response]: /graph/errors

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
  ]
}
-->


