---
title: 获取订阅
description: 检索订阅的属性和关系。
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 058d4e918b629d0ff1572dffb2a38228de56afdf
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092727"
---
# <a name="get-subscription"></a><span data-ttu-id="d47ba-103">获取订阅</span><span class="sxs-lookup"><span data-stu-id="d47ba-103">Get subscription</span></span>

<span data-ttu-id="d47ba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d47ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d47ba-105">检索订阅的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d47ba-105">Retrieve the properties and relationships of a subscription.</span></span>

<span data-ttu-id="d47ba-106">有关支持订阅更改通知[](#permissions)的资源列表，请参阅"权限"部分中的表。</span><span class="sxs-lookup"><span data-stu-id="d47ba-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="d47ba-107">权限</span><span class="sxs-lookup"><span data-stu-id="d47ba-107">Permissions</span></span>

<span data-ttu-id="d47ba-108">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="d47ba-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="d47ba-109">若要了解 [更多信息，包括在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 选择更多特权权限之前保持谨慎，请搜索"权限"中的以下 [权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d47ba-109">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d47ba-110">支持的资源</span><span class="sxs-lookup"><span data-stu-id="d47ba-110">Supported resource</span></span> | <span data-ttu-id="d47ba-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d47ba-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d47ba-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d47ba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d47ba-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="d47ba-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="d47ba-114">callRecord</span><span class="sxs-lookup"><span data-stu-id="d47ba-114">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="d47ba-115">不支持</span><span class="sxs-lookup"><span data-stu-id="d47ba-115">Not supported</span></span> | <span data-ttu-id="d47ba-116">不支持</span><span class="sxs-lookup"><span data-stu-id="d47ba-116">Not supported</span></span> | <span data-ttu-id="d47ba-117">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="d47ba-117">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="d47ba-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="d47ba-118">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="d47ba-119">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d47ba-119">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="d47ba-120">不支持</span><span class="sxs-lookup"><span data-stu-id="d47ba-120">Not supported</span></span> | <span data-ttu-id="d47ba-121">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="d47ba-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="d47ba-122">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="d47ba-122">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="d47ba-123">不支持</span><span class="sxs-lookup"><span data-stu-id="d47ba-123">Not supported</span></span> | <span data-ttu-id="d47ba-124">不支持</span><span class="sxs-lookup"><span data-stu-id="d47ba-124">Not supported</span></span> | <span data-ttu-id="d47ba-125">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="d47ba-125">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="d47ba-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="d47ba-126">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="d47ba-127">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d47ba-127">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="d47ba-128">不支持</span><span class="sxs-lookup"><span data-stu-id="d47ba-128">Not supported</span></span> | <span data-ttu-id="d47ba-129">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="d47ba-129">Chat.Read.All</span></span>  |
|<span data-ttu-id="d47ba-130">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="d47ba-130">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="d47ba-131">不支持</span><span class="sxs-lookup"><span data-stu-id="d47ba-131">Not supported</span></span> | <span data-ttu-id="d47ba-132">不支持</span><span class="sxs-lookup"><span data-stu-id="d47ba-132">Not supported</span></span> | <span data-ttu-id="d47ba-133">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="d47ba-133">Chat.Read.All</span></span>  |
|[<span data-ttu-id="d47ba-134">contact</span><span class="sxs-lookup"><span data-stu-id="d47ba-134">contact</span></span>](../resources/contact.md) | <span data-ttu-id="d47ba-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d47ba-135">Contacts.Read</span></span> | <span data-ttu-id="d47ba-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d47ba-136">Contacts.Read</span></span> | <span data-ttu-id="d47ba-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d47ba-137">Contacts.Read</span></span> |
|<span data-ttu-id="d47ba-138">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="d47ba-138">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="d47ba-139">不支持</span><span class="sxs-lookup"><span data-stu-id="d47ba-139">Not supported</span></span> | <span data-ttu-id="d47ba-140">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d47ba-140">Files.ReadWrite</span></span> | <span data-ttu-id="d47ba-141">不支持</span><span class="sxs-lookup"><span data-stu-id="d47ba-141">Not supported</span></span> |
|<span data-ttu-id="d47ba-142">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="d47ba-142">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="d47ba-143">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d47ba-143">Files.ReadWrite.All</span></span> | <span data-ttu-id="d47ba-144">不支持</span><span class="sxs-lookup"><span data-stu-id="d47ba-144">Not supported</span></span> | <span data-ttu-id="d47ba-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d47ba-145">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="d47ba-146">事件</span><span class="sxs-lookup"><span data-stu-id="d47ba-146">event</span></span>](../resources/event.md) | <span data-ttu-id="d47ba-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d47ba-147">Calendars.Read</span></span> | <span data-ttu-id="d47ba-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d47ba-148">Calendars.Read</span></span> | <span data-ttu-id="d47ba-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d47ba-149">Calendars.Read</span></span> |
|[<span data-ttu-id="d47ba-150">组</span><span class="sxs-lookup"><span data-stu-id="d47ba-150">group</span></span>](../resources/group.md) | <span data-ttu-id="d47ba-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d47ba-151">Group.Read.All</span></span> | <span data-ttu-id="d47ba-152">不支持</span><span class="sxs-lookup"><span data-stu-id="d47ba-152">Not supported</span></span> | <span data-ttu-id="d47ba-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d47ba-153">Group.Read.All</span></span> |
|[<span data-ttu-id="d47ba-154">组对话</span><span class="sxs-lookup"><span data-stu-id="d47ba-154">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="d47ba-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d47ba-155">Group.Read.All</span></span> | <span data-ttu-id="d47ba-156">不支持</span><span class="sxs-lookup"><span data-stu-id="d47ba-156">Not supported</span></span> | <span data-ttu-id="d47ba-157">不支持</span><span class="sxs-lookup"><span data-stu-id="d47ba-157">Not supported</span></span> |
|[<span data-ttu-id="d47ba-158">列表</span><span class="sxs-lookup"><span data-stu-id="d47ba-158">list</span></span>](../resources/list.md) | <span data-ttu-id="d47ba-159">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d47ba-159">Sites.ReadWrite.All</span></span> | <span data-ttu-id="d47ba-160">不支持</span><span class="sxs-lookup"><span data-stu-id="d47ba-160">Not supported</span></span> | <span data-ttu-id="d47ba-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d47ba-161">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="d47ba-162">邮件</span><span class="sxs-lookup"><span data-stu-id="d47ba-162">message</span></span>](../resources/message.md) | <span data-ttu-id="d47ba-163">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d47ba-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="d47ba-164">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d47ba-164">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="d47ba-165">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d47ba-165">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="d47ba-166">状态</span><span class="sxs-lookup"><span data-stu-id="d47ba-166">presence</span></span>](../resources/presence.md) | <span data-ttu-id="d47ba-167">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="d47ba-167">Presence.Read.All</span></span> | <span data-ttu-id="d47ba-168">不支持</span><span class="sxs-lookup"><span data-stu-id="d47ba-168">Not supported</span></span> | <span data-ttu-id="d47ba-169">不支持</span><span class="sxs-lookup"><span data-stu-id="d47ba-169">Not supported</span></span> |
|[<span data-ttu-id="d47ba-170">打印机</span><span class="sxs-lookup"><span data-stu-id="d47ba-170">printer</span></span>](../resources/printer.md) | <span data-ttu-id="d47ba-171">不支持</span><span class="sxs-lookup"><span data-stu-id="d47ba-171">Not supported</span></span> | <span data-ttu-id="d47ba-172">不支持</span><span class="sxs-lookup"><span data-stu-id="d47ba-172">Not supported</span></span> | <span data-ttu-id="d47ba-173">Printer.Read.All、Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d47ba-173">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="d47ba-174">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="d47ba-174">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="d47ba-175">不支持</span><span class="sxs-lookup"><span data-stu-id="d47ba-175">Not supported</span></span> | <span data-ttu-id="d47ba-176">不支持</span><span class="sxs-lookup"><span data-stu-id="d47ba-176">Not supported</span></span> | <span data-ttu-id="d47ba-177">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d47ba-177">PrintTaskDefinition.ReadWrite.All</span></span> |
|<span data-ttu-id="d47ba-178">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="d47ba-178">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="d47ba-179">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d47ba-179">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="d47ba-180">不支持</span><span class="sxs-lookup"><span data-stu-id="d47ba-180">Not supported</span></span> | <span data-ttu-id="d47ba-181">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d47ba-181">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="d47ba-182">todoTask</span><span class="sxs-lookup"><span data-stu-id="d47ba-182">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="d47ba-183">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d47ba-183">Tasks.ReadWrite</span></span> | <span data-ttu-id="d47ba-184">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d47ba-184">Tasks.ReadWrite</span></span> | <span data-ttu-id="d47ba-185">不支持</span><span class="sxs-lookup"><span data-stu-id="d47ba-185">Not supported</span></span> |
|[<span data-ttu-id="d47ba-186">用户</span><span class="sxs-lookup"><span data-stu-id="d47ba-186">user</span></span>](../resources/user.md) | <span data-ttu-id="d47ba-187">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d47ba-187">User.Read.All</span></span> | <span data-ttu-id="d47ba-188">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d47ba-188">User.Read.All</span></span> | <span data-ttu-id="d47ba-189">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d47ba-189">User.Read.All</span></span> |

> <span data-ttu-id="d47ba-190">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="d47ba-190">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="d47ba-191">driveItem</span><span class="sxs-lookup"><span data-stu-id="d47ba-191">driveItem</span></span>

<span data-ttu-id="d47ba-192">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="d47ba-192">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="d47ba-193">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="d47ba-193">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="d47ba-194">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="d47ba-194">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="d47ba-195">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="d47ba-195">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="d47ba-196">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="d47ba-196">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="d47ba-197">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="d47ba-197">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="d47ba-198">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="d47ba-198">contact, event, and message</span></span>

<span data-ttu-id="d47ba-199">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="d47ba-199">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="d47ba-200">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="d47ba-200">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="d47ba-201">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="d47ba-201">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="d47ba-202">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="d47ba-202">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="d47ba-203">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="d47ba-203">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="d47ba-204">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="d47ba-204">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="d47ba-205">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="d47ba-205">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="d47ba-206">状态</span><span class="sxs-lookup"><span data-stu-id="d47ba-206">presence</span></span>

<span data-ttu-id="d47ba-207">**状态** 订阅需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="d47ba-207">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="d47ba-208">如果未指定 [encryptionCertificate](../resources/subscription.md)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="d47ba-208">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="d47ba-209">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d47ba-209">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d47ba-210">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d47ba-210">Optional query parameters</span></span>

<span data-ttu-id="d47ba-211">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d47ba-211">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d47ba-212">请求标头</span><span class="sxs-lookup"><span data-stu-id="d47ba-212">Request headers</span></span>

| <span data-ttu-id="d47ba-213">名称</span><span class="sxs-lookup"><span data-stu-id="d47ba-213">Name</span></span>       | <span data-ttu-id="d47ba-214">类型</span><span class="sxs-lookup"><span data-stu-id="d47ba-214">Type</span></span> | <span data-ttu-id="d47ba-215">说明</span><span class="sxs-lookup"><span data-stu-id="d47ba-215">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="d47ba-216">Authorization</span><span class="sxs-lookup"><span data-stu-id="d47ba-216">Authorization</span></span>  | <span data-ttu-id="d47ba-217">string</span><span class="sxs-lookup"><span data-stu-id="d47ba-217">string</span></span>  | <span data-ttu-id="d47ba-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d47ba-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d47ba-220">请求正文</span><span class="sxs-lookup"><span data-stu-id="d47ba-220">Request body</span></span>

<span data-ttu-id="d47ba-221">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d47ba-221">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d47ba-222">响应</span><span class="sxs-lookup"><span data-stu-id="d47ba-222">Response</span></span>

<span data-ttu-id="d47ba-223">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d47ba-223">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d47ba-224">示例</span><span class="sxs-lookup"><span data-stu-id="d47ba-224">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d47ba-225">请求</span><span class="sxs-lookup"><span data-stu-id="d47ba-225">Request</span></span>

<span data-ttu-id="d47ba-226">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d47ba-226">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d47ba-227">HTTP</span><span class="sxs-lookup"><span data-stu-id="d47ba-227">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="d47ba-228">C#</span><span class="sxs-lookup"><span data-stu-id="d47ba-228">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d47ba-229">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d47ba-229">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d47ba-230">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d47ba-230">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d47ba-231">Java</span><span class="sxs-lookup"><span data-stu-id="d47ba-231">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d47ba-232">响应</span><span class="sxs-lookup"><span data-stu-id="d47ba-232">Response</span></span>

<span data-ttu-id="d47ba-233">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d47ba-233">Here is an example of the response.</span></span>
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


