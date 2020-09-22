---
title: 删除订阅
description: 删除订阅。
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 08166c2570c6c73fbb412a4713b5669b36e57736
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193315"
---
# <a name="delete-subscription"></a><span data-ttu-id="b6c49-103">删除订阅</span><span class="sxs-lookup"><span data-stu-id="b6c49-103">Delete subscription</span></span>

<span data-ttu-id="b6c49-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6c49-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6c49-105">删除订阅。</span><span class="sxs-lookup"><span data-stu-id="b6c49-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6c49-106">权限</span><span class="sxs-lookup"><span data-stu-id="b6c49-106">Permissions</span></span>

<span data-ttu-id="b6c49-107">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="b6c49-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="b6c49-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b6c49-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b6c49-109">支持的资源</span><span class="sxs-lookup"><span data-stu-id="b6c49-109">Supported resource</span></span> | <span data-ttu-id="b6c49-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b6c49-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b6c49-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b6c49-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6c49-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="b6c49-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="b6c49-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="b6c49-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="b6c49-114">不支持</span><span class="sxs-lookup"><span data-stu-id="b6c49-114">Not supported</span></span> | <span data-ttu-id="b6c49-115">不支持</span><span class="sxs-lookup"><span data-stu-id="b6c49-115">Not supported</span></span> | <span data-ttu-id="b6c49-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6c49-116">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="b6c49-117">[了 chatmessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages) </span><span class="sxs-lookup"><span data-stu-id="b6c49-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="b6c49-118">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6c49-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="b6c49-119">不支持</span><span class="sxs-lookup"><span data-stu-id="b6c49-119">Not supported</span></span> | <span data-ttu-id="b6c49-120">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6c49-120">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="b6c49-121">[了 chatmessage](../resources/chatmessage.md) (/teams/getallmessages--组织中的所有频道邮件) </span><span class="sxs-lookup"><span data-stu-id="b6c49-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="b6c49-122">不支持</span><span class="sxs-lookup"><span data-stu-id="b6c49-122">Not supported</span></span> | <span data-ttu-id="b6c49-123">不支持</span><span class="sxs-lookup"><span data-stu-id="b6c49-123">Not supported</span></span> | <span data-ttu-id="b6c49-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6c49-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="b6c49-125">[了 chatmessage](../resources/chatmessage.md) (/chats/{id}/messages) </span><span class="sxs-lookup"><span data-stu-id="b6c49-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="b6c49-126">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6c49-126">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="b6c49-127">不支持</span><span class="sxs-lookup"><span data-stu-id="b6c49-127">Not supported</span></span> | <span data-ttu-id="b6c49-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6c49-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="b6c49-129">[了 chatmessage](../resources/chatmessage.md) (/chats/getallmessages--组织中的所有聊天邮件) </span><span class="sxs-lookup"><span data-stu-id="b6c49-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="b6c49-130">不支持</span><span class="sxs-lookup"><span data-stu-id="b6c49-130">Not supported</span></span> | <span data-ttu-id="b6c49-131">不支持</span><span class="sxs-lookup"><span data-stu-id="b6c49-131">Not supported</span></span> | <span data-ttu-id="b6c49-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6c49-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="b6c49-133">联系人</span><span class="sxs-lookup"><span data-stu-id="b6c49-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="b6c49-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b6c49-134">Contacts.Read</span></span> | <span data-ttu-id="b6c49-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b6c49-135">Contacts.Read</span></span> | <span data-ttu-id="b6c49-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b6c49-136">Contacts.Read</span></span> |
|<span data-ttu-id="b6c49-137">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="b6c49-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="b6c49-138">不支持</span><span class="sxs-lookup"><span data-stu-id="b6c49-138">Not supported</span></span> | <span data-ttu-id="b6c49-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6c49-139">Files.ReadWrite</span></span> | <span data-ttu-id="b6c49-140">不支持</span><span class="sxs-lookup"><span data-stu-id="b6c49-140">Not supported</span></span> |
|<span data-ttu-id="b6c49-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="b6c49-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="b6c49-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6c49-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="b6c49-143">不支持</span><span class="sxs-lookup"><span data-stu-id="b6c49-143">Not supported</span></span> | <span data-ttu-id="b6c49-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6c49-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="b6c49-145">事件</span><span class="sxs-lookup"><span data-stu-id="b6c49-145">event</span></span>](../resources/event.md) | <span data-ttu-id="b6c49-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b6c49-146">Calendars.Read</span></span> | <span data-ttu-id="b6c49-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b6c49-147">Calendars.Read</span></span> | <span data-ttu-id="b6c49-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b6c49-148">Calendars.Read</span></span> |
|[<span data-ttu-id="b6c49-149">组</span><span class="sxs-lookup"><span data-stu-id="b6c49-149">group</span></span>](../resources/group.md) | <span data-ttu-id="b6c49-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6c49-150">Group.Read.All</span></span> | <span data-ttu-id="b6c49-151">不支持</span><span class="sxs-lookup"><span data-stu-id="b6c49-151">Not supported</span></span> | <span data-ttu-id="b6c49-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6c49-152">Group.Read.All</span></span> |
|[<span data-ttu-id="b6c49-153">组对话</span><span class="sxs-lookup"><span data-stu-id="b6c49-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="b6c49-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6c49-154">Group.Read.All</span></span> | <span data-ttu-id="b6c49-155">不支持</span><span class="sxs-lookup"><span data-stu-id="b6c49-155">Not supported</span></span> | <span data-ttu-id="b6c49-156">不支持</span><span class="sxs-lookup"><span data-stu-id="b6c49-156">Not supported</span></span> |
|[<span data-ttu-id="b6c49-157">列表</span><span class="sxs-lookup"><span data-stu-id="b6c49-157">list</span></span>](../resources/list.md) | <span data-ttu-id="b6c49-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6c49-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="b6c49-159">不支持</span><span class="sxs-lookup"><span data-stu-id="b6c49-159">Not supported</span></span> | <span data-ttu-id="b6c49-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6c49-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="b6c49-161">邮件</span><span class="sxs-lookup"><span data-stu-id="b6c49-161">message</span></span>](../resources/message.md) | <span data-ttu-id="b6c49-162">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b6c49-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="b6c49-163">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b6c49-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="b6c49-164">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b6c49-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="b6c49-165">状态</span><span class="sxs-lookup"><span data-stu-id="b6c49-165">presence</span></span>](../resources/presence.md) | <span data-ttu-id="b6c49-166">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6c49-166">Presence.Read.All</span></span> | <span data-ttu-id="b6c49-167">不支持</span><span class="sxs-lookup"><span data-stu-id="b6c49-167">Not supported</span></span> | <span data-ttu-id="b6c49-168">不支持</span><span class="sxs-lookup"><span data-stu-id="b6c49-168">Not supported</span></span> |
|<span data-ttu-id="b6c49-169">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="b6c49-169">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="b6c49-170">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6c49-170">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="b6c49-171">不支持</span><span class="sxs-lookup"><span data-stu-id="b6c49-171">Not supported</span></span> | <span data-ttu-id="b6c49-172">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6c49-172">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="b6c49-173">用户</span><span class="sxs-lookup"><span data-stu-id="b6c49-173">user</span></span>](../resources/user.md) | <span data-ttu-id="b6c49-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6c49-174">User.Read.All</span></span> | <span data-ttu-id="b6c49-175">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6c49-175">User.Read.All</span></span> | <span data-ttu-id="b6c49-176">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6c49-176">User.Read.All</span></span> |

### <a name="chatmessage"></a><span data-ttu-id="b6c49-177">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b6c49-177">chatMessage</span></span>

<span data-ttu-id="b6c49-178">具有委派权限的**了 chatmessage**订阅不支持资源数据 (**includeResourceData**必须 `false`) ，并且不需要[加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="b6c49-178">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="b6c49-179">具有应用程序权限的**了 chatmessage**订阅包括资源数据，并需要[加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="b6c49-179">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="b6c49-180">如果未指定 [encryptionCertificate](../resources/subscription.md) ，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="b6c49-180">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="b6c49-181">在创建 **了 chatmessage** 订阅之前，您必须请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="b6c49-181">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="b6c49-182">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="b6c49-182">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="b6c49-183">**注意：** `/teams/getAllMessages`并 `/chats/getAllMessages` 可供具有  
 [所需许可证](https://aka.ms/teams-changenotification-licenses)的用户使用。</span><span class="sxs-lookup"><span data-stu-id="b6c49-183">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the 
[required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="b6c49-184">driveItem</span><span class="sxs-lookup"><span data-stu-id="b6c49-184">driveItem</span></span>

<span data-ttu-id="b6c49-185">对 OneDrive 项目的订阅适用其他限制。</span><span class="sxs-lookup"><span data-stu-id="b6c49-185">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="b6c49-186">这些限制适用于创建以及管理 (获取、更新和删除) 订阅。</span><span class="sxs-lookup"><span data-stu-id="b6c49-186">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="b6c49-187">在个人 OneDrive 上，您可以订阅该驱动器中的根文件夹或任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="b6c49-187">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="b6c49-188">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="b6c49-188">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="b6c49-189">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="b6c49-189">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="b6c49-190">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="b6c49-190">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="b6c49-191">联系人、事件和邮件</span><span class="sxs-lookup"><span data-stu-id="b6c49-191">contact, event, and message</span></span>

<span data-ttu-id="b6c49-192">对 Outlook 项目的订阅适用其他限制。</span><span class="sxs-lookup"><span data-stu-id="b6c49-192">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="b6c49-193">这些限制适用于创建以及管理 (获取、更新和删除) 订阅。</span><span class="sxs-lookup"><span data-stu-id="b6c49-193">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="b6c49-194">委派权限仅支持订阅登录用户的邮箱中的文件夹中的项目。</span><span class="sxs-lookup"><span data-stu-id="b6c49-194">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="b6c49-195">例如，不能使用委派的权限日历。读取它可订阅其他用户的邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="b6c49-195">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="b6c49-196">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="b6c49-196">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="b6c49-197">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="b6c49-197">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="b6c49-198">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="b6c49-198">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="b6c49-199">状态</span><span class="sxs-lookup"><span data-stu-id="b6c49-199">presence</span></span>

<span data-ttu-id="b6c49-200">**状态** 订阅需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="b6c49-200">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="b6c49-201">如果未指定 [encryptionCertificate](../resources/subscription.md) ，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="b6c49-201">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="b6c49-202">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b6c49-202">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b6c49-203">请求标头</span><span class="sxs-lookup"><span data-stu-id="b6c49-203">Request headers</span></span>

| <span data-ttu-id="b6c49-204">名称</span><span class="sxs-lookup"><span data-stu-id="b6c49-204">Name</span></span>       | <span data-ttu-id="b6c49-205">类型</span><span class="sxs-lookup"><span data-stu-id="b6c49-205">Type</span></span> | <span data-ttu-id="b6c49-206">说明</span><span class="sxs-lookup"><span data-stu-id="b6c49-206">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b6c49-207">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6c49-207">Authorization</span></span>  | <span data-ttu-id="b6c49-208">string</span><span class="sxs-lookup"><span data-stu-id="b6c49-208">string</span></span>  | <span data-ttu-id="b6c49-p108">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b6c49-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6c49-211">请求正文</span><span class="sxs-lookup"><span data-stu-id="b6c49-211">Request body</span></span>

<span data-ttu-id="b6c49-212">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b6c49-212">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6c49-213">响应</span><span class="sxs-lookup"><span data-stu-id="b6c49-213">Response</span></span>

<span data-ttu-id="b6c49-214">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b6c49-214">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="b6c49-215">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="b6c49-215">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="b6c49-216">示例</span><span class="sxs-lookup"><span data-stu-id="b6c49-216">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b6c49-217">请求</span><span class="sxs-lookup"><span data-stu-id="b6c49-217">Request</span></span>

<span data-ttu-id="b6c49-218">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b6c49-218">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b6c49-219">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6c49-219">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="b6c49-220">C#</span><span class="sxs-lookup"><span data-stu-id="b6c49-220">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6c49-221">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6c49-221">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6c49-222">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6c49-222">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b6c49-223">响应</span><span class="sxs-lookup"><span data-stu-id="b6c49-223">Response</span></span>

<span data-ttu-id="b6c49-224">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b6c49-224">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


