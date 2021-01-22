---
title: 删除订阅
description: 删除订阅。
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5518091d21a3ed2e1c05a8bc95c70b62d7cb82eb
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934833"
---
# <a name="delete-subscription"></a><span data-ttu-id="84ca1-103">删除订阅</span><span class="sxs-lookup"><span data-stu-id="84ca1-103">Delete subscription</span></span>

<span data-ttu-id="84ca1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84ca1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84ca1-105">删除订阅。</span><span class="sxs-lookup"><span data-stu-id="84ca1-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="84ca1-106">权限</span><span class="sxs-lookup"><span data-stu-id="84ca1-106">Permissions</span></span>

<span data-ttu-id="84ca1-107">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="84ca1-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="84ca1-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84ca1-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="84ca1-109">支持的资源</span><span class="sxs-lookup"><span data-stu-id="84ca1-109">Supported resource</span></span> | <span data-ttu-id="84ca1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84ca1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="84ca1-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84ca1-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84ca1-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="84ca1-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="84ca1-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="84ca1-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="84ca1-114">不支持</span><span class="sxs-lookup"><span data-stu-id="84ca1-114">Not supported</span></span> | <span data-ttu-id="84ca1-115">不支持</span><span class="sxs-lookup"><span data-stu-id="84ca1-115">Not supported</span></span> | <span data-ttu-id="84ca1-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="84ca1-116">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="84ca1-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="84ca1-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="84ca1-118">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84ca1-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="84ca1-119">不支持</span><span class="sxs-lookup"><span data-stu-id="84ca1-119">Not supported</span></span> | <span data-ttu-id="84ca1-120">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="84ca1-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="84ca1-121">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="84ca1-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="84ca1-122">不支持</span><span class="sxs-lookup"><span data-stu-id="84ca1-122">Not supported</span></span> | <span data-ttu-id="84ca1-123">不支持</span><span class="sxs-lookup"><span data-stu-id="84ca1-123">Not supported</span></span> | <span data-ttu-id="84ca1-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="84ca1-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="84ca1-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="84ca1-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="84ca1-126">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84ca1-126">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="84ca1-127">不支持</span><span class="sxs-lookup"><span data-stu-id="84ca1-127">Not supported</span></span> | <span data-ttu-id="84ca1-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="84ca1-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="84ca1-129">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="84ca1-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="84ca1-130">不支持</span><span class="sxs-lookup"><span data-stu-id="84ca1-130">Not supported</span></span> | <span data-ttu-id="84ca1-131">不支持</span><span class="sxs-lookup"><span data-stu-id="84ca1-131">Not supported</span></span> | <span data-ttu-id="84ca1-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="84ca1-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="84ca1-133">contact</span><span class="sxs-lookup"><span data-stu-id="84ca1-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="84ca1-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="84ca1-134">Contacts.Read</span></span> | <span data-ttu-id="84ca1-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="84ca1-135">Contacts.Read</span></span> | <span data-ttu-id="84ca1-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="84ca1-136">Contacts.Read</span></span> |
|<span data-ttu-id="84ca1-137">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="84ca1-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="84ca1-138">不支持</span><span class="sxs-lookup"><span data-stu-id="84ca1-138">Not supported</span></span> | <span data-ttu-id="84ca1-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84ca1-139">Files.ReadWrite</span></span> | <span data-ttu-id="84ca1-140">不支持</span><span class="sxs-lookup"><span data-stu-id="84ca1-140">Not supported</span></span> |
|<span data-ttu-id="84ca1-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="84ca1-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="84ca1-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84ca1-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="84ca1-143">不支持</span><span class="sxs-lookup"><span data-stu-id="84ca1-143">Not supported</span></span> | <span data-ttu-id="84ca1-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84ca1-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="84ca1-145">事件</span><span class="sxs-lookup"><span data-stu-id="84ca1-145">event</span></span>](../resources/event.md) | <span data-ttu-id="84ca1-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="84ca1-146">Calendars.Read</span></span> | <span data-ttu-id="84ca1-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="84ca1-147">Calendars.Read</span></span> | <span data-ttu-id="84ca1-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="84ca1-148">Calendars.Read</span></span> |
|[<span data-ttu-id="84ca1-149">组</span><span class="sxs-lookup"><span data-stu-id="84ca1-149">group</span></span>](../resources/group.md) | <span data-ttu-id="84ca1-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="84ca1-150">Group.Read.All</span></span> | <span data-ttu-id="84ca1-151">不支持</span><span class="sxs-lookup"><span data-stu-id="84ca1-151">Not supported</span></span> | <span data-ttu-id="84ca1-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="84ca1-152">Group.Read.All</span></span> |
|[<span data-ttu-id="84ca1-153">组对话</span><span class="sxs-lookup"><span data-stu-id="84ca1-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="84ca1-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="84ca1-154">Group.Read.All</span></span> | <span data-ttu-id="84ca1-155">不支持</span><span class="sxs-lookup"><span data-stu-id="84ca1-155">Not supported</span></span> | <span data-ttu-id="84ca1-156">不支持</span><span class="sxs-lookup"><span data-stu-id="84ca1-156">Not supported</span></span> |
|[<span data-ttu-id="84ca1-157">列表</span><span class="sxs-lookup"><span data-stu-id="84ca1-157">list</span></span>](../resources/list.md) | <span data-ttu-id="84ca1-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84ca1-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="84ca1-159">不支持</span><span class="sxs-lookup"><span data-stu-id="84ca1-159">Not supported</span></span> | <span data-ttu-id="84ca1-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84ca1-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="84ca1-161">邮件</span><span class="sxs-lookup"><span data-stu-id="84ca1-161">message</span></span>](../resources/message.md) | <span data-ttu-id="84ca1-162">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="84ca1-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="84ca1-163">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="84ca1-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="84ca1-164">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="84ca1-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="84ca1-165">状态</span><span class="sxs-lookup"><span data-stu-id="84ca1-165">presence</span></span>](../resources/presence.md) | <span data-ttu-id="84ca1-166">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="84ca1-166">Presence.Read.All</span></span> | <span data-ttu-id="84ca1-167">不支持</span><span class="sxs-lookup"><span data-stu-id="84ca1-167">Not supported</span></span> | <span data-ttu-id="84ca1-168">不支持</span><span class="sxs-lookup"><span data-stu-id="84ca1-168">Not supported</span></span> |
|[<span data-ttu-id="84ca1-169">printer</span><span class="sxs-lookup"><span data-stu-id="84ca1-169">printer</span></span>](../resources/printer.md) | <span data-ttu-id="84ca1-170">不支持</span><span class="sxs-lookup"><span data-stu-id="84ca1-170">Not supported</span></span> | <span data-ttu-id="84ca1-171">不支持</span><span class="sxs-lookup"><span data-stu-id="84ca1-171">Not supported</span></span> | <span data-ttu-id="84ca1-172">Printer.Read.All、Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84ca1-172">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="84ca1-173">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="84ca1-173">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="84ca1-174">不支持</span><span class="sxs-lookup"><span data-stu-id="84ca1-174">Not supported</span></span> | <span data-ttu-id="84ca1-175">不支持</span><span class="sxs-lookup"><span data-stu-id="84ca1-175">Not supported</span></span> | <span data-ttu-id="84ca1-176">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84ca1-176">PrintTaskDefinition.ReadWrite.All</span></span> |
|<span data-ttu-id="84ca1-177">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="84ca1-177">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="84ca1-178">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84ca1-178">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="84ca1-179">不支持</span><span class="sxs-lookup"><span data-stu-id="84ca1-179">Not supported</span></span> | <span data-ttu-id="84ca1-180">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84ca1-180">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="84ca1-181">todoTask</span><span class="sxs-lookup"><span data-stu-id="84ca1-181">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="84ca1-182">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84ca1-182">Tasks.ReadWrite</span></span> | <span data-ttu-id="84ca1-183">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84ca1-183">Tasks.ReadWrite</span></span> | <span data-ttu-id="84ca1-184">不支持</span><span class="sxs-lookup"><span data-stu-id="84ca1-184">Not supported</span></span> |
|[<span data-ttu-id="84ca1-185">用户</span><span class="sxs-lookup"><span data-stu-id="84ca1-185">user</span></span>](../resources/user.md) | <span data-ttu-id="84ca1-186">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="84ca1-186">User.Read.All</span></span> | <span data-ttu-id="84ca1-187">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="84ca1-187">User.Read.All</span></span> | <span data-ttu-id="84ca1-188">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="84ca1-188">User.Read.All</span></span> |

> <span data-ttu-id="84ca1-189">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="84ca1-189">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="84ca1-190">chatMessage</span><span class="sxs-lookup"><span data-stu-id="84ca1-190">chatMessage</span></span>

<span data-ttu-id="84ca1-191">**具有委派权限的 chatMessage** 订阅不支持资源数据 (**includeResourceData** 必须) ， `false` 并且不需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="84ca1-191">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="84ca1-192">具有应用程序权限的 **chatMessage** 订阅包含资源数据，并且需要进行 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="84ca1-192">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="84ca1-193">如果未指定 [encryptionCertificate](../resources/subscription.md)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="84ca1-193">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="84ca1-194">创建 **chatMessage** 订阅前，必须请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="84ca1-194">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="84ca1-195">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="84ca1-195">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="84ca1-196">**注意：** `/teams/getAllMessages` 和 `/chats/getAllMessages` 可供拥有 [所需许可证](https://aka.ms/teams-changenotification-licenses)的用户使用。</span><span class="sxs-lookup"><span data-stu-id="84ca1-196">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>
<span data-ttu-id="84ca1-197">将来，Microsoft 可能会要求你或你的客户根据通过 API 访问的数据量支付其他费用。</span><span class="sxs-lookup"><span data-stu-id="84ca1-197">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>

### <a name="driveitem"></a><span data-ttu-id="84ca1-198">driveItem</span><span class="sxs-lookup"><span data-stu-id="84ca1-198">driveItem</span></span>

<span data-ttu-id="84ca1-199">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="84ca1-199">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="84ca1-200">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="84ca1-200">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="84ca1-201">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="84ca1-201">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="84ca1-202">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="84ca1-202">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="84ca1-203">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="84ca1-203">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="84ca1-204">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="84ca1-204">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="84ca1-205">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="84ca1-205">contact, event, and message</span></span>

<span data-ttu-id="84ca1-206">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="84ca1-206">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="84ca1-207">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="84ca1-207">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="84ca1-208">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="84ca1-208">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="84ca1-209">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="84ca1-209">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="84ca1-210">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="84ca1-210">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="84ca1-211">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="84ca1-211">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="84ca1-212">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="84ca1-212">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="84ca1-213">状态</span><span class="sxs-lookup"><span data-stu-id="84ca1-213">presence</span></span>

<span data-ttu-id="84ca1-214">**状态** 订阅需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="84ca1-214">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="84ca1-215">如果未指定 [encryptionCertificate](../resources/subscription.md)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="84ca1-215">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="84ca1-216">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84ca1-216">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="84ca1-217">请求标头</span><span class="sxs-lookup"><span data-stu-id="84ca1-217">Request headers</span></span>

| <span data-ttu-id="84ca1-218">名称</span><span class="sxs-lookup"><span data-stu-id="84ca1-218">Name</span></span>       | <span data-ttu-id="84ca1-219">类型</span><span class="sxs-lookup"><span data-stu-id="84ca1-219">Type</span></span> | <span data-ttu-id="84ca1-220">说明</span><span class="sxs-lookup"><span data-stu-id="84ca1-220">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="84ca1-221">Authorization</span><span class="sxs-lookup"><span data-stu-id="84ca1-221">Authorization</span></span>  | <span data-ttu-id="84ca1-222">string</span><span class="sxs-lookup"><span data-stu-id="84ca1-222">string</span></span>  | <span data-ttu-id="84ca1-p109">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="84ca1-p109">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="84ca1-225">请求正文</span><span class="sxs-lookup"><span data-stu-id="84ca1-225">Request body</span></span>

<span data-ttu-id="84ca1-226">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="84ca1-226">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84ca1-227">响应</span><span class="sxs-lookup"><span data-stu-id="84ca1-227">Response</span></span>

<span data-ttu-id="84ca1-228">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="84ca1-228">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="84ca1-229">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="84ca1-229">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="84ca1-230">示例</span><span class="sxs-lookup"><span data-stu-id="84ca1-230">Example</span></span>

##### <a name="request"></a><span data-ttu-id="84ca1-231">请求</span><span class="sxs-lookup"><span data-stu-id="84ca1-231">Request</span></span>

<span data-ttu-id="84ca1-232">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="84ca1-232">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="84ca1-233">HTTP</span><span class="sxs-lookup"><span data-stu-id="84ca1-233">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="84ca1-234">C#</span><span class="sxs-lookup"><span data-stu-id="84ca1-234">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84ca1-235">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84ca1-235">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84ca1-236">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84ca1-236">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84ca1-237">Java</span><span class="sxs-lookup"><span data-stu-id="84ca1-237">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="84ca1-238">响应</span><span class="sxs-lookup"><span data-stu-id="84ca1-238">Response</span></span>

<span data-ttu-id="84ca1-239">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="84ca1-239">Here is an example of the response.</span></span>
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


