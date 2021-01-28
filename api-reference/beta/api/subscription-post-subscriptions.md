---
title: 创建订阅
description: 订阅侦听器应用程序，以在 Microsoft Graph 资源上的数据发生更改时接收更改通知。
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 68e748a054812350c7aad029d604e87aa77b7345
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034273"
---
# <a name="create-subscription"></a><span data-ttu-id="800bb-103">创建订阅</span><span class="sxs-lookup"><span data-stu-id="800bb-103">Create subscription</span></span>

<span data-ttu-id="800bb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="800bb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="800bb-105">订阅侦听器应用程序，以在 Microsoft Graph 中指定资源发生的更改属于请求的更改类型时接收更改通知。</span><span class="sxs-lookup"><span data-stu-id="800bb-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="800bb-106">权限</span><span class="sxs-lookup"><span data-stu-id="800bb-106">Permissions</span></span>

<span data-ttu-id="800bb-107">创建订阅需要对资源的读取权限。</span><span class="sxs-lookup"><span data-stu-id="800bb-107">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="800bb-108">例如，若要获取邮件更改通知，您的应用程序需要 Mail.Read 权限。</span><span class="sxs-lookup"><span data-stu-id="800bb-108">For example, to get change notifications on messages, your app needs the Mail.Read permission.</span></span> 

 <span data-ttu-id="800bb-109">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="800bb-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="800bb-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="800bb-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="800bb-111">支持的资源</span><span class="sxs-lookup"><span data-stu-id="800bb-111">Supported resource</span></span> | <span data-ttu-id="800bb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="800bb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="800bb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="800bb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="800bb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="800bb-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="800bb-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="800bb-115">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="800bb-116">不支持</span><span class="sxs-lookup"><span data-stu-id="800bb-116">Not supported</span></span> | <span data-ttu-id="800bb-117">不支持</span><span class="sxs-lookup"><span data-stu-id="800bb-117">Not supported</span></span> | <span data-ttu-id="800bb-118">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="800bb-118">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="800bb-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="800bb-119">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="800bb-120">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="800bb-120">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="800bb-121">不支持</span><span class="sxs-lookup"><span data-stu-id="800bb-121">Not supported</span></span> | <span data-ttu-id="800bb-122">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="800bb-122">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="800bb-123">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="800bb-123">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="800bb-124">不支持</span><span class="sxs-lookup"><span data-stu-id="800bb-124">Not supported</span></span> | <span data-ttu-id="800bb-125">不支持</span><span class="sxs-lookup"><span data-stu-id="800bb-125">Not supported</span></span> | <span data-ttu-id="800bb-126">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="800bb-126">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="800bb-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="800bb-127">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="800bb-128">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="800bb-128">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="800bb-129">不支持</span><span class="sxs-lookup"><span data-stu-id="800bb-129">Not supported</span></span> | <span data-ttu-id="800bb-130">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="800bb-130">Chat.Read.All</span></span>  |
|<span data-ttu-id="800bb-131">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="800bb-131">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="800bb-132">不支持</span><span class="sxs-lookup"><span data-stu-id="800bb-132">Not supported</span></span> | <span data-ttu-id="800bb-133">不支持</span><span class="sxs-lookup"><span data-stu-id="800bb-133">Not supported</span></span> | <span data-ttu-id="800bb-134">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="800bb-134">Chat.Read.All</span></span>  |
|[<span data-ttu-id="800bb-135">contact</span><span class="sxs-lookup"><span data-stu-id="800bb-135">contact</span></span>](../resources/contact.md) | <span data-ttu-id="800bb-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="800bb-136">Contacts.Read</span></span> | <span data-ttu-id="800bb-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="800bb-137">Contacts.Read</span></span> | <span data-ttu-id="800bb-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="800bb-138">Contacts.Read</span></span> |
|<span data-ttu-id="800bb-139">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="800bb-139">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="800bb-140">不支持</span><span class="sxs-lookup"><span data-stu-id="800bb-140">Not supported</span></span> | <span data-ttu-id="800bb-141">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="800bb-141">Files.ReadWrite</span></span> | <span data-ttu-id="800bb-142">不支持</span><span class="sxs-lookup"><span data-stu-id="800bb-142">Not supported</span></span> |
|<span data-ttu-id="800bb-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="800bb-143">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="800bb-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="800bb-144">Files.ReadWrite.All</span></span> | <span data-ttu-id="800bb-145">不支持</span><span class="sxs-lookup"><span data-stu-id="800bb-145">Not supported</span></span> | <span data-ttu-id="800bb-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="800bb-146">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="800bb-147">事件</span><span class="sxs-lookup"><span data-stu-id="800bb-147">event</span></span>](../resources/event.md) | <span data-ttu-id="800bb-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="800bb-148">Calendars.Read</span></span> | <span data-ttu-id="800bb-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="800bb-149">Calendars.Read</span></span> | <span data-ttu-id="800bb-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="800bb-150">Calendars.Read</span></span> |
|[<span data-ttu-id="800bb-151">组</span><span class="sxs-lookup"><span data-stu-id="800bb-151">group</span></span>](../resources/group.md) | <span data-ttu-id="800bb-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="800bb-152">Group.Read.All</span></span> | <span data-ttu-id="800bb-153">不支持</span><span class="sxs-lookup"><span data-stu-id="800bb-153">Not supported</span></span> | <span data-ttu-id="800bb-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="800bb-154">Group.Read.All</span></span> |
|[<span data-ttu-id="800bb-155">组对话</span><span class="sxs-lookup"><span data-stu-id="800bb-155">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="800bb-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="800bb-156">Group.Read.All</span></span> | <span data-ttu-id="800bb-157">不支持</span><span class="sxs-lookup"><span data-stu-id="800bb-157">Not supported</span></span> | <span data-ttu-id="800bb-158">不支持</span><span class="sxs-lookup"><span data-stu-id="800bb-158">Not supported</span></span> |
|[<span data-ttu-id="800bb-159">列表</span><span class="sxs-lookup"><span data-stu-id="800bb-159">list</span></span>](../resources/list.md) | <span data-ttu-id="800bb-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="800bb-160">Sites.ReadWrite.All</span></span> | <span data-ttu-id="800bb-161">不支持</span><span class="sxs-lookup"><span data-stu-id="800bb-161">Not supported</span></span> | <span data-ttu-id="800bb-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="800bb-162">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="800bb-163">邮件</span><span class="sxs-lookup"><span data-stu-id="800bb-163">message</span></span>](../resources/message.md) | <span data-ttu-id="800bb-164">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="800bb-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="800bb-165">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="800bb-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="800bb-166">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="800bb-166">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="800bb-167">状态</span><span class="sxs-lookup"><span data-stu-id="800bb-167">presence</span></span>](../resources/presence.md) | <span data-ttu-id="800bb-168">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="800bb-168">Presence.Read.All</span></span> | <span data-ttu-id="800bb-169">不支持</span><span class="sxs-lookup"><span data-stu-id="800bb-169">Not supported</span></span> | <span data-ttu-id="800bb-170">不支持</span><span class="sxs-lookup"><span data-stu-id="800bb-170">Not supported</span></span> |
|[<span data-ttu-id="800bb-171">打印机</span><span class="sxs-lookup"><span data-stu-id="800bb-171">printer</span></span>](../resources/printer.md) | <span data-ttu-id="800bb-172">不支持</span><span class="sxs-lookup"><span data-stu-id="800bb-172">Not supported</span></span> | <span data-ttu-id="800bb-173">不支持</span><span class="sxs-lookup"><span data-stu-id="800bb-173">Not supported</span></span> | <span data-ttu-id="800bb-174">Printer.Read.All、Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="800bb-174">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="800bb-175">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="800bb-175">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="800bb-176">不支持</span><span class="sxs-lookup"><span data-stu-id="800bb-176">Not supported</span></span> | <span data-ttu-id="800bb-177">不支持</span><span class="sxs-lookup"><span data-stu-id="800bb-177">Not supported</span></span> | <span data-ttu-id="800bb-178">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="800bb-178">PrintTaskDefinition.ReadWrite.All</span></span> |
|<span data-ttu-id="800bb-179">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="800bb-179">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="800bb-180">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="800bb-180">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="800bb-181">不支持</span><span class="sxs-lookup"><span data-stu-id="800bb-181">Not supported</span></span> | <span data-ttu-id="800bb-182">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="800bb-182">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="800bb-183">todoTask</span><span class="sxs-lookup"><span data-stu-id="800bb-183">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="800bb-184">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="800bb-184">Tasks.ReadWrite</span></span> | <span data-ttu-id="800bb-185">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="800bb-185">Tasks.ReadWrite</span></span> | <span data-ttu-id="800bb-186">不支持</span><span class="sxs-lookup"><span data-stu-id="800bb-186">Not supported</span></span> |
|[<span data-ttu-id="800bb-187">用户</span><span class="sxs-lookup"><span data-stu-id="800bb-187">user</span></span>](../resources/user.md) | <span data-ttu-id="800bb-188">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="800bb-188">User.Read.All</span></span> | <span data-ttu-id="800bb-189">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="800bb-189">User.Read.All</span></span> | <span data-ttu-id="800bb-190">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="800bb-190">User.Read.All</span></span> |

> <span data-ttu-id="800bb-191">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="800bb-191">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [beta-disclaimer](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="800bb-192">driveItem</span><span class="sxs-lookup"><span data-stu-id="800bb-192">driveItem</span></span>

<span data-ttu-id="800bb-193">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="800bb-193">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="800bb-194">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="800bb-194">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="800bb-195">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="800bb-195">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="800bb-196">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="800bb-196">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="800bb-197">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="800bb-197">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="800bb-198">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="800bb-198">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="800bb-199">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="800bb-199">contact, event, and message</span></span>

<span data-ttu-id="800bb-200">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="800bb-200">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="800bb-201">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="800bb-201">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="800bb-202">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="800bb-202">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="800bb-203">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="800bb-203">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="800bb-204">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="800bb-204">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="800bb-205">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="800bb-205">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="800bb-206">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="800bb-206">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="800bb-207">状态</span><span class="sxs-lookup"><span data-stu-id="800bb-207">presence</span></span>

<span data-ttu-id="800bb-208">**状态** 订阅需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="800bb-208">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="800bb-209">如果未指定 [encryptionCertificate](../resources/subscription.md)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="800bb-209">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="800bb-210">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="800bb-210">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="800bb-211">请求标头</span><span class="sxs-lookup"><span data-stu-id="800bb-211">Request headers</span></span>

| <span data-ttu-id="800bb-212">名称</span><span class="sxs-lookup"><span data-stu-id="800bb-212">Name</span></span>       | <span data-ttu-id="800bb-213">类型</span><span class="sxs-lookup"><span data-stu-id="800bb-213">Type</span></span> | <span data-ttu-id="800bb-214">说明</span><span class="sxs-lookup"><span data-stu-id="800bb-214">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="800bb-215">Authorization</span><span class="sxs-lookup"><span data-stu-id="800bb-215">Authorization</span></span>  | <span data-ttu-id="800bb-216">string</span><span class="sxs-lookup"><span data-stu-id="800bb-216">string</span></span>  | <span data-ttu-id="800bb-p108">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="800bb-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="800bb-219">响应</span><span class="sxs-lookup"><span data-stu-id="800bb-219">Response</span></span>

<span data-ttu-id="800bb-220">如果成功，此方法在响应 `201 Created` 正文中返回响应代码[](../resources/subscription.md)和订阅对象。</span><span class="sxs-lookup"><span data-stu-id="800bb-220">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="800bb-221">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="800bb-221">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="800bb-222">示例</span><span class="sxs-lookup"><span data-stu-id="800bb-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="800bb-223">请求</span><span class="sxs-lookup"><span data-stu-id="800bb-223">Request</span></span>

<span data-ttu-id="800bb-224">在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="800bb-224">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="800bb-225">`clientState` 和 `latestSupportedTlsVersion` 是可选字段。</span><span class="sxs-lookup"><span data-stu-id="800bb-225">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="800bb-226">此请求为当前登录用户收到的新邮件更改通知创建订阅。</span><span class="sxs-lookup"><span data-stu-id="800bb-226">This request creates a subscription for change notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="800bb-227">HTTP</span><span class="sxs-lookup"><span data-stu-id="800bb-227">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="800bb-228">C#</span><span class="sxs-lookup"><span data-stu-id="800bb-228">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="800bb-229">JavaScript</span><span class="sxs-lookup"><span data-stu-id="800bb-229">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="800bb-230">Objective-C</span><span class="sxs-lookup"><span data-stu-id="800bb-230">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="800bb-231">Java</span><span class="sxs-lookup"><span data-stu-id="800bb-231">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="800bb-232">在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="800bb-232">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="800bb-233">`clientState` 和 `latestSupportedTlsVersion` 是可选字段。</span><span class="sxs-lookup"><span data-stu-id="800bb-233">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

#### <a name="resources-examples"></a><span data-ttu-id="800bb-234">资源示例</span><span class="sxs-lookup"><span data-stu-id="800bb-234">Resources examples</span></span>

<span data-ttu-id="800bb-235">以下是资源属性的有效值。</span><span class="sxs-lookup"><span data-stu-id="800bb-235">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="800bb-236">资源类型</span><span class="sxs-lookup"><span data-stu-id="800bb-236">Resource type</span></span> | <span data-ttu-id="800bb-237">示例</span><span class="sxs-lookup"><span data-stu-id="800bb-237">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="800bb-238">通话记录</span><span class="sxs-lookup"><span data-stu-id="800bb-238">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="800bb-239">聊天消息</span><span class="sxs-lookup"><span data-stu-id="800bb-239">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="800bb-240">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="800bb-240">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="800bb-241">联系人</span><span class="sxs-lookup"><span data-stu-id="800bb-241">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="800bb-242">对话</span><span class="sxs-lookup"><span data-stu-id="800bb-242">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="800bb-243">驱动器</span><span class="sxs-lookup"><span data-stu-id="800bb-243">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="800bb-244">事件</span><span class="sxs-lookup"><span data-stu-id="800bb-244">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="800bb-245">组</span><span class="sxs-lookup"><span data-stu-id="800bb-245">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="800bb-246">列表</span><span class="sxs-lookup"><span data-stu-id="800bb-246">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="800bb-247">邮件</span><span class="sxs-lookup"><span data-stu-id="800bb-247">Mail</span></span>](../resources/message.md)|<span data-ttu-id="800bb-248">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="800bb-248">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="800bb-249">状态</span><span class="sxs-lookup"><span data-stu-id="800bb-249">Presence</span></span>](../resources/presence.md)| <span data-ttu-id="800bb-250">`/communications/presences/{id}` (单个用户) ， (`/communications/presences?$filter=id in ({id},{id}…)` 多个) </span><span class="sxs-lookup"><span data-stu-id="800bb-250">`/communications/presences/{id}` (single user), `/communications/presences?$filter=id in ({id},{id}…)` (multiple users)</span></span>|
|[<span data-ttu-id="800bb-251">打印机</span><span class="sxs-lookup"><span data-stu-id="800bb-251">printer</span></span>](../resources/printer.md) |`print/printers/{id}/jobs`|
|[<span data-ttu-id="800bb-252">PrintTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="800bb-252">PrintTaskDefinition</span></span>](../resources/printtaskdefinition.md)|`print/taskDefinitions/{id}/tasks`|
|[<span data-ttu-id="800bb-253">用户</span><span class="sxs-lookup"><span data-stu-id="800bb-253">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="800bb-254">todoTask</span><span class="sxs-lookup"><span data-stu-id="800bb-254">todoTask</span></span>](../resources/todotask.md) | `/me/todo/lists/{todoTaskListId}/tasks`
|[<span data-ttu-id="800bb-255">安全警报</span><span class="sxs-lookup"><span data-stu-id="800bb-255">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'NewAlert'`|

> <span data-ttu-id="800bb-256">**注意：** 以 `me` 开头的任何路径也可与 `users/{id}`（而不是 `me`）一起使用，从而以特定用户为目标，而不是以当前用户为目标。</span><span class="sxs-lookup"><span data-stu-id="800bb-256">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

### <a name="response"></a><span data-ttu-id="800bb-257">响应</span><span class="sxs-lookup"><span data-stu-id="800bb-257">Response</span></span>

<span data-ttu-id="800bb-258">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="800bb-258">The following example shows the response.</span></span> 

><span data-ttu-id="800bb-p111">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="800bb-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

### <a name="notification-endpoint-validation"></a><span data-ttu-id="800bb-261">通知终结点验证</span><span class="sxs-lookup"><span data-stu-id="800bb-261">Notification endpoint validation</span></span>

<span data-ttu-id="800bb-262">notificationUrl (中指定的订阅通知终结点) 必须能够响应验证请求，如"设置用户数据更改通知["中所述](/graph/webhooks#notification-endpoint-validation)。</span><span class="sxs-lookup"><span data-stu-id="800bb-262">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="800bb-263">如果验证失败，创建订阅请求返回错误“400 请求无效”。</span><span class="sxs-lookup"><span data-stu-id="800bb-263">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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


