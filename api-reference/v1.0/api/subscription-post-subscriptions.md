---
title: 创建订阅
description: 订阅侦听器应用程序，以在 Microsoft Graph 中的数据发生更改时接收更改通知。
localization_priority: Priority
author: Jumaodhiss
ms.prod: change-notifications
doc_type: apiPageType
ms.openlocfilehash: 239de6da37b9e795c5b0c2eec359f0b4b457f5f4
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912052"
---
# <a name="create-subscription"></a><span data-ttu-id="0665e-103">创建订阅</span><span class="sxs-lookup"><span data-stu-id="0665e-103">Create subscription</span></span>

<span data-ttu-id="0665e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0665e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0665e-105">订阅侦听器应用程序，以在 Microsoft Graph 中指定资源发生的更改属于请求的更改类型时接收更改通知。</span><span class="sxs-lookup"><span data-stu-id="0665e-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

<span data-ttu-id="0665e-106">请参阅" [权限](#permissions) 部分中的表格，了解支持订阅以更改通知的资源列表。</span><span class="sxs-lookup"><span data-stu-id="0665e-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="0665e-107">权限</span><span class="sxs-lookup"><span data-stu-id="0665e-107">Permissions</span></span>

<span data-ttu-id="0665e-108">创建订阅需要读取资源范围。</span><span class="sxs-lookup"><span data-stu-id="0665e-108">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="0665e-109">例如，若要获取更改消息通知，应用需要 `Mail.Read` 权限。</span><span class="sxs-lookup"><span data-stu-id="0665e-109">For example, to get change notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
<span data-ttu-id="0665e-110">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="0665e-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="0665e-111">若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0665e-111">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0665e-112">支持的资源</span><span class="sxs-lookup"><span data-stu-id="0665e-112">Supported resource</span></span> | <span data-ttu-id="0665e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0665e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0665e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0665e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0665e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0665e-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="0665e-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="0665e-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="0665e-117">不支持</span><span class="sxs-lookup"><span data-stu-id="0665e-117">Not supported</span></span> | <span data-ttu-id="0665e-118">不支持</span><span class="sxs-lookup"><span data-stu-id="0665e-118">Not supported</span></span> | <span data-ttu-id="0665e-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="0665e-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="0665e-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="0665e-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="0665e-121">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="0665e-121">ChannelMessage.Read.All</span></span> | <span data-ttu-id="0665e-122">不支持</span><span class="sxs-lookup"><span data-stu-id="0665e-122">Not supported</span></span> |  <span data-ttu-id="0665e-123">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="0665e-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="0665e-124">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="0665e-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="0665e-125">不支持</span><span class="sxs-lookup"><span data-stu-id="0665e-125">Not supported</span></span> | <span data-ttu-id="0665e-126">不支持</span><span class="sxs-lookup"><span data-stu-id="0665e-126">Not supported</span></span> | <span data-ttu-id="0665e-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="0665e-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="0665e-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="0665e-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="0665e-129">不支持</span><span class="sxs-lookup"><span data-stu-id="0665e-129">Not supported</span></span> | <span data-ttu-id="0665e-130">不支持</span><span class="sxs-lookup"><span data-stu-id="0665e-130">Not supported</span></span> | <span data-ttu-id="0665e-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="0665e-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="0665e-132">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="0665e-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="0665e-133">不支持</span><span class="sxs-lookup"><span data-stu-id="0665e-133">Not supported</span></span> | <span data-ttu-id="0665e-134">不支持</span><span class="sxs-lookup"><span data-stu-id="0665e-134">Not supported</span></span> | <span data-ttu-id="0665e-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="0665e-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="0665e-136">contact</span><span class="sxs-lookup"><span data-stu-id="0665e-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="0665e-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="0665e-137">Contacts.Read</span></span> | <span data-ttu-id="0665e-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="0665e-138">Contacts.Read</span></span> | <span data-ttu-id="0665e-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="0665e-139">Contacts.Read</span></span> |
|<span data-ttu-id="0665e-140">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="0665e-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="0665e-141">不支持</span><span class="sxs-lookup"><span data-stu-id="0665e-141">Not supported</span></span> | <span data-ttu-id="0665e-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0665e-142">Files.ReadWrite</span></span> | <span data-ttu-id="0665e-143">不支持</span><span class="sxs-lookup"><span data-stu-id="0665e-143">Not supported</span></span> |
|<span data-ttu-id="0665e-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="0665e-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="0665e-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0665e-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="0665e-146">不支持</span><span class="sxs-lookup"><span data-stu-id="0665e-146">Not supported</span></span> | <span data-ttu-id="0665e-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0665e-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="0665e-148">事件</span><span class="sxs-lookup"><span data-stu-id="0665e-148">event</span></span>](../resources/event.md) | <span data-ttu-id="0665e-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0665e-149">Calendars.Read</span></span> | <span data-ttu-id="0665e-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0665e-150">Calendars.Read</span></span> | <span data-ttu-id="0665e-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0665e-151">Calendars.Read</span></span> |
|[<span data-ttu-id="0665e-152">组</span><span class="sxs-lookup"><span data-stu-id="0665e-152">group</span></span>](../resources/group.md) | <span data-ttu-id="0665e-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0665e-153">Group.Read.All</span></span> | <span data-ttu-id="0665e-154">不支持</span><span class="sxs-lookup"><span data-stu-id="0665e-154">Not supported</span></span> | <span data-ttu-id="0665e-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0665e-155">Group.Read.All</span></span> |
|[<span data-ttu-id="0665e-156">组对话</span><span class="sxs-lookup"><span data-stu-id="0665e-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="0665e-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0665e-157">Group.Read.All</span></span> | <span data-ttu-id="0665e-158">不支持</span><span class="sxs-lookup"><span data-stu-id="0665e-158">Not supported</span></span> | <span data-ttu-id="0665e-159">不支持</span><span class="sxs-lookup"><span data-stu-id="0665e-159">Not supported</span></span> |
|[<span data-ttu-id="0665e-160">列表</span><span class="sxs-lookup"><span data-stu-id="0665e-160">list</span></span>](../resources/list.md) | <span data-ttu-id="0665e-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0665e-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="0665e-162">不支持</span><span class="sxs-lookup"><span data-stu-id="0665e-162">Not supported</span></span> | <span data-ttu-id="0665e-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0665e-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="0665e-164">邮件</span><span class="sxs-lookup"><span data-stu-id="0665e-164">message</span></span>](../resources/message.md) | <span data-ttu-id="0665e-165">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0665e-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="0665e-166">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0665e-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="0665e-167">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0665e-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="0665e-168">打印机</span><span class="sxs-lookup"><span data-stu-id="0665e-168">printer</span></span>](../resources/printer.md) | <span data-ttu-id="0665e-169">不支持</span><span class="sxs-lookup"><span data-stu-id="0665e-169">Not supported</span></span> | <span data-ttu-id="0665e-170">不支持</span><span class="sxs-lookup"><span data-stu-id="0665e-170">Not supported</span></span> | <span data-ttu-id="0665e-171">打印机。阅读.All，Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0665e-171">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="0665e-172">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="0665e-172">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="0665e-173">不支持</span><span class="sxs-lookup"><span data-stu-id="0665e-173">Not supported</span></span> | <span data-ttu-id="0665e-174">不支持</span><span class="sxs-lookup"><span data-stu-id="0665e-174">Not supported</span></span> | <span data-ttu-id="0665e-175">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0665e-175">PrintTaskDefinition.ReadWrite.All</span></span> |
|<span data-ttu-id="0665e-176">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="0665e-176">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="0665e-177">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0665e-177">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="0665e-178">不支持</span><span class="sxs-lookup"><span data-stu-id="0665e-178">Not supported</span></span> | <span data-ttu-id="0665e-179">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0665e-179">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="0665e-180">用户</span><span class="sxs-lookup"><span data-stu-id="0665e-180">user</span></span>](../resources/user.md) | <span data-ttu-id="0665e-181">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="0665e-181">User.Read.All</span></span> | <span data-ttu-id="0665e-182">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="0665e-182">User.Read.All</span></span> | <span data-ttu-id="0665e-183">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="0665e-183">User.Read.All</span></span> |

> <span data-ttu-id="0665e-184">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="0665e-184">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="0665e-185">driveItem</span><span class="sxs-lookup"><span data-stu-id="0665e-185">driveItem</span></span>

<span data-ttu-id="0665e-186">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="0665e-186">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="0665e-187">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="0665e-187">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="0665e-188">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="0665e-188">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="0665e-189">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="0665e-189">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="0665e-190">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="0665e-190">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="0665e-191">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="0665e-191">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

<span data-ttu-id="0665e-192">OneDrive for Business 和 SharePoint 支持向应用程序发送有关在 **driveItem** 上发生的安全事件通知。</span><span class="sxs-lookup"><span data-stu-id="0665e-192">OneDrive for Business and SharePoint support sending your application notifications of security events that occur on a **driveItem**.</span></span> <span data-ttu-id="0665e-193">若要订阅这些事件，请为请求添加 `prefer:includesecuritywebhooks` 标头以创建订阅。</span><span class="sxs-lookup"><span data-stu-id="0665e-193">To subscribe to these events, add the `prefer:includesecuritywebhooks` header to your request to create a subscription.</span></span> <span data-ttu-id="0665e-194">创建订阅后，当项目权限更改时，你将收到通知。</span><span class="sxs-lookup"><span data-stu-id="0665e-194">After the subscription is created, you will receive notifications when the permissions on an item change.</span></span> <span data-ttu-id="0665e-195">此标头适用于 SharePoint 和 OneDrive for Business 帐户，但不适用于 OneDrive 消费者版本的帐户。</span><span class="sxs-lookup"><span data-stu-id="0665e-195">This header is applicable to SharePoint and OneDrive for Business but not consumer OneDrive accounts.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="0665e-196">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="0665e-196">contact, event, and message</span></span>

<span data-ttu-id="0665e-197">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="0665e-197">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="0665e-198">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="0665e-198">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="0665e-199">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="0665e-199">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="0665e-200">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="0665e-200">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="0665e-201">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="0665e-201">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="0665e-202">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="0665e-202">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="0665e-203">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="0665e-203">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="0665e-204">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0665e-204">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="0665e-205">请求标头</span><span class="sxs-lookup"><span data-stu-id="0665e-205">Request headers</span></span>

| <span data-ttu-id="0665e-206">名称</span><span class="sxs-lookup"><span data-stu-id="0665e-206">Name</span></span>       | <span data-ttu-id="0665e-207">类型</span><span class="sxs-lookup"><span data-stu-id="0665e-207">Type</span></span> | <span data-ttu-id="0665e-208">说明</span><span class="sxs-lookup"><span data-stu-id="0665e-208">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0665e-209">Authorization</span><span class="sxs-lookup"><span data-stu-id="0665e-209">Authorization</span></span>  | <span data-ttu-id="0665e-210">string</span><span class="sxs-lookup"><span data-stu-id="0665e-210">string</span></span>  | <span data-ttu-id="0665e-p108">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0665e-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0665e-213">响应</span><span class="sxs-lookup"><span data-stu-id="0665e-213">Response</span></span>

<span data-ttu-id="0665e-214">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0665e-214">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>
<span data-ttu-id="0665e-215">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="0665e-215">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="0665e-216">示例</span><span class="sxs-lookup"><span data-stu-id="0665e-216">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0665e-217">请求</span><span class="sxs-lookup"><span data-stu-id="0665e-217">Request</span></span>

<span data-ttu-id="0665e-218">下面是在用户收到新邮件时请求发送更改通知的示例。</span><span class="sxs-lookup"><span data-stu-id="0665e-218">Here is an example of the request to send a change notification when the user receives a new mail.</span></span>

# <a name="http"></a>[<span data-ttu-id="0665e-219">HTTP</span><span class="sxs-lookup"><span data-stu-id="0665e-219">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
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
# <a name="c"></a>[<span data-ttu-id="0665e-220">C#</span><span class="sxs-lookup"><span data-stu-id="0665e-220">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0665e-221">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0665e-221">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0665e-222">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0665e-222">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0665e-223">Java</span><span class="sxs-lookup"><span data-stu-id="0665e-223">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="0665e-224">在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0665e-224">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="0665e-225">`clientState` 和 `latestSupportedTlsVersion` 是可选字段。</span><span class="sxs-lookup"><span data-stu-id="0665e-225">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="0665e-226">资源示例</span><span class="sxs-lookup"><span data-stu-id="0665e-226">Resources examples</span></span>

<span data-ttu-id="0665e-227">订阅资源属性的有效值如下：</span><span class="sxs-lookup"><span data-stu-id="0665e-227">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="0665e-228">资源类型</span><span class="sxs-lookup"><span data-stu-id="0665e-228">Resource type</span></span> | <span data-ttu-id="0665e-229">示例</span><span class="sxs-lookup"><span data-stu-id="0665e-229">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="0665e-230">通话记录</span><span class="sxs-lookup"><span data-stu-id="0665e-230">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="0665e-231">聊天消息</span><span class="sxs-lookup"><span data-stu-id="0665e-231">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="0665e-232">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="0665e-232">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="0665e-233">联系人</span><span class="sxs-lookup"><span data-stu-id="0665e-233">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="0665e-234">对话</span><span class="sxs-lookup"><span data-stu-id="0665e-234">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="0665e-235">驱动器</span><span class="sxs-lookup"><span data-stu-id="0665e-235">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="0665e-236">事件</span><span class="sxs-lookup"><span data-stu-id="0665e-236">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="0665e-237">组</span><span class="sxs-lookup"><span data-stu-id="0665e-237">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="0665e-238">列表</span><span class="sxs-lookup"><span data-stu-id="0665e-238">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="0665e-239">邮件</span><span class="sxs-lookup"><span data-stu-id="0665e-239">Mail</span></span>](../resources/message.md)|<span data-ttu-id="0665e-240">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="0665e-240">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="0665e-241">打印机</span><span class="sxs-lookup"><span data-stu-id="0665e-241">printer</span></span>](../resources/printer.md) |`print/printers/{id}/jobs`|
|[<span data-ttu-id="0665e-242">PrintTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="0665e-242">PrintTaskDefinition</span></span>](../resources/printtaskdefinition.md)|`print/taskDefinitions/{id}/tasks`|
|[<span data-ttu-id="0665e-243">安全警报</span><span class="sxs-lookup"><span data-stu-id="0665e-243">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'New'`|
|[<span data-ttu-id="0665e-244">用户</span><span class="sxs-lookup"><span data-stu-id="0665e-244">Users</span></span>](../resources/user.md)|`users`|

> <span data-ttu-id="0665e-245">**注意：** 以 `me` 开头的任何路径也可与 `users/{id}`（而不是 `me`）一起使用，从而以特定用户为目标，而不是以当前用户为目标。</span><span class="sxs-lookup"><span data-stu-id="0665e-245">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

##### <a name="response"></a><span data-ttu-id="0665e-246">响应</span><span class="sxs-lookup"><span data-stu-id="0665e-246">Response</span></span>

<span data-ttu-id="0665e-p111">这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0665e-p111">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2",
  "notificationContentType": "application/json"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="0665e-249">通知终结点验证</span><span class="sxs-lookup"><span data-stu-id="0665e-249">Notification endpoint validation</span></span>

<span data-ttu-id="0665e-250">通知终结点（于 `notificationUrl` 属性中指定）必须能够响应验证请求，如[设置用户数据更改的通知](/graph/webhooks#notification-endpoint-validation)中所述。</span><span class="sxs-lookup"><span data-stu-id="0665e-250">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="0665e-251">如果验证失败，创建订阅请求返回错误“400 请求无效”。</span><span class="sxs-lookup"><span data-stu-id="0665e-251">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

[error-response]: /graph/errors

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

