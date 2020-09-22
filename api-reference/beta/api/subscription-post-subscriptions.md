---
title: 创建订阅
description: 订阅侦听器应用程序，以便在 Microsoft Graph 资源上的数据发生更改时接收更改通知。
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: a2a2b112974e25840127a1deabfcb893c53dac1f
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193391"
---
# <a name="create-subscription"></a><span data-ttu-id="2e5c3-103">创建订阅</span><span class="sxs-lookup"><span data-stu-id="2e5c3-103">Create subscription</span></span>

<span data-ttu-id="2e5c3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e5c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e5c3-105">订阅侦听器应用程序，以在 Microsoft Graph 中指定资源发生的更改属于请求的更改类型时接收更改通知。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e5c3-106">权限</span><span class="sxs-lookup"><span data-stu-id="2e5c3-106">Permissions</span></span>

<span data-ttu-id="2e5c3-107">创建订阅需要对资源具有读取权限。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-107">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="2e5c3-108">例如，若要获取邮件的更改通知，您的应用程序需要具有邮件读取权限。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-108">For example, to get change notifications on messages, your app needs the Mail.Read permission.</span></span> 

 <span data-ttu-id="2e5c3-109">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="2e5c3-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2e5c3-111">支持的资源</span><span class="sxs-lookup"><span data-stu-id="2e5c3-111">Supported resource</span></span> | <span data-ttu-id="2e5c3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e5c3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2e5c3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e5c3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e5c3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e5c3-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="2e5c3-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="2e5c3-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="2e5c3-116">不支持</span><span class="sxs-lookup"><span data-stu-id="2e5c3-116">Not supported</span></span> | <span data-ttu-id="2e5c3-117">不支持</span><span class="sxs-lookup"><span data-stu-id="2e5c3-117">Not supported</span></span> | <span data-ttu-id="2e5c3-118">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e5c3-118">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="2e5c3-119">[了 chatmessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages) </span><span class="sxs-lookup"><span data-stu-id="2e5c3-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="2e5c3-120">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e5c3-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="2e5c3-121">不支持</span><span class="sxs-lookup"><span data-stu-id="2e5c3-121">Not supported</span></span> | <span data-ttu-id="2e5c3-122">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e5c3-122">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="2e5c3-123">[了 chatmessage](../resources/chatmessage.md) (/teams/getallmessages--组织中的所有频道邮件) </span><span class="sxs-lookup"><span data-stu-id="2e5c3-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="2e5c3-124">不支持</span><span class="sxs-lookup"><span data-stu-id="2e5c3-124">Not supported</span></span> | <span data-ttu-id="2e5c3-125">不支持</span><span class="sxs-lookup"><span data-stu-id="2e5c3-125">Not supported</span></span> | <span data-ttu-id="2e5c3-126">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e5c3-126">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="2e5c3-127">[了 chatmessage](../resources/chatmessage.md) (/chats/{id}/messages) </span><span class="sxs-lookup"><span data-stu-id="2e5c3-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="2e5c3-128">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e5c3-128">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="2e5c3-129">不支持</span><span class="sxs-lookup"><span data-stu-id="2e5c3-129">Not supported</span></span> | <span data-ttu-id="2e5c3-130">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e5c3-130">Chat.Read.All</span></span>  |
|<span data-ttu-id="2e5c3-131">[了 chatmessage](../resources/chatmessage.md) (/chats/getallmessages--组织中的所有聊天邮件) </span><span class="sxs-lookup"><span data-stu-id="2e5c3-131">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="2e5c3-132">不支持</span><span class="sxs-lookup"><span data-stu-id="2e5c3-132">Not supported</span></span> | <span data-ttu-id="2e5c3-133">不支持</span><span class="sxs-lookup"><span data-stu-id="2e5c3-133">Not supported</span></span> | <span data-ttu-id="2e5c3-134">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e5c3-134">Chat.Read.All</span></span>  |
|[<span data-ttu-id="2e5c3-135">联系人</span><span class="sxs-lookup"><span data-stu-id="2e5c3-135">contact</span></span>](../resources/contact.md) | <span data-ttu-id="2e5c3-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2e5c3-136">Contacts.Read</span></span> | <span data-ttu-id="2e5c3-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2e5c3-137">Contacts.Read</span></span> | <span data-ttu-id="2e5c3-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2e5c3-138">Contacts.Read</span></span> |
|<span data-ttu-id="2e5c3-139">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="2e5c3-139">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="2e5c3-140">不支持</span><span class="sxs-lookup"><span data-stu-id="2e5c3-140">Not supported</span></span> | <span data-ttu-id="2e5c3-141">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e5c3-141">Files.ReadWrite</span></span> | <span data-ttu-id="2e5c3-142">不支持</span><span class="sxs-lookup"><span data-stu-id="2e5c3-142">Not supported</span></span> |
|<span data-ttu-id="2e5c3-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="2e5c3-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="2e5c3-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e5c3-144">Files.ReadWrite.All</span></span> | <span data-ttu-id="2e5c3-145">不支持</span><span class="sxs-lookup"><span data-stu-id="2e5c3-145">Not supported</span></span> | <span data-ttu-id="2e5c3-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e5c3-146">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="2e5c3-147">事件</span><span class="sxs-lookup"><span data-stu-id="2e5c3-147">event</span></span>](../resources/event.md) | <span data-ttu-id="2e5c3-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2e5c3-148">Calendars.Read</span></span> | <span data-ttu-id="2e5c3-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2e5c3-149">Calendars.Read</span></span> | <span data-ttu-id="2e5c3-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2e5c3-150">Calendars.Read</span></span> |
|[<span data-ttu-id="2e5c3-151">组</span><span class="sxs-lookup"><span data-stu-id="2e5c3-151">group</span></span>](../resources/group.md) | <span data-ttu-id="2e5c3-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e5c3-152">Group.Read.All</span></span> | <span data-ttu-id="2e5c3-153">不支持</span><span class="sxs-lookup"><span data-stu-id="2e5c3-153">Not supported</span></span> | <span data-ttu-id="2e5c3-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e5c3-154">Group.Read.All</span></span> |
|[<span data-ttu-id="2e5c3-155">组对话</span><span class="sxs-lookup"><span data-stu-id="2e5c3-155">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="2e5c3-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e5c3-156">Group.Read.All</span></span> | <span data-ttu-id="2e5c3-157">不支持</span><span class="sxs-lookup"><span data-stu-id="2e5c3-157">Not supported</span></span> | <span data-ttu-id="2e5c3-158">不支持</span><span class="sxs-lookup"><span data-stu-id="2e5c3-158">Not supported</span></span> |
|[<span data-ttu-id="2e5c3-159">列表</span><span class="sxs-lookup"><span data-stu-id="2e5c3-159">list</span></span>](../resources/list.md) | <span data-ttu-id="2e5c3-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e5c3-160">Sites.ReadWrite.All</span></span> | <span data-ttu-id="2e5c3-161">不支持</span><span class="sxs-lookup"><span data-stu-id="2e5c3-161">Not supported</span></span> | <span data-ttu-id="2e5c3-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e5c3-162">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="2e5c3-163">邮件</span><span class="sxs-lookup"><span data-stu-id="2e5c3-163">message</span></span>](../resources/message.md) | <span data-ttu-id="2e5c3-164">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2e5c3-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="2e5c3-165">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2e5c3-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="2e5c3-166">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2e5c3-166">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="2e5c3-167">状态</span><span class="sxs-lookup"><span data-stu-id="2e5c3-167">presence</span></span>](../resources/presence.md) | <span data-ttu-id="2e5c3-168">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e5c3-168">Presence.Read.All</span></span> | <span data-ttu-id="2e5c3-169">不支持</span><span class="sxs-lookup"><span data-stu-id="2e5c3-169">Not supported</span></span> | <span data-ttu-id="2e5c3-170">不支持</span><span class="sxs-lookup"><span data-stu-id="2e5c3-170">Not supported</span></span> |
|<span data-ttu-id="2e5c3-171">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="2e5c3-171">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="2e5c3-172">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e5c3-172">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="2e5c3-173">不支持</span><span class="sxs-lookup"><span data-stu-id="2e5c3-173">Not supported</span></span> | <span data-ttu-id="2e5c3-174">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e5c3-174">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="2e5c3-175">用户</span><span class="sxs-lookup"><span data-stu-id="2e5c3-175">user</span></span>](../resources/user.md) | <span data-ttu-id="2e5c3-176">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e5c3-176">User.Read.All</span></span> | <span data-ttu-id="2e5c3-177">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e5c3-177">User.Read.All</span></span> | <span data-ttu-id="2e5c3-178">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e5c3-178">User.Read.All</span></span> |

### <a name="chatmessage"></a><span data-ttu-id="2e5c3-179">chatMessage</span><span class="sxs-lookup"><span data-stu-id="2e5c3-179">chatMessage</span></span>

<span data-ttu-id="2e5c3-180">具有委派权限的**了 chatmessage**订阅不支持资源数据 (**includeResourceData**必须 `false`) ，并且不需要[加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-180">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="2e5c3-181">具有应用程序权限的**了 chatmessage**订阅包括资源数据，并需要[加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-181">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="2e5c3-182">如果未指定 [encryptionCertificate](../resources/subscription.md) ，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-182">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="2e5c3-183">在创建 **了 chatmessage** 订阅之前，您必须请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-183">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="2e5c3-184">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-184">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="2e5c3-185">**注意：** `/teams/getAllMessages`并 `/chats/getAllMessages` 可供具有  
 [所需许可证](https://aka.ms/teams-changenotification-licenses)的用户使用。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-185">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the 
[required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="2e5c3-186">driveItem</span><span class="sxs-lookup"><span data-stu-id="2e5c3-186">driveItem</span></span>

<span data-ttu-id="2e5c3-187">对 OneDrive 项目的订阅适用其他限制。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-187">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="2e5c3-188">这些限制适用于创建以及管理 (获取、更新和删除) 订阅。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-188">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="2e5c3-189">在个人 OneDrive 上，您可以订阅该驱动器中的根文件夹或任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-189">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="2e5c3-190">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-190">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="2e5c3-191">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-191">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="2e5c3-192">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-192">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="2e5c3-193">联系人、事件和邮件</span><span class="sxs-lookup"><span data-stu-id="2e5c3-193">contact, event, and message</span></span>

<span data-ttu-id="2e5c3-194">对 Outlook 项目的订阅适用其他限制。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-194">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="2e5c3-195">这些限制适用于创建以及管理 (获取、更新和删除) 订阅。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-195">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="2e5c3-196">委派权限仅支持订阅登录用户的邮箱中的文件夹中的项目。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-196">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="2e5c3-197">例如，不能使用委派的权限日历。读取它可订阅其他用户的邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-197">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="2e5c3-198">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="2e5c3-198">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="2e5c3-199">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-199">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="2e5c3-200">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-200">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="2e5c3-201">状态</span><span class="sxs-lookup"><span data-stu-id="2e5c3-201">presence</span></span>

<span data-ttu-id="2e5c3-202">**状态** 订阅需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-202">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="2e5c3-203">如果未指定 [encryptionCertificate](../resources/subscription.md) ，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-203">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="2e5c3-204">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e5c3-204">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="2e5c3-205">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e5c3-205">Request headers</span></span>

| <span data-ttu-id="2e5c3-206">名称</span><span class="sxs-lookup"><span data-stu-id="2e5c3-206">Name</span></span>       | <span data-ttu-id="2e5c3-207">类型</span><span class="sxs-lookup"><span data-stu-id="2e5c3-207">Type</span></span> | <span data-ttu-id="2e5c3-208">说明</span><span class="sxs-lookup"><span data-stu-id="2e5c3-208">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2e5c3-209">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e5c3-209">Authorization</span></span>  | <span data-ttu-id="2e5c3-210">string</span><span class="sxs-lookup"><span data-stu-id="2e5c3-210">string</span></span>  | <span data-ttu-id="2e5c3-p109">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-p109">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2e5c3-213">响应</span><span class="sxs-lookup"><span data-stu-id="2e5c3-213">Response</span></span>

<span data-ttu-id="2e5c3-214">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [订阅](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-214">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="2e5c3-215">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-215">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="2e5c3-216">示例</span><span class="sxs-lookup"><span data-stu-id="2e5c3-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e5c3-217">请求</span><span class="sxs-lookup"><span data-stu-id="2e5c3-217">Request</span></span>

<span data-ttu-id="2e5c3-218">在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-218">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="2e5c3-219">`clientState` 和 `latestSupportedTlsVersion` 是可选字段。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-219">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="2e5c3-220">此请求创建订阅，以获取当前登录用户接收到的新邮件的更改通知。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-220">This request creates a subscription for change notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e5c3-221">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e5c3-221">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2e5c3-222">C#</span><span class="sxs-lookup"><span data-stu-id="2e5c3-222">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e5c3-223">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e5c3-223">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e5c3-224">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e5c3-224">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="2e5c3-225">在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-225">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="2e5c3-226">`clientState` 和 `latestSupportedTlsVersion` 是可选字段。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-226">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

#### <a name="resources-examples"></a><span data-ttu-id="2e5c3-227">资源示例</span><span class="sxs-lookup"><span data-stu-id="2e5c3-227">Resources examples</span></span>

<span data-ttu-id="2e5c3-228">以下是 resource 属性的有效值。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-228">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="2e5c3-229">资源类型</span><span class="sxs-lookup"><span data-stu-id="2e5c3-229">Resource type</span></span> | <span data-ttu-id="2e5c3-230">示例</span><span class="sxs-lookup"><span data-stu-id="2e5c3-230">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="2e5c3-231">通话记录</span><span class="sxs-lookup"><span data-stu-id="2e5c3-231">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="2e5c3-232">聊天消息</span><span class="sxs-lookup"><span data-stu-id="2e5c3-232">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="2e5c3-233">`chats/{id}/messages`, `chats/allMessages`, `teams/{id}/channels/{id}/messages`, `teams/allMessages`</span><span class="sxs-lookup"><span data-stu-id="2e5c3-233">`chats/{id}/messages`, `chats/allMessages`, `teams/{id}/channels/{id}/messages`, `teams/allMessages`</span></span> |
|[<span data-ttu-id="2e5c3-234">联系人</span><span class="sxs-lookup"><span data-stu-id="2e5c3-234">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="2e5c3-235">对话</span><span class="sxs-lookup"><span data-stu-id="2e5c3-235">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="2e5c3-236">Drives</span><span class="sxs-lookup"><span data-stu-id="2e5c3-236">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="2e5c3-237">事件</span><span class="sxs-lookup"><span data-stu-id="2e5c3-237">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="2e5c3-238">组</span><span class="sxs-lookup"><span data-stu-id="2e5c3-238">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="2e5c3-239">List</span><span class="sxs-lookup"><span data-stu-id="2e5c3-239">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="2e5c3-240">邮件</span><span class="sxs-lookup"><span data-stu-id="2e5c3-240">Mail</span></span>](../resources/message.md)|<span data-ttu-id="2e5c3-241">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="2e5c3-241">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="2e5c3-242">Shell</span><span class="sxs-lookup"><span data-stu-id="2e5c3-242">Presence</span></span>](../resources/presence.md)| <span data-ttu-id="2e5c3-243">`/communications/presences/{id}` (单个用户) ， `/communications/presences?$filter=id in ({id},{id}…)` (多个用户) </span><span class="sxs-lookup"><span data-stu-id="2e5c3-243">`/communications/presences/{id}` (single user), `/communications/presences?$filter=id in ({id},{id}…)` (multiple users)</span></span>|
|[<span data-ttu-id="2e5c3-244">用户</span><span class="sxs-lookup"><span data-stu-id="2e5c3-244">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="2e5c3-245">安全警报</span><span class="sxs-lookup"><span data-stu-id="2e5c3-245">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'NewAlert'`|

> <span data-ttu-id="2e5c3-246">**注意：** 以此开头的任何路径 `me` 也可以与 `users/{id}` `me` 特定用户而不是当前用户的目标一起使用。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-246">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

### <a name="response"></a><span data-ttu-id="2e5c3-247">响应</span><span class="sxs-lookup"><span data-stu-id="2e5c3-247">Response</span></span>

<span data-ttu-id="2e5c3-248">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-248">The following example shows the response.</span></span> 

><span data-ttu-id="2e5c3-p112">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

### <a name="notification-endpoint-validation"></a><span data-ttu-id="2e5c3-251">通知终结点验证</span><span class="sxs-lookup"><span data-stu-id="2e5c3-251">Notification endpoint validation</span></span>

<span data-ttu-id="2e5c3-252"> (在 **notificationUrl** 属性中指定的订阅通知终结点) 必须能够响应验证请求，如 [设置用户数据中的更改通知](/graph/webhooks#notification-endpoint-validation)中所述。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-252">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="2e5c3-253">如果验证失败，创建订阅请求返回错误“400 请求无效”。</span><span class="sxs-lookup"><span data-stu-id="2e5c3-253">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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


