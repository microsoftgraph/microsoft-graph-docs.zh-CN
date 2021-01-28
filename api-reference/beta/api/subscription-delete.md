---
title: 删除订阅
description: 删除订阅。
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b38975627a0a3c23b9e19acbb235c4bc26036918
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034259"
---
# <a name="delete-subscription"></a><span data-ttu-id="1d7c5-103">删除订阅</span><span class="sxs-lookup"><span data-stu-id="1d7c5-103">Delete subscription</span></span>

<span data-ttu-id="1d7c5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d7c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d7c5-105">删除订阅。</span><span class="sxs-lookup"><span data-stu-id="1d7c5-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d7c5-106">权限</span><span class="sxs-lookup"><span data-stu-id="1d7c5-106">Permissions</span></span>

<span data-ttu-id="1d7c5-107">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="1d7c5-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="1d7c5-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1d7c5-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1d7c5-109">支持的资源</span><span class="sxs-lookup"><span data-stu-id="1d7c5-109">Supported resource</span></span> | <span data-ttu-id="1d7c5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1d7c5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1d7c5-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1d7c5-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d7c5-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="1d7c5-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="1d7c5-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="1d7c5-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="1d7c5-114">不支持</span><span class="sxs-lookup"><span data-stu-id="1d7c5-114">Not supported</span></span> | <span data-ttu-id="1d7c5-115">不支持</span><span class="sxs-lookup"><span data-stu-id="1d7c5-115">Not supported</span></span> | <span data-ttu-id="1d7c5-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d7c5-116">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="1d7c5-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="1d7c5-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="1d7c5-118">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d7c5-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="1d7c5-119">不支持</span><span class="sxs-lookup"><span data-stu-id="1d7c5-119">Not supported</span></span> | <span data-ttu-id="1d7c5-120">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d7c5-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="1d7c5-121">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="1d7c5-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="1d7c5-122">不支持</span><span class="sxs-lookup"><span data-stu-id="1d7c5-122">Not supported</span></span> | <span data-ttu-id="1d7c5-123">不支持</span><span class="sxs-lookup"><span data-stu-id="1d7c5-123">Not supported</span></span> | <span data-ttu-id="1d7c5-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d7c5-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="1d7c5-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="1d7c5-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="1d7c5-126">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d7c5-126">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="1d7c5-127">不支持</span><span class="sxs-lookup"><span data-stu-id="1d7c5-127">Not supported</span></span> | <span data-ttu-id="1d7c5-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d7c5-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="1d7c5-129">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="1d7c5-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="1d7c5-130">不支持</span><span class="sxs-lookup"><span data-stu-id="1d7c5-130">Not supported</span></span> | <span data-ttu-id="1d7c5-131">不支持</span><span class="sxs-lookup"><span data-stu-id="1d7c5-131">Not supported</span></span> | <span data-ttu-id="1d7c5-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d7c5-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="1d7c5-133">contact</span><span class="sxs-lookup"><span data-stu-id="1d7c5-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="1d7c5-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1d7c5-134">Contacts.Read</span></span> | <span data-ttu-id="1d7c5-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1d7c5-135">Contacts.Read</span></span> | <span data-ttu-id="1d7c5-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1d7c5-136">Contacts.Read</span></span> |
|<span data-ttu-id="1d7c5-137">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="1d7c5-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="1d7c5-138">不支持</span><span class="sxs-lookup"><span data-stu-id="1d7c5-138">Not supported</span></span> | <span data-ttu-id="1d7c5-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d7c5-139">Files.ReadWrite</span></span> | <span data-ttu-id="1d7c5-140">不支持</span><span class="sxs-lookup"><span data-stu-id="1d7c5-140">Not supported</span></span> |
|<span data-ttu-id="1d7c5-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="1d7c5-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="1d7c5-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d7c5-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="1d7c5-143">不支持</span><span class="sxs-lookup"><span data-stu-id="1d7c5-143">Not supported</span></span> | <span data-ttu-id="1d7c5-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d7c5-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="1d7c5-145">事件</span><span class="sxs-lookup"><span data-stu-id="1d7c5-145">event</span></span>](../resources/event.md) | <span data-ttu-id="1d7c5-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1d7c5-146">Calendars.Read</span></span> | <span data-ttu-id="1d7c5-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1d7c5-147">Calendars.Read</span></span> | <span data-ttu-id="1d7c5-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1d7c5-148">Calendars.Read</span></span> |
|[<span data-ttu-id="1d7c5-149">组</span><span class="sxs-lookup"><span data-stu-id="1d7c5-149">group</span></span>](../resources/group.md) | <span data-ttu-id="1d7c5-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d7c5-150">Group.Read.All</span></span> | <span data-ttu-id="1d7c5-151">不支持</span><span class="sxs-lookup"><span data-stu-id="1d7c5-151">Not supported</span></span> | <span data-ttu-id="1d7c5-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d7c5-152">Group.Read.All</span></span> |
|[<span data-ttu-id="1d7c5-153">组对话</span><span class="sxs-lookup"><span data-stu-id="1d7c5-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="1d7c5-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d7c5-154">Group.Read.All</span></span> | <span data-ttu-id="1d7c5-155">不支持</span><span class="sxs-lookup"><span data-stu-id="1d7c5-155">Not supported</span></span> | <span data-ttu-id="1d7c5-156">不支持</span><span class="sxs-lookup"><span data-stu-id="1d7c5-156">Not supported</span></span> |
|[<span data-ttu-id="1d7c5-157">列表</span><span class="sxs-lookup"><span data-stu-id="1d7c5-157">list</span></span>](../resources/list.md) | <span data-ttu-id="1d7c5-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d7c5-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="1d7c5-159">不支持</span><span class="sxs-lookup"><span data-stu-id="1d7c5-159">Not supported</span></span> | <span data-ttu-id="1d7c5-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d7c5-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="1d7c5-161">邮件</span><span class="sxs-lookup"><span data-stu-id="1d7c5-161">message</span></span>](../resources/message.md) | <span data-ttu-id="1d7c5-162">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1d7c5-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="1d7c5-163">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1d7c5-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="1d7c5-164">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1d7c5-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="1d7c5-165">状态</span><span class="sxs-lookup"><span data-stu-id="1d7c5-165">presence</span></span>](../resources/presence.md) | <span data-ttu-id="1d7c5-166">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d7c5-166">Presence.Read.All</span></span> | <span data-ttu-id="1d7c5-167">不支持</span><span class="sxs-lookup"><span data-stu-id="1d7c5-167">Not supported</span></span> | <span data-ttu-id="1d7c5-168">不支持</span><span class="sxs-lookup"><span data-stu-id="1d7c5-168">Not supported</span></span> |
|[<span data-ttu-id="1d7c5-169">打印机</span><span class="sxs-lookup"><span data-stu-id="1d7c5-169">printer</span></span>](../resources/printer.md) | <span data-ttu-id="1d7c5-170">不支持</span><span class="sxs-lookup"><span data-stu-id="1d7c5-170">Not supported</span></span> | <span data-ttu-id="1d7c5-171">不支持</span><span class="sxs-lookup"><span data-stu-id="1d7c5-171">Not supported</span></span> | <span data-ttu-id="1d7c5-172">Printer.Read.All、Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d7c5-172">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="1d7c5-173">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="1d7c5-173">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="1d7c5-174">不支持</span><span class="sxs-lookup"><span data-stu-id="1d7c5-174">Not supported</span></span> | <span data-ttu-id="1d7c5-175">不支持</span><span class="sxs-lookup"><span data-stu-id="1d7c5-175">Not supported</span></span> | <span data-ttu-id="1d7c5-176">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d7c5-176">PrintTaskDefinition.ReadWrite.All</span></span> |
|<span data-ttu-id="1d7c5-177">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="1d7c5-177">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="1d7c5-178">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d7c5-178">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="1d7c5-179">不支持</span><span class="sxs-lookup"><span data-stu-id="1d7c5-179">Not supported</span></span> | <span data-ttu-id="1d7c5-180">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d7c5-180">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="1d7c5-181">todoTask</span><span class="sxs-lookup"><span data-stu-id="1d7c5-181">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="1d7c5-182">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d7c5-182">Tasks.ReadWrite</span></span> | <span data-ttu-id="1d7c5-183">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d7c5-183">Tasks.ReadWrite</span></span> | <span data-ttu-id="1d7c5-184">不支持</span><span class="sxs-lookup"><span data-stu-id="1d7c5-184">Not supported</span></span> |
|[<span data-ttu-id="1d7c5-185">用户</span><span class="sxs-lookup"><span data-stu-id="1d7c5-185">user</span></span>](../resources/user.md) | <span data-ttu-id="1d7c5-186">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d7c5-186">User.Read.All</span></span> | <span data-ttu-id="1d7c5-187">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d7c5-187">User.Read.All</span></span> | <span data-ttu-id="1d7c5-188">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d7c5-188">User.Read.All</span></span> |

> <span data-ttu-id="1d7c5-189">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="1d7c5-189">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [beta-disclaimer](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="1d7c5-190">driveItem</span><span class="sxs-lookup"><span data-stu-id="1d7c5-190">driveItem</span></span>

<span data-ttu-id="1d7c5-191">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="1d7c5-191">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="1d7c5-192">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="1d7c5-192">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="1d7c5-193">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="1d7c5-193">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="1d7c5-194">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="1d7c5-194">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="1d7c5-195">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="1d7c5-195">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="1d7c5-196">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="1d7c5-196">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="1d7c5-197">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="1d7c5-197">contact, event, and message</span></span>

<span data-ttu-id="1d7c5-198">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="1d7c5-198">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="1d7c5-199">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="1d7c5-199">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="1d7c5-200">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="1d7c5-200">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="1d7c5-201">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="1d7c5-201">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="1d7c5-202">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="1d7c5-202">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="1d7c5-203">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="1d7c5-203">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="1d7c5-204">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="1d7c5-204">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="1d7c5-205">状态</span><span class="sxs-lookup"><span data-stu-id="1d7c5-205">presence</span></span>

<span data-ttu-id="1d7c5-206">**状态** 订阅需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="1d7c5-206">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="1d7c5-207">如果未指定 [encryptionCertificate](../resources/subscription.md)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="1d7c5-207">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="1d7c5-208">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1d7c5-208">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="1d7c5-209">请求标头</span><span class="sxs-lookup"><span data-stu-id="1d7c5-209">Request headers</span></span>

| <span data-ttu-id="1d7c5-210">名称</span><span class="sxs-lookup"><span data-stu-id="1d7c5-210">Name</span></span>       | <span data-ttu-id="1d7c5-211">类型</span><span class="sxs-lookup"><span data-stu-id="1d7c5-211">Type</span></span> | <span data-ttu-id="1d7c5-212">说明</span><span class="sxs-lookup"><span data-stu-id="1d7c5-212">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1d7c5-213">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d7c5-213">Authorization</span></span>  | <span data-ttu-id="1d7c5-214">string</span><span class="sxs-lookup"><span data-stu-id="1d7c5-214">string</span></span>  | <span data-ttu-id="1d7c5-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1d7c5-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d7c5-217">请求正文</span><span class="sxs-lookup"><span data-stu-id="1d7c5-217">Request body</span></span>

<span data-ttu-id="1d7c5-218">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1d7c5-218">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d7c5-219">响应</span><span class="sxs-lookup"><span data-stu-id="1d7c5-219">Response</span></span>

<span data-ttu-id="1d7c5-220">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1d7c5-220">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="1d7c5-221">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="1d7c5-221">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="1d7c5-222">示例</span><span class="sxs-lookup"><span data-stu-id="1d7c5-222">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1d7c5-223">请求</span><span class="sxs-lookup"><span data-stu-id="1d7c5-223">Request</span></span>

<span data-ttu-id="1d7c5-224">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1d7c5-224">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1d7c5-225">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d7c5-225">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="1d7c5-226">C#</span><span class="sxs-lookup"><span data-stu-id="1d7c5-226">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d7c5-227">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d7c5-227">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d7c5-228">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d7c5-228">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1d7c5-229">Java</span><span class="sxs-lookup"><span data-stu-id="1d7c5-229">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1d7c5-230">响应</span><span class="sxs-lookup"><span data-stu-id="1d7c5-230">Response</span></span>

<span data-ttu-id="1d7c5-231">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1d7c5-231">Here is an example of the response.</span></span>
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


