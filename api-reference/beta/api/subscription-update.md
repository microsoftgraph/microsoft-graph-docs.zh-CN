---
title: 更新订阅
description: 通过延长到期时间续订订阅。
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 855c0463c75bd57e49b2de990a8de69965c34b48
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034263"
---
# <a name="update-subscription"></a><span data-ttu-id="4332a-103">更新订阅</span><span class="sxs-lookup"><span data-stu-id="4332a-103">Update subscription</span></span>

<span data-ttu-id="4332a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4332a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4332a-105">通过延长到期时间续订订阅。</span><span class="sxs-lookup"><span data-stu-id="4332a-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="4332a-106">订阅在一段时间后过期，该时间长度因资源类型而异。</span><span class="sxs-lookup"><span data-stu-id="4332a-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="4332a-107">为了避免缺少更改通知，应用应在到期日期之前很好地续订其订阅。</span><span class="sxs-lookup"><span data-stu-id="4332a-107">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="4332a-108">请参阅 [订阅](../resources/subscription.md) ，了解每种资源类型的订阅的最大长度。</span><span class="sxs-lookup"><span data-stu-id="4332a-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="4332a-109">权限</span><span class="sxs-lookup"><span data-stu-id="4332a-109">Permissions</span></span>

<span data-ttu-id="4332a-110">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="4332a-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="4332a-111">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4332a-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4332a-112">支持的资源</span><span class="sxs-lookup"><span data-stu-id="4332a-112">Supported resource</span></span> | <span data-ttu-id="4332a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4332a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4332a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4332a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4332a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4332a-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="4332a-116">callRecord</span><span class="sxs-lookup"><span data-stu-id="4332a-116">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="4332a-117">不支持</span><span class="sxs-lookup"><span data-stu-id="4332a-117">Not supported</span></span> | <span data-ttu-id="4332a-118">不支持</span><span class="sxs-lookup"><span data-stu-id="4332a-118">Not supported</span></span> | <span data-ttu-id="4332a-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="4332a-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="4332a-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="4332a-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="4332a-121">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4332a-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="4332a-122">不支持</span><span class="sxs-lookup"><span data-stu-id="4332a-122">Not supported</span></span> | <span data-ttu-id="4332a-123">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="4332a-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="4332a-124">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="4332a-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="4332a-125">不支持</span><span class="sxs-lookup"><span data-stu-id="4332a-125">Not supported</span></span> | <span data-ttu-id="4332a-126">不支持</span><span class="sxs-lookup"><span data-stu-id="4332a-126">Not supported</span></span> | <span data-ttu-id="4332a-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="4332a-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="4332a-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="4332a-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="4332a-129">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4332a-129">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="4332a-130">不支持</span><span class="sxs-lookup"><span data-stu-id="4332a-130">Not supported</span></span> | <span data-ttu-id="4332a-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="4332a-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="4332a-132">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="4332a-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="4332a-133">不支持</span><span class="sxs-lookup"><span data-stu-id="4332a-133">Not supported</span></span> | <span data-ttu-id="4332a-134">不支持</span><span class="sxs-lookup"><span data-stu-id="4332a-134">Not supported</span></span> | <span data-ttu-id="4332a-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="4332a-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="4332a-136">contact</span><span class="sxs-lookup"><span data-stu-id="4332a-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="4332a-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4332a-137">Contacts.Read</span></span> | <span data-ttu-id="4332a-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4332a-138">Contacts.Read</span></span> | <span data-ttu-id="4332a-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4332a-139">Contacts.Read</span></span> |
|<span data-ttu-id="4332a-140">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="4332a-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="4332a-141">不支持</span><span class="sxs-lookup"><span data-stu-id="4332a-141">Not supported</span></span> | <span data-ttu-id="4332a-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4332a-142">Files.ReadWrite</span></span> | <span data-ttu-id="4332a-143">不支持</span><span class="sxs-lookup"><span data-stu-id="4332a-143">Not supported</span></span> |
|<span data-ttu-id="4332a-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="4332a-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="4332a-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4332a-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="4332a-146">不支持</span><span class="sxs-lookup"><span data-stu-id="4332a-146">Not supported</span></span> | <span data-ttu-id="4332a-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4332a-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="4332a-148">事件</span><span class="sxs-lookup"><span data-stu-id="4332a-148">event</span></span>](../resources/event.md) | <span data-ttu-id="4332a-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4332a-149">Calendars.Read</span></span> | <span data-ttu-id="4332a-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4332a-150">Calendars.Read</span></span> | <span data-ttu-id="4332a-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4332a-151">Calendars.Read</span></span> |
|[<span data-ttu-id="4332a-152">组</span><span class="sxs-lookup"><span data-stu-id="4332a-152">group</span></span>](../resources/group.md) | <span data-ttu-id="4332a-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4332a-153">Group.Read.All</span></span> | <span data-ttu-id="4332a-154">不支持</span><span class="sxs-lookup"><span data-stu-id="4332a-154">Not supported</span></span> | <span data-ttu-id="4332a-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4332a-155">Group.Read.All</span></span> |
|[<span data-ttu-id="4332a-156">组对话</span><span class="sxs-lookup"><span data-stu-id="4332a-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="4332a-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4332a-157">Group.Read.All</span></span> | <span data-ttu-id="4332a-158">不支持</span><span class="sxs-lookup"><span data-stu-id="4332a-158">Not supported</span></span> | <span data-ttu-id="4332a-159">不支持</span><span class="sxs-lookup"><span data-stu-id="4332a-159">Not supported</span></span> |
|[<span data-ttu-id="4332a-160">列表</span><span class="sxs-lookup"><span data-stu-id="4332a-160">list</span></span>](../resources/list.md) | <span data-ttu-id="4332a-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4332a-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="4332a-162">不支持</span><span class="sxs-lookup"><span data-stu-id="4332a-162">Not supported</span></span> | <span data-ttu-id="4332a-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4332a-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="4332a-164">邮件</span><span class="sxs-lookup"><span data-stu-id="4332a-164">message</span></span>](../resources/message.md) | <span data-ttu-id="4332a-165">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4332a-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="4332a-166">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4332a-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="4332a-167">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4332a-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="4332a-168">状态</span><span class="sxs-lookup"><span data-stu-id="4332a-168">presence</span></span>](../resources/presence.md) | <span data-ttu-id="4332a-169">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="4332a-169">Presence.Read.All</span></span> | <span data-ttu-id="4332a-170">不支持</span><span class="sxs-lookup"><span data-stu-id="4332a-170">Not supported</span></span> | <span data-ttu-id="4332a-171">不支持</span><span class="sxs-lookup"><span data-stu-id="4332a-171">Not supported</span></span> |
|[<span data-ttu-id="4332a-172">打印机</span><span class="sxs-lookup"><span data-stu-id="4332a-172">printer</span></span>](../resources/printer.md) | <span data-ttu-id="4332a-173">不支持</span><span class="sxs-lookup"><span data-stu-id="4332a-173">Not supported</span></span> | <span data-ttu-id="4332a-174">不支持</span><span class="sxs-lookup"><span data-stu-id="4332a-174">Not supported</span></span> | <span data-ttu-id="4332a-175">Printer.Read.All、Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4332a-175">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="4332a-176">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="4332a-176">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="4332a-177">不支持</span><span class="sxs-lookup"><span data-stu-id="4332a-177">Not supported</span></span> | <span data-ttu-id="4332a-178">不支持</span><span class="sxs-lookup"><span data-stu-id="4332a-178">Not supported</span></span> | <span data-ttu-id="4332a-179">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4332a-179">PrintTaskDefinition.ReadWrite.All</span></span> |
|<span data-ttu-id="4332a-180">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="4332a-180">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="4332a-181">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4332a-181">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="4332a-182">不支持</span><span class="sxs-lookup"><span data-stu-id="4332a-182">Not supported</span></span> | <span data-ttu-id="4332a-183">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4332a-183">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="4332a-184">todoTask</span><span class="sxs-lookup"><span data-stu-id="4332a-184">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="4332a-185">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4332a-185">Tasks.ReadWrite</span></span> | <span data-ttu-id="4332a-186">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4332a-186">Tasks.ReadWrite</span></span> | <span data-ttu-id="4332a-187">不支持</span><span class="sxs-lookup"><span data-stu-id="4332a-187">Not supported</span></span> |
|[<span data-ttu-id="4332a-188">用户</span><span class="sxs-lookup"><span data-stu-id="4332a-188">user</span></span>](../resources/user.md) | <span data-ttu-id="4332a-189">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4332a-189">User.Read.All</span></span> | <span data-ttu-id="4332a-190">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4332a-190">User.Read.All</span></span> | <span data-ttu-id="4332a-191">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4332a-191">User.Read.All</span></span> |

> <span data-ttu-id="4332a-192">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="4332a-192">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [beta-disclaimer](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="4332a-193">driveItem</span><span class="sxs-lookup"><span data-stu-id="4332a-193">driveItem</span></span>

<span data-ttu-id="4332a-194">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="4332a-194">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="4332a-195">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="4332a-195">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="4332a-196">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="4332a-196">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="4332a-197">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="4332a-197">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="4332a-198">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="4332a-198">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="4332a-199">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="4332a-199">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="4332a-200">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="4332a-200">contact, event, and message</span></span>

<span data-ttu-id="4332a-201">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="4332a-201">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="4332a-202">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="4332a-202">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="4332a-203">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="4332a-203">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="4332a-204">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="4332a-204">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="4332a-205">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="4332a-205">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="4332a-206">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="4332a-206">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="4332a-207">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="4332a-207">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="4332a-208">状态</span><span class="sxs-lookup"><span data-stu-id="4332a-208">presence</span></span>

<span data-ttu-id="4332a-209">**状态** 订阅需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="4332a-209">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="4332a-210">如果未指定 [encryptionCertificate](../resources/subscription.md)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="4332a-210">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="4332a-211">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4332a-211">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4332a-212">请求标头</span><span class="sxs-lookup"><span data-stu-id="4332a-212">Request headers</span></span>

| <span data-ttu-id="4332a-213">名称</span><span class="sxs-lookup"><span data-stu-id="4332a-213">Name</span></span>       | <span data-ttu-id="4332a-214">类型</span><span class="sxs-lookup"><span data-stu-id="4332a-214">Type</span></span> | <span data-ttu-id="4332a-215">说明</span><span class="sxs-lookup"><span data-stu-id="4332a-215">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4332a-216">Authorization</span><span class="sxs-lookup"><span data-stu-id="4332a-216">Authorization</span></span>  | <span data-ttu-id="4332a-217">string</span><span class="sxs-lookup"><span data-stu-id="4332a-217">string</span></span>  | <span data-ttu-id="4332a-p108">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4332a-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4332a-220">响应</span><span class="sxs-lookup"><span data-stu-id="4332a-220">Response</span></span>

<span data-ttu-id="4332a-221">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4332a-221">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="4332a-222">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="4332a-222">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="4332a-223">示例</span><span class="sxs-lookup"><span data-stu-id="4332a-223">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4332a-224">请求</span><span class="sxs-lookup"><span data-stu-id="4332a-224">Request</span></span>

<span data-ttu-id="4332a-225">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4332a-225">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4332a-226">HTTP</span><span class="sxs-lookup"><span data-stu-id="4332a-226">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4332a-227">C#</span><span class="sxs-lookup"><span data-stu-id="4332a-227">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4332a-228">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4332a-228">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4332a-229">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4332a-229">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4332a-230">Java</span><span class="sxs-lookup"><span data-stu-id="4332a-230">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4332a-231">响应</span><span class="sxs-lookup"><span data-stu-id="4332a-231">Response</span></span>

<span data-ttu-id="4332a-232">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4332a-232">Here is an example of the response.</span></span>
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
  "lifecycleNotificationUrl":"https://webhook.azurewebsites.net/api/send/lifecycleNotifications",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2",
  "encryptionCertificate": "",
  "encryptionCertificateId": "",
  "includeResourceData": false
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


