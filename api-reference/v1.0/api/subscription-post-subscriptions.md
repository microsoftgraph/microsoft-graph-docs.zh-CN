---
title: 创建订阅
description: 订阅侦听器应用程序，以在 Microsoft Graph 中的数据发生更改时接收更改通知。
localization_priority: Priority
author: Jumaodhiss
ms.prod: change-notifications
doc_type: apiPageType
ms.openlocfilehash: 733e9d0665e135d2e5dd1be152e6676c184252c5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055769"
---
# <a name="create-subscription"></a><span data-ttu-id="5d1e0-103">创建订阅</span><span class="sxs-lookup"><span data-stu-id="5d1e0-103">Create subscription</span></span>

<span data-ttu-id="5d1e0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d1e0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5d1e0-105">订阅侦听器应用程序，以在 Microsoft Graph 中指定资源发生的更改属于请求的更改类型时接收更改通知。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

<span data-ttu-id="5d1e0-106">请参阅" [权限](#permissions) 部分中的表格，了解支持订阅以更改通知的资源列表。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d1e0-107">权限</span><span class="sxs-lookup"><span data-stu-id="5d1e0-107">Permissions</span></span>

<span data-ttu-id="5d1e0-108">创建订阅需要读取资源范围。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-108">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="5d1e0-109">例如，若要获取更改消息通知，应用需要 `Mail.Read` 权限。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-109">For example, to get change notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
<span data-ttu-id="5d1e0-110">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="5d1e0-111">若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-111">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5d1e0-112">支持的资源</span><span class="sxs-lookup"><span data-stu-id="5d1e0-112">Supported resource</span></span> | <span data-ttu-id="5d1e0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d1e0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5d1e0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d1e0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d1e0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d1e0-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="5d1e0-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="5d1e0-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="5d1e0-117">不支持</span><span class="sxs-lookup"><span data-stu-id="5d1e0-117">Not supported</span></span> | <span data-ttu-id="5d1e0-118">不支持</span><span class="sxs-lookup"><span data-stu-id="5d1e0-118">Not supported</span></span> | <span data-ttu-id="5d1e0-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d1e0-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="5d1e0-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="5d1e0-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="5d1e0-121">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d1e0-121">ChannelMessage.Read.All</span></span> | <span data-ttu-id="5d1e0-122">不支持</span><span class="sxs-lookup"><span data-stu-id="5d1e0-122">Not supported</span></span> |  <span data-ttu-id="5d1e0-123">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d1e0-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="5d1e0-124">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="5d1e0-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="5d1e0-125">不支持</span><span class="sxs-lookup"><span data-stu-id="5d1e0-125">Not supported</span></span> | <span data-ttu-id="5d1e0-126">不支持</span><span class="sxs-lookup"><span data-stu-id="5d1e0-126">Not supported</span></span> | <span data-ttu-id="5d1e0-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d1e0-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="5d1e0-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="5d1e0-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="5d1e0-129">不支持</span><span class="sxs-lookup"><span data-stu-id="5d1e0-129">Not supported</span></span> | <span data-ttu-id="5d1e0-130">不支持</span><span class="sxs-lookup"><span data-stu-id="5d1e0-130">Not supported</span></span> | <span data-ttu-id="5d1e0-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d1e0-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="5d1e0-132">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="5d1e0-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="5d1e0-133">不支持</span><span class="sxs-lookup"><span data-stu-id="5d1e0-133">Not supported</span></span> | <span data-ttu-id="5d1e0-134">不支持</span><span class="sxs-lookup"><span data-stu-id="5d1e0-134">Not supported</span></span> | <span data-ttu-id="5d1e0-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d1e0-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="5d1e0-136">contact</span><span class="sxs-lookup"><span data-stu-id="5d1e0-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="5d1e0-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5d1e0-137">Contacts.Read</span></span> | <span data-ttu-id="5d1e0-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5d1e0-138">Contacts.Read</span></span> | <span data-ttu-id="5d1e0-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5d1e0-139">Contacts.Read</span></span> |
|<span data-ttu-id="5d1e0-140">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="5d1e0-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="5d1e0-141">不支持</span><span class="sxs-lookup"><span data-stu-id="5d1e0-141">Not supported</span></span> | <span data-ttu-id="5d1e0-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d1e0-142">Files.ReadWrite</span></span> | <span data-ttu-id="5d1e0-143">不支持</span><span class="sxs-lookup"><span data-stu-id="5d1e0-143">Not supported</span></span> |
|<span data-ttu-id="5d1e0-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="5d1e0-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="5d1e0-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d1e0-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="5d1e0-146">不支持</span><span class="sxs-lookup"><span data-stu-id="5d1e0-146">Not supported</span></span> | <span data-ttu-id="5d1e0-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d1e0-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="5d1e0-148">事件</span><span class="sxs-lookup"><span data-stu-id="5d1e0-148">event</span></span>](../resources/event.md) | <span data-ttu-id="5d1e0-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5d1e0-149">Calendars.Read</span></span> | <span data-ttu-id="5d1e0-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5d1e0-150">Calendars.Read</span></span> | <span data-ttu-id="5d1e0-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5d1e0-151">Calendars.Read</span></span> |
|[<span data-ttu-id="5d1e0-152">组</span><span class="sxs-lookup"><span data-stu-id="5d1e0-152">group</span></span>](../resources/group.md) | <span data-ttu-id="5d1e0-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d1e0-153">Group.Read.All</span></span> | <span data-ttu-id="5d1e0-154">不支持</span><span class="sxs-lookup"><span data-stu-id="5d1e0-154">Not supported</span></span> | <span data-ttu-id="5d1e0-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d1e0-155">Group.Read.All</span></span> |
|[<span data-ttu-id="5d1e0-156">组对话</span><span class="sxs-lookup"><span data-stu-id="5d1e0-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="5d1e0-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d1e0-157">Group.Read.All</span></span> | <span data-ttu-id="5d1e0-158">不支持</span><span class="sxs-lookup"><span data-stu-id="5d1e0-158">Not supported</span></span> | <span data-ttu-id="5d1e0-159">不支持</span><span class="sxs-lookup"><span data-stu-id="5d1e0-159">Not supported</span></span> |
|[<span data-ttu-id="5d1e0-160">列表</span><span class="sxs-lookup"><span data-stu-id="5d1e0-160">list</span></span>](../resources/list.md) | <span data-ttu-id="5d1e0-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d1e0-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="5d1e0-162">不支持</span><span class="sxs-lookup"><span data-stu-id="5d1e0-162">Not supported</span></span> | <span data-ttu-id="5d1e0-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d1e0-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="5d1e0-164">邮件</span><span class="sxs-lookup"><span data-stu-id="5d1e0-164">message</span></span>](../resources/message.md) | <span data-ttu-id="5d1e0-165">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5d1e0-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="5d1e0-166">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5d1e0-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="5d1e0-167">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5d1e0-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="5d1e0-168">打印机</span><span class="sxs-lookup"><span data-stu-id="5d1e0-168">printer</span></span>](../resources/printer.md) | <span data-ttu-id="5d1e0-169">不支持</span><span class="sxs-lookup"><span data-stu-id="5d1e0-169">Not supported</span></span> | <span data-ttu-id="5d1e0-170">不支持</span><span class="sxs-lookup"><span data-stu-id="5d1e0-170">Not supported</span></span> | <span data-ttu-id="5d1e0-171">打印机。阅读.All，Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d1e0-171">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="5d1e0-172">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="5d1e0-172">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="5d1e0-173">不支持</span><span class="sxs-lookup"><span data-stu-id="5d1e0-173">Not supported</span></span> | <span data-ttu-id="5d1e0-174">不支持</span><span class="sxs-lookup"><span data-stu-id="5d1e0-174">Not supported</span></span> | <span data-ttu-id="5d1e0-175">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d1e0-175">PrintTaskDefinition.ReadWrite.All</span></span> |
|<span data-ttu-id="5d1e0-176">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="5d1e0-176">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="5d1e0-177">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d1e0-177">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="5d1e0-178">不支持</span><span class="sxs-lookup"><span data-stu-id="5d1e0-178">Not supported</span></span> | <span data-ttu-id="5d1e0-179">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d1e0-179">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="5d1e0-180">用户</span><span class="sxs-lookup"><span data-stu-id="5d1e0-180">user</span></span>](../resources/user.md) | <span data-ttu-id="5d1e0-181">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d1e0-181">User.Read.All</span></span> | <span data-ttu-id="5d1e0-182">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d1e0-182">User.Read.All</span></span> | <span data-ttu-id="5d1e0-183">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d1e0-183">User.Read.All</span></span> |

> <span data-ttu-id="5d1e0-184">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-184">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="5d1e0-185">driveItem</span><span class="sxs-lookup"><span data-stu-id="5d1e0-185">driveItem</span></span>

<span data-ttu-id="5d1e0-186">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-186">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="5d1e0-187">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-187">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="5d1e0-188">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-188">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="5d1e0-189">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-189">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="5d1e0-190">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-190">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="5d1e0-191">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-191">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="5d1e0-192">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="5d1e0-192">contact, event, and message</span></span>

<span data-ttu-id="5d1e0-193">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-193">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="5d1e0-194">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-194">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="5d1e0-195">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-195">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="5d1e0-196">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-196">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="5d1e0-197">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="5d1e0-197">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="5d1e0-198">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-198">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="5d1e0-199">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-199">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="5d1e0-200">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d1e0-200">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="5d1e0-201">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d1e0-201">Request headers</span></span>

| <span data-ttu-id="5d1e0-202">名称</span><span class="sxs-lookup"><span data-stu-id="5d1e0-202">Name</span></span>       | <span data-ttu-id="5d1e0-203">类型</span><span class="sxs-lookup"><span data-stu-id="5d1e0-203">Type</span></span> | <span data-ttu-id="5d1e0-204">说明</span><span class="sxs-lookup"><span data-stu-id="5d1e0-204">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5d1e0-205">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d1e0-205">Authorization</span></span>  | <span data-ttu-id="5d1e0-206">string</span><span class="sxs-lookup"><span data-stu-id="5d1e0-206">string</span></span>  | <span data-ttu-id="5d1e0-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5d1e0-209">响应</span><span class="sxs-lookup"><span data-stu-id="5d1e0-209">Response</span></span>

<span data-ttu-id="5d1e0-210">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-210">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>
<span data-ttu-id="5d1e0-211">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-211">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="5d1e0-212">示例</span><span class="sxs-lookup"><span data-stu-id="5d1e0-212">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5d1e0-213">请求</span><span class="sxs-lookup"><span data-stu-id="5d1e0-213">Request</span></span>

<span data-ttu-id="5d1e0-214">下面是在用户收到新邮件时请求发送更改通知的示例。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-214">Here is an example of the request to send a change notification when the user receives a new mail.</span></span>

# <a name="http"></a>[<span data-ttu-id="5d1e0-215">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d1e0-215">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5d1e0-216">C#</span><span class="sxs-lookup"><span data-stu-id="5d1e0-216">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d1e0-217">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d1e0-217">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d1e0-218">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d1e0-218">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d1e0-219">Java</span><span class="sxs-lookup"><span data-stu-id="5d1e0-219">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="5d1e0-220">在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-220">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="5d1e0-221">`clientState` 和 `latestSupportedTlsVersion` 是可选字段。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-221">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="5d1e0-222">资源示例</span><span class="sxs-lookup"><span data-stu-id="5d1e0-222">Resources examples</span></span>

<span data-ttu-id="5d1e0-223">订阅资源属性的有效值如下：</span><span class="sxs-lookup"><span data-stu-id="5d1e0-223">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="5d1e0-224">资源类型</span><span class="sxs-lookup"><span data-stu-id="5d1e0-224">Resource type</span></span> | <span data-ttu-id="5d1e0-225">示例</span><span class="sxs-lookup"><span data-stu-id="5d1e0-225">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="5d1e0-226">通话记录</span><span class="sxs-lookup"><span data-stu-id="5d1e0-226">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="5d1e0-227">聊天消息</span><span class="sxs-lookup"><span data-stu-id="5d1e0-227">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="5d1e0-228">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="5d1e0-228">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="5d1e0-229">联系人</span><span class="sxs-lookup"><span data-stu-id="5d1e0-229">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="5d1e0-230">对话</span><span class="sxs-lookup"><span data-stu-id="5d1e0-230">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="5d1e0-231">驱动器</span><span class="sxs-lookup"><span data-stu-id="5d1e0-231">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="5d1e0-232">事件</span><span class="sxs-lookup"><span data-stu-id="5d1e0-232">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="5d1e0-233">组</span><span class="sxs-lookup"><span data-stu-id="5d1e0-233">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="5d1e0-234">列表</span><span class="sxs-lookup"><span data-stu-id="5d1e0-234">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="5d1e0-235">邮件</span><span class="sxs-lookup"><span data-stu-id="5d1e0-235">Mail</span></span>](../resources/message.md)|<span data-ttu-id="5d1e0-236">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="5d1e0-236">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="5d1e0-237">打印机</span><span class="sxs-lookup"><span data-stu-id="5d1e0-237">printer</span></span>](../resources/printer.md) |`print/printers/{id}/jobs`|
|[<span data-ttu-id="5d1e0-238">PrintTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="5d1e0-238">PrintTaskDefinition</span></span>](../resources/printtaskdefinition.md)|`print/taskDefinitions/{id}/tasks`|
|[<span data-ttu-id="5d1e0-239">安全警报</span><span class="sxs-lookup"><span data-stu-id="5d1e0-239">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'New'`|
|[<span data-ttu-id="5d1e0-240">用户</span><span class="sxs-lookup"><span data-stu-id="5d1e0-240">Users</span></span>](../resources/user.md)|`users`|

> <span data-ttu-id="5d1e0-241">**注意：** 以 `me` 开头的任何路径也可与 `users/{id}`（而不是 `me`）一起使用，从而以特定用户为目标，而不是以当前用户为目标。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-241">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

##### <a name="response"></a><span data-ttu-id="5d1e0-242">响应</span><span class="sxs-lookup"><span data-stu-id="5d1e0-242">Response</span></span>

<span data-ttu-id="5d1e0-243">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-243">Here is an example of the response.</span></span> <span data-ttu-id="5d1e0-244">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-244">Note: The response object shown here might be shortened for readability.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="5d1e0-245">通知终结点验证</span><span class="sxs-lookup"><span data-stu-id="5d1e0-245">Notification endpoint validation</span></span>

<span data-ttu-id="5d1e0-246">通知终结点（于 `notificationUrl` 属性中指定）必须能够响应验证请求，如[设置用户数据更改的通知](/graph/webhooks#notification-endpoint-validation)中所述。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-246">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="5d1e0-247">如果验证失败，创建订阅请求返回错误“400 请求无效”。</span><span class="sxs-lookup"><span data-stu-id="5d1e0-247">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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

