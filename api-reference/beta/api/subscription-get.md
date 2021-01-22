---
title: 获取订阅
description: 检索订阅的属性和关系。
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 1c5187eb36ace429d97c71a127a7c61768a4971d
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934701"
---
# <a name="get-subscription"></a><span data-ttu-id="651ce-103">获取订阅</span><span class="sxs-lookup"><span data-stu-id="651ce-103">Get subscription</span></span>

<span data-ttu-id="651ce-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="651ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="651ce-105">检索订阅的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="651ce-105">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="651ce-106">权限</span><span class="sxs-lookup"><span data-stu-id="651ce-106">Permissions</span></span>

<span data-ttu-id="651ce-107">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="651ce-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="651ce-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="651ce-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="651ce-109">支持的资源</span><span class="sxs-lookup"><span data-stu-id="651ce-109">Supported resource</span></span> | <span data-ttu-id="651ce-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="651ce-110">Delegated (work or school account)</span></span> | <span data-ttu-id="651ce-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="651ce-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="651ce-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="651ce-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="651ce-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="651ce-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="651ce-114">不支持</span><span class="sxs-lookup"><span data-stu-id="651ce-114">Not supported</span></span> | <span data-ttu-id="651ce-115">不支持</span><span class="sxs-lookup"><span data-stu-id="651ce-115">Not supported</span></span> | <span data-ttu-id="651ce-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="651ce-116">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="651ce-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="651ce-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="651ce-118">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="651ce-118">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="651ce-119">不支持</span><span class="sxs-lookup"><span data-stu-id="651ce-119">Not supported</span></span> | <span data-ttu-id="651ce-120">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="651ce-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="651ce-121">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="651ce-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="651ce-122">不支持</span><span class="sxs-lookup"><span data-stu-id="651ce-122">Not supported</span></span> | <span data-ttu-id="651ce-123">不支持</span><span class="sxs-lookup"><span data-stu-id="651ce-123">Not supported</span></span> | <span data-ttu-id="651ce-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="651ce-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="651ce-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="651ce-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="651ce-126">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="651ce-126">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="651ce-127">不支持</span><span class="sxs-lookup"><span data-stu-id="651ce-127">Not supported</span></span> | <span data-ttu-id="651ce-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="651ce-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="651ce-129">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="651ce-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="651ce-130">不支持</span><span class="sxs-lookup"><span data-stu-id="651ce-130">Not supported</span></span> | <span data-ttu-id="651ce-131">不支持</span><span class="sxs-lookup"><span data-stu-id="651ce-131">Not supported</span></span> | <span data-ttu-id="651ce-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="651ce-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="651ce-133">contact</span><span class="sxs-lookup"><span data-stu-id="651ce-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="651ce-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="651ce-134">Contacts.Read</span></span> | <span data-ttu-id="651ce-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="651ce-135">Contacts.Read</span></span> | <span data-ttu-id="651ce-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="651ce-136">Contacts.Read</span></span> |
|<span data-ttu-id="651ce-137">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="651ce-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="651ce-138">不支持</span><span class="sxs-lookup"><span data-stu-id="651ce-138">Not supported</span></span> | <span data-ttu-id="651ce-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="651ce-139">Files.ReadWrite</span></span> | <span data-ttu-id="651ce-140">不支持</span><span class="sxs-lookup"><span data-stu-id="651ce-140">Not supported</span></span> |
|<span data-ttu-id="651ce-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="651ce-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="651ce-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="651ce-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="651ce-143">不支持</span><span class="sxs-lookup"><span data-stu-id="651ce-143">Not supported</span></span> | <span data-ttu-id="651ce-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="651ce-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="651ce-145">事件</span><span class="sxs-lookup"><span data-stu-id="651ce-145">event</span></span>](../resources/event.md) | <span data-ttu-id="651ce-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="651ce-146">Calendars.Read</span></span> | <span data-ttu-id="651ce-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="651ce-147">Calendars.Read</span></span> | <span data-ttu-id="651ce-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="651ce-148">Calendars.Read</span></span> |
|[<span data-ttu-id="651ce-149">组</span><span class="sxs-lookup"><span data-stu-id="651ce-149">group</span></span>](../resources/group.md) | <span data-ttu-id="651ce-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="651ce-150">Group.Read.All</span></span> | <span data-ttu-id="651ce-151">不支持</span><span class="sxs-lookup"><span data-stu-id="651ce-151">Not supported</span></span> | <span data-ttu-id="651ce-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="651ce-152">Group.Read.All</span></span> |
|[<span data-ttu-id="651ce-153">组对话</span><span class="sxs-lookup"><span data-stu-id="651ce-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="651ce-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="651ce-154">Group.Read.All</span></span> | <span data-ttu-id="651ce-155">不支持</span><span class="sxs-lookup"><span data-stu-id="651ce-155">Not supported</span></span> | <span data-ttu-id="651ce-156">不支持</span><span class="sxs-lookup"><span data-stu-id="651ce-156">Not supported</span></span> |
|[<span data-ttu-id="651ce-157">列表</span><span class="sxs-lookup"><span data-stu-id="651ce-157">list</span></span>](../resources/list.md) | <span data-ttu-id="651ce-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="651ce-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="651ce-159">不支持</span><span class="sxs-lookup"><span data-stu-id="651ce-159">Not supported</span></span> | <span data-ttu-id="651ce-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="651ce-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="651ce-161">邮件</span><span class="sxs-lookup"><span data-stu-id="651ce-161">message</span></span>](../resources/message.md) | <span data-ttu-id="651ce-162">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="651ce-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="651ce-163">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="651ce-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="651ce-164">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="651ce-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="651ce-165">状态</span><span class="sxs-lookup"><span data-stu-id="651ce-165">presence</span></span>](../resources/presence.md) | <span data-ttu-id="651ce-166">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="651ce-166">Presence.Read.All</span></span> | <span data-ttu-id="651ce-167">不支持</span><span class="sxs-lookup"><span data-stu-id="651ce-167">Not supported</span></span> | <span data-ttu-id="651ce-168">不支持</span><span class="sxs-lookup"><span data-stu-id="651ce-168">Not supported</span></span> |
|[<span data-ttu-id="651ce-169">printer</span><span class="sxs-lookup"><span data-stu-id="651ce-169">printer</span></span>](../resources/printer.md) | <span data-ttu-id="651ce-170">不支持</span><span class="sxs-lookup"><span data-stu-id="651ce-170">Not supported</span></span> | <span data-ttu-id="651ce-171">不支持</span><span class="sxs-lookup"><span data-stu-id="651ce-171">Not supported</span></span> | <span data-ttu-id="651ce-172">Printer.Read.All、Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="651ce-172">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="651ce-173">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="651ce-173">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="651ce-174">不支持</span><span class="sxs-lookup"><span data-stu-id="651ce-174">Not supported</span></span> | <span data-ttu-id="651ce-175">不支持</span><span class="sxs-lookup"><span data-stu-id="651ce-175">Not supported</span></span> | <span data-ttu-id="651ce-176">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="651ce-176">PrintTaskDefinition.ReadWrite.All</span></span> |
|<span data-ttu-id="651ce-177">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="651ce-177">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="651ce-178">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="651ce-178">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="651ce-179">不支持</span><span class="sxs-lookup"><span data-stu-id="651ce-179">Not supported</span></span> | <span data-ttu-id="651ce-180">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="651ce-180">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="651ce-181">todoTask</span><span class="sxs-lookup"><span data-stu-id="651ce-181">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="651ce-182">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="651ce-182">Tasks.ReadWrite</span></span> | <span data-ttu-id="651ce-183">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="651ce-183">Tasks.ReadWrite</span></span> | <span data-ttu-id="651ce-184">不支持</span><span class="sxs-lookup"><span data-stu-id="651ce-184">Not supported</span></span> |
|[<span data-ttu-id="651ce-185">用户</span><span class="sxs-lookup"><span data-stu-id="651ce-185">user</span></span>](../resources/user.md) | <span data-ttu-id="651ce-186">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="651ce-186">User.Read.All</span></span> | <span data-ttu-id="651ce-187">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="651ce-187">User.Read.All</span></span> | <span data-ttu-id="651ce-188">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="651ce-188">User.Read.All</span></span> |

> <span data-ttu-id="651ce-189">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="651ce-189">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="651ce-190">chatMessage</span><span class="sxs-lookup"><span data-stu-id="651ce-190">chatMessage</span></span>

<span data-ttu-id="651ce-191">**具有委派权限的 chatMessage** 订阅不支持资源数据 (**includeResourceData** 必须) ， `false` 并且不需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="651ce-191">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="651ce-192">具有应用程序权限的 **chatMessage** 订阅包含资源数据，并且需要进行 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="651ce-192">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="651ce-193">如果未指定 [encryptionCertificate](../resources/subscription.md)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="651ce-193">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="651ce-194">创建 **chatMessage** 订阅前，必须请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="651ce-194">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="651ce-195">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="651ce-195">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="651ce-196">**注意：** `/teams/getAllMessages` 和 `/chats/getAllMessages` 可供拥有 [所需许可证](https://aka.ms/teams-changenotification-licenses)的用户使用。</span><span class="sxs-lookup"><span data-stu-id="651ce-196">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>
<span data-ttu-id="651ce-197">将来，Microsoft 可能会要求你或你的客户根据通过 API 访问的数据量支付其他费用。</span><span class="sxs-lookup"><span data-stu-id="651ce-197">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>

### <a name="driveitem"></a><span data-ttu-id="651ce-198">driveItem</span><span class="sxs-lookup"><span data-stu-id="651ce-198">driveItem</span></span>

<span data-ttu-id="651ce-199">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="651ce-199">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="651ce-200">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="651ce-200">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="651ce-201">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="651ce-201">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="651ce-202">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="651ce-202">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="651ce-203">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="651ce-203">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="651ce-204">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="651ce-204">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="651ce-205">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="651ce-205">contact, event, and message</span></span>

<span data-ttu-id="651ce-206">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="651ce-206">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="651ce-207">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="651ce-207">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="651ce-208">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="651ce-208">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="651ce-209">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="651ce-209">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="651ce-210">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="651ce-210">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="651ce-211">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="651ce-211">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="651ce-212">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="651ce-212">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="651ce-213">状态</span><span class="sxs-lookup"><span data-stu-id="651ce-213">presence</span></span>

<span data-ttu-id="651ce-214">**状态** 订阅需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="651ce-214">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="651ce-215">如果未指定 [encryptionCertificate](../resources/subscription.md)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="651ce-215">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="651ce-216">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="651ce-216">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="651ce-217">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="651ce-217">Optional query parameters</span></span>

<span data-ttu-id="651ce-218">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="651ce-218">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="651ce-219">请求标头</span><span class="sxs-lookup"><span data-stu-id="651ce-219">Request headers</span></span>

| <span data-ttu-id="651ce-220">名称</span><span class="sxs-lookup"><span data-stu-id="651ce-220">Name</span></span>       | <span data-ttu-id="651ce-221">类型</span><span class="sxs-lookup"><span data-stu-id="651ce-221">Type</span></span> | <span data-ttu-id="651ce-222">说明</span><span class="sxs-lookup"><span data-stu-id="651ce-222">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="651ce-223">Authorization</span><span class="sxs-lookup"><span data-stu-id="651ce-223">Authorization</span></span>  | <span data-ttu-id="651ce-224">string</span><span class="sxs-lookup"><span data-stu-id="651ce-224">string</span></span>  | <span data-ttu-id="651ce-p109">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="651ce-p109">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="651ce-227">请求正文</span><span class="sxs-lookup"><span data-stu-id="651ce-227">Request body</span></span>

<span data-ttu-id="651ce-228">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="651ce-228">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="651ce-229">响应</span><span class="sxs-lookup"><span data-stu-id="651ce-229">Response</span></span>

<span data-ttu-id="651ce-230">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="651ce-230">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="651ce-231">示例</span><span class="sxs-lookup"><span data-stu-id="651ce-231">Example</span></span>

##### <a name="request"></a><span data-ttu-id="651ce-232">请求</span><span class="sxs-lookup"><span data-stu-id="651ce-232">Request</span></span>

<span data-ttu-id="651ce-233">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="651ce-233">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="651ce-234">HTTP</span><span class="sxs-lookup"><span data-stu-id="651ce-234">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="651ce-235">C#</span><span class="sxs-lookup"><span data-stu-id="651ce-235">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="651ce-236">JavaScript</span><span class="sxs-lookup"><span data-stu-id="651ce-236">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="651ce-237">Objective-C</span><span class="sxs-lookup"><span data-stu-id="651ce-237">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="651ce-238">Java</span><span class="sxs-lookup"><span data-stu-id="651ce-238">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="651ce-239">响应</span><span class="sxs-lookup"><span data-stu-id="651ce-239">Response</span></span>

<span data-ttu-id="651ce-240">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="651ce-240">Here is an example of the response.</span></span>
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
  "lifecycleNotificationUrl":"https://webhook.azurewebsites.net/api/send/lifecycleNotifications",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string",
  "latestSupportedTlsVersion": "v1_2",
  "encryptionCertificate": "",
  "encryptionCertificateId": "",
  "includeResourceData": false
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


