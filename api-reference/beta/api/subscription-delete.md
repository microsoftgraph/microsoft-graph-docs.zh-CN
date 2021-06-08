---
title: 删除订阅
description: 删除订阅。
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 4cc38673566bdff9114e0f94e0a8e27c3d9ad2eb
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787574"
---
# <a name="delete-subscription"></a><span data-ttu-id="8b341-103">删除订阅</span><span class="sxs-lookup"><span data-stu-id="8b341-103">Delete subscription</span></span>

<span data-ttu-id="8b341-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b341-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b341-105">删除订阅。</span><span class="sxs-lookup"><span data-stu-id="8b341-105">Delete a subscription.</span></span>

<span data-ttu-id="8b341-106">请参阅" [权限](#permissions) 部分中的表格，了解支持订阅以更改通知的资源列表。</span><span class="sxs-lookup"><span data-stu-id="8b341-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b341-107">权限</span><span class="sxs-lookup"><span data-stu-id="8b341-107">Permissions</span></span>

<span data-ttu-id="8b341-108">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="8b341-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="8b341-109">若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8b341-109">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b341-110">支持的资源</span><span class="sxs-lookup"><span data-stu-id="8b341-110">Supported resource</span></span> | <span data-ttu-id="8b341-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8b341-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8b341-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8b341-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b341-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="8b341-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="8b341-114">callRecord</span><span class="sxs-lookup"><span data-stu-id="8b341-114">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="8b341-115">不支持</span><span class="sxs-lookup"><span data-stu-id="8b341-115">Not supported</span></span> | <span data-ttu-id="8b341-116">不支持</span><span class="sxs-lookup"><span data-stu-id="8b341-116">Not supported</span></span> | <span data-ttu-id="8b341-117">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b341-117">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="8b341-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="8b341-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="8b341-119">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b341-119">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="8b341-120">不支持</span><span class="sxs-lookup"><span data-stu-id="8b341-120">Not supported</span></span> | <span data-ttu-id="8b341-121">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b341-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="8b341-122">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="8b341-122">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="8b341-123">不支持</span><span class="sxs-lookup"><span data-stu-id="8b341-123">Not supported</span></span> | <span data-ttu-id="8b341-124">不支持</span><span class="sxs-lookup"><span data-stu-id="8b341-124">Not supported</span></span> | <span data-ttu-id="8b341-125">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b341-125">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="8b341-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="8b341-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="8b341-127">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b341-127">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="8b341-128">不支持</span><span class="sxs-lookup"><span data-stu-id="8b341-128">Not supported</span></span> | <span data-ttu-id="8b341-129">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b341-129">Chat.Read.All</span></span>  |
|<span data-ttu-id="8b341-130">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="8b341-130">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="8b341-131">不支持</span><span class="sxs-lookup"><span data-stu-id="8b341-131">Not supported</span></span> | <span data-ttu-id="8b341-132">不支持</span><span class="sxs-lookup"><span data-stu-id="8b341-132">Not supported</span></span> | <span data-ttu-id="8b341-133">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b341-133">Chat.Read.All</span></span>  |
|[<span data-ttu-id="8b341-134">contact</span><span class="sxs-lookup"><span data-stu-id="8b341-134">contact</span></span>](../resources/contact.md) | <span data-ttu-id="8b341-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8b341-135">Contacts.Read</span></span> | <span data-ttu-id="8b341-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8b341-136">Contacts.Read</span></span> | <span data-ttu-id="8b341-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8b341-137">Contacts.Read</span></span> |
|<span data-ttu-id="8b341-138">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="8b341-138">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="8b341-139">不支持</span><span class="sxs-lookup"><span data-stu-id="8b341-139">Not supported</span></span> | <span data-ttu-id="8b341-140">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b341-140">Files.ReadWrite</span></span> | <span data-ttu-id="8b341-141">不支持</span><span class="sxs-lookup"><span data-stu-id="8b341-141">Not supported</span></span> |
|<span data-ttu-id="8b341-142">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="8b341-142">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="8b341-143">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b341-143">Files.ReadWrite.All</span></span> | <span data-ttu-id="8b341-144">不支持</span><span class="sxs-lookup"><span data-stu-id="8b341-144">Not supported</span></span> | <span data-ttu-id="8b341-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b341-145">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="8b341-146">事件</span><span class="sxs-lookup"><span data-stu-id="8b341-146">event</span></span>](../resources/event.md) | <span data-ttu-id="8b341-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8b341-147">Calendars.Read</span></span> | <span data-ttu-id="8b341-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8b341-148">Calendars.Read</span></span> | <span data-ttu-id="8b341-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8b341-149">Calendars.Read</span></span> |
|[<span data-ttu-id="8b341-150">组</span><span class="sxs-lookup"><span data-stu-id="8b341-150">group</span></span>](../resources/group.md) | <span data-ttu-id="8b341-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b341-151">Group.Read.All</span></span> | <span data-ttu-id="8b341-152">不支持</span><span class="sxs-lookup"><span data-stu-id="8b341-152">Not supported</span></span> | <span data-ttu-id="8b341-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b341-153">Group.Read.All</span></span> |
|[<span data-ttu-id="8b341-154">组对话</span><span class="sxs-lookup"><span data-stu-id="8b341-154">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="8b341-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b341-155">Group.Read.All</span></span> | <span data-ttu-id="8b341-156">不支持</span><span class="sxs-lookup"><span data-stu-id="8b341-156">Not supported</span></span> | <span data-ttu-id="8b341-157">不支持</span><span class="sxs-lookup"><span data-stu-id="8b341-157">Not supported</span></span> |
|[<span data-ttu-id="8b341-158">列表</span><span class="sxs-lookup"><span data-stu-id="8b341-158">list</span></span>](../resources/list.md) | <span data-ttu-id="8b341-159">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b341-159">Sites.ReadWrite.All</span></span> | <span data-ttu-id="8b341-160">不支持</span><span class="sxs-lookup"><span data-stu-id="8b341-160">Not supported</span></span> | <span data-ttu-id="8b341-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b341-161">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="8b341-162">邮件</span><span class="sxs-lookup"><span data-stu-id="8b341-162">message</span></span>](../resources/message.md) | <span data-ttu-id="8b341-163">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8b341-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="8b341-164">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8b341-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="8b341-165">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8b341-165">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="8b341-166">状态</span><span class="sxs-lookup"><span data-stu-id="8b341-166">presence</span></span>](../resources/presence.md) | <span data-ttu-id="8b341-167">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b341-167">Presence.Read.All</span></span> | <span data-ttu-id="8b341-168">不支持</span><span class="sxs-lookup"><span data-stu-id="8b341-168">Not supported</span></span> | <span data-ttu-id="8b341-169">不支持</span><span class="sxs-lookup"><span data-stu-id="8b341-169">Not supported</span></span> |
|[<span data-ttu-id="8b341-170">打印机</span><span class="sxs-lookup"><span data-stu-id="8b341-170">printer</span></span>](../resources/printer.md) | <span data-ttu-id="8b341-171">不支持</span><span class="sxs-lookup"><span data-stu-id="8b341-171">Not supported</span></span> | <span data-ttu-id="8b341-172">不支持</span><span class="sxs-lookup"><span data-stu-id="8b341-172">Not supported</span></span> | <span data-ttu-id="8b341-173">打印机。阅读.All，Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b341-173">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="8b341-174">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="8b341-174">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="8b341-175">不支持</span><span class="sxs-lookup"><span data-stu-id="8b341-175">Not supported</span></span> | <span data-ttu-id="8b341-176">不支持</span><span class="sxs-lookup"><span data-stu-id="8b341-176">Not supported</span></span> | <span data-ttu-id="8b341-177">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b341-177">PrintTaskDefinition.ReadWrite.All</span></span> |
|<span data-ttu-id="8b341-178">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="8b341-178">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="8b341-179">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b341-179">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="8b341-180">不支持</span><span class="sxs-lookup"><span data-stu-id="8b341-180">Not supported</span></span> | <span data-ttu-id="8b341-181">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b341-181">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="8b341-182">todoTask</span><span class="sxs-lookup"><span data-stu-id="8b341-182">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="8b341-183">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b341-183">Tasks.ReadWrite</span></span> | <span data-ttu-id="8b341-184">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b341-184">Tasks.ReadWrite</span></span> | <span data-ttu-id="8b341-185">不支持</span><span class="sxs-lookup"><span data-stu-id="8b341-185">Not supported</span></span> |
|[<span data-ttu-id="8b341-186">用户</span><span class="sxs-lookup"><span data-stu-id="8b341-186">user</span></span>](../resources/user.md) | <span data-ttu-id="8b341-187">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b341-187">User.Read.All</span></span> | <span data-ttu-id="8b341-188">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b341-188">User.Read.All</span></span> | <span data-ttu-id="8b341-189">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b341-189">User.Read.All</span></span> |

> <span data-ttu-id="8b341-190">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="8b341-190">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="8b341-191">driveItem</span><span class="sxs-lookup"><span data-stu-id="8b341-191">driveItem</span></span>

<span data-ttu-id="8b341-192">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="8b341-192">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="8b341-193">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="8b341-193">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="8b341-194">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="8b341-194">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="8b341-195">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="8b341-195">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="8b341-196">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="8b341-196">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="8b341-197">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="8b341-197">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="8b341-198">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="8b341-198">contact, event, and message</span></span>

<span data-ttu-id="8b341-199">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="8b341-199">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="8b341-200">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="8b341-200">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="8b341-201">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="8b341-201">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="8b341-202">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="8b341-202">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="8b341-203">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="8b341-203">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="8b341-204">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="8b341-204">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="8b341-205">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="8b341-205">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="8b341-206">状态</span><span class="sxs-lookup"><span data-stu-id="8b341-206">presence</span></span>

<span data-ttu-id="8b341-207">**状态** 订阅需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="8b341-207">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="8b341-208">如果未指定 [encryptionCertificate](../resources/subscription.md)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="8b341-208">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="8b341-209">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8b341-209">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="8b341-210">请求标头</span><span class="sxs-lookup"><span data-stu-id="8b341-210">Request headers</span></span>

| <span data-ttu-id="8b341-211">名称</span><span class="sxs-lookup"><span data-stu-id="8b341-211">Name</span></span>       | <span data-ttu-id="8b341-212">类型</span><span class="sxs-lookup"><span data-stu-id="8b341-212">Type</span></span> | <span data-ttu-id="8b341-213">说明</span><span class="sxs-lookup"><span data-stu-id="8b341-213">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8b341-214">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b341-214">Authorization</span></span>  | <span data-ttu-id="8b341-215">string</span><span class="sxs-lookup"><span data-stu-id="8b341-215">string</span></span>  | <span data-ttu-id="8b341-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8b341-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b341-218">请求正文</span><span class="sxs-lookup"><span data-stu-id="8b341-218">Request body</span></span>

<span data-ttu-id="8b341-219">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8b341-219">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b341-220">响应</span><span class="sxs-lookup"><span data-stu-id="8b341-220">Response</span></span>

<span data-ttu-id="8b341-221">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8b341-221">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="8b341-222">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="8b341-222">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="8b341-223">示例</span><span class="sxs-lookup"><span data-stu-id="8b341-223">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8b341-224">请求</span><span class="sxs-lookup"><span data-stu-id="8b341-224">Request</span></span>

<span data-ttu-id="8b341-225">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8b341-225">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8b341-226">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b341-226">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="8b341-227">C#</span><span class="sxs-lookup"><span data-stu-id="8b341-227">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b341-228">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b341-228">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b341-229">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b341-229">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b341-230">Java</span><span class="sxs-lookup"><span data-stu-id="8b341-230">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8b341-231">响应</span><span class="sxs-lookup"><span data-stu-id="8b341-231">Response</span></span>

<span data-ttu-id="8b341-232">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8b341-232">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response"
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


