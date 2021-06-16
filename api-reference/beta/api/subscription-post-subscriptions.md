---
title: 创建订阅
description: 订阅侦听器应用程序，以在 Microsoft 数据或资源发生更改时Graph更改通知。
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: f87f448e4a1dfc2544eb229e16bb674ba3627e26
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941499"
---
# <a name="create-subscription"></a><span data-ttu-id="8b4fa-103">创建订阅</span><span class="sxs-lookup"><span data-stu-id="8b4fa-103">Create subscription</span></span>

<span data-ttu-id="8b4fa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b4fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b4fa-105">订阅侦听器应用程序，以在 Microsoft Graph 中指定资源发生的更改属于请求的更改类型时接收更改通知。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

<span data-ttu-id="8b4fa-106">请参阅" [权限](#permissions) 部分中的表格，了解支持订阅以更改通知的资源列表。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b4fa-107">权限</span><span class="sxs-lookup"><span data-stu-id="8b4fa-107">Permissions</span></span>

<span data-ttu-id="8b4fa-108">创建订阅需要对资源的读取权限。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-108">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="8b4fa-109">例如，若要获取邮件更改通知，您的应用程序需要 Mail.Read 权限。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-109">For example, to get change notifications on messages, your app needs the Mail.Read permission.</span></span> 

<span data-ttu-id="8b4fa-110">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="8b4fa-111">若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-111">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b4fa-112">支持的资源</span><span class="sxs-lookup"><span data-stu-id="8b4fa-112">Supported resource</span></span> | <span data-ttu-id="8b4fa-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8b4fa-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8b4fa-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8b4fa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b4fa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8b4fa-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="8b4fa-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="8b4fa-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="8b4fa-117">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-117">Not supported</span></span> | <span data-ttu-id="8b4fa-118">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-118">Not supported</span></span> | <span data-ttu-id="8b4fa-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="8b4fa-120">[channels](../resources/channel.md) (/teams/getAllChannels – 组织中所有频道) </span><span class="sxs-lookup"><span data-stu-id="8b4fa-120">[channels](../resources/channel.md) (/teams/getAllChannels – all channels in an organization)</span></span> | <span data-ttu-id="8b4fa-121">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-121">Not supported</span></span>  | <span data-ttu-id="8b4fa-122">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-122">Not supported</span></span> | <span data-ttu-id="8b4fa-123">Channel.ReadBasic.All、ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-123">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span> |
|<span data-ttu-id="8b4fa-124">[频道 (](../resources/channel.md) /teams/{id}/channels) </span><span class="sxs-lookup"><span data-stu-id="8b4fa-124">[channels](../resources/channel.md) (/teams/{id}/channels)</span></span> | <span data-ttu-id="8b4fa-125">Channel.ReadBasic.All、ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-125">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  | <span data-ttu-id="8b4fa-126">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-126">Not supported</span></span> | <span data-ttu-id="8b4fa-127">Channel.ReadBasic.All、ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-127">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  |
|<span data-ttu-id="8b4fa-128">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="8b4fa-128">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="8b4fa-129">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-129">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="8b4fa-130">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-130">Not supported</span></span> | <span data-ttu-id="8b4fa-131">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-131">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="8b4fa-132">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="8b4fa-132">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="8b4fa-133">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-133">Not supported</span></span> | <span data-ttu-id="8b4fa-134">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-134">Not supported</span></span> | <span data-ttu-id="8b4fa-135">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-135">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="8b4fa-136">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="8b4fa-136">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="8b4fa-137">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b4fa-137">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="8b4fa-138">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-138">Not supported</span></span> | <span data-ttu-id="8b4fa-139">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-139">Chat.Read.All</span></span>  |
|<span data-ttu-id="8b4fa-140">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="8b4fa-140">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="8b4fa-141">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-141">Not supported</span></span> | <span data-ttu-id="8b4fa-142">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-142">Not supported</span></span> | <span data-ttu-id="8b4fa-143">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-143">Chat.Read.All</span></span>  |
|[<span data-ttu-id="8b4fa-144">contact</span><span class="sxs-lookup"><span data-stu-id="8b4fa-144">contact</span></span>](../resources/contact.md) | <span data-ttu-id="8b4fa-145">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8b4fa-145">Contacts.Read</span></span> | <span data-ttu-id="8b4fa-146">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8b4fa-146">Contacts.Read</span></span> | <span data-ttu-id="8b4fa-147">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8b4fa-147">Contacts.Read</span></span> |
|<span data-ttu-id="8b4fa-148">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members) </span><span class="sxs-lookup"><span data-stu-id="8b4fa-148">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span></span> | <span data-ttu-id="8b4fa-149">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-149">TeamMember.Read.All</span></span> | <span data-ttu-id="8b4fa-150">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-150">Not supported</span></span> | <span data-ttu-id="8b4fa-151">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-151">TeamMember.Read.All</span></span> |
|<span data-ttu-id="8b4fa-152">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="8b4fa-152">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="8b4fa-153">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-153">Not supported</span></span> | <span data-ttu-id="8b4fa-154">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b4fa-154">Files.ReadWrite</span></span> | <span data-ttu-id="8b4fa-155">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-155">Not supported</span></span> |
|<span data-ttu-id="8b4fa-156">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="8b4fa-156">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="8b4fa-157">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-157">Files.ReadWrite.All</span></span> | <span data-ttu-id="8b4fa-158">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-158">Not supported</span></span> | <span data-ttu-id="8b4fa-159">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-159">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="8b4fa-160">事件</span><span class="sxs-lookup"><span data-stu-id="8b4fa-160">event</span></span>](../resources/event.md) | <span data-ttu-id="8b4fa-161">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8b4fa-161">Calendars.Read</span></span> | <span data-ttu-id="8b4fa-162">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8b4fa-162">Calendars.Read</span></span> | <span data-ttu-id="8b4fa-163">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8b4fa-163">Calendars.Read</span></span> |
|[<span data-ttu-id="8b4fa-164">组</span><span class="sxs-lookup"><span data-stu-id="8b4fa-164">group</span></span>](../resources/group.md) | <span data-ttu-id="8b4fa-165">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-165">Group.Read.All</span></span> | <span data-ttu-id="8b4fa-166">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-166">Not supported</span></span> | <span data-ttu-id="8b4fa-167">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-167">Group.Read.All</span></span> |
|[<span data-ttu-id="8b4fa-168">组对话</span><span class="sxs-lookup"><span data-stu-id="8b4fa-168">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="8b4fa-169">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-169">Group.Read.All</span></span> | <span data-ttu-id="8b4fa-170">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-170">Not supported</span></span> | <span data-ttu-id="8b4fa-171">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-171">Not supported</span></span> |
|[<span data-ttu-id="8b4fa-172">列表</span><span class="sxs-lookup"><span data-stu-id="8b4fa-172">list</span></span>](../resources/list.md) | <span data-ttu-id="8b4fa-173">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-173">Sites.ReadWrite.All</span></span> | <span data-ttu-id="8b4fa-174">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-174">Not supported</span></span> | <span data-ttu-id="8b4fa-175">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-175">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="8b4fa-176">邮件</span><span class="sxs-lookup"><span data-stu-id="8b4fa-176">message</span></span>](../resources/message.md) | <span data-ttu-id="8b4fa-177">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8b4fa-177">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="8b4fa-178">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8b4fa-178">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="8b4fa-179">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8b4fa-179">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="8b4fa-180">状态</span><span class="sxs-lookup"><span data-stu-id="8b4fa-180">presence</span></span>](../resources/presence.md) | <span data-ttu-id="8b4fa-181">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-181">Presence.Read.All</span></span> | <span data-ttu-id="8b4fa-182">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-182">Not supported</span></span> | <span data-ttu-id="8b4fa-183">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-183">Not supported</span></span> |
|[<span data-ttu-id="8b4fa-184">打印机</span><span class="sxs-lookup"><span data-stu-id="8b4fa-184">printer</span></span>](../resources/printer.md) | <span data-ttu-id="8b4fa-185">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-185">Not supported</span></span> | <span data-ttu-id="8b4fa-186">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-186">Not supported</span></span> | <span data-ttu-id="8b4fa-187">打印机。阅读.All，Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-187">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="8b4fa-188">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="8b4fa-188">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="8b4fa-189">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-189">Not supported</span></span> | <span data-ttu-id="8b4fa-190">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-190">Not supported</span></span> | <span data-ttu-id="8b4fa-191">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-191">PrintTaskDefinition.ReadWrite.All</span></span> |
|<span data-ttu-id="8b4fa-192">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="8b4fa-192">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="8b4fa-193">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-193">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="8b4fa-194">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-194">Not supported</span></span> | <span data-ttu-id="8b4fa-195">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-195">SecurityEvents.ReadWrite.All</span></span> |
|<span data-ttu-id="8b4fa-196">[teams](../resources/team.md) (/teams – 组织内部的所有) </span><span class="sxs-lookup"><span data-stu-id="8b4fa-196">[teams](../resources/team.md) (/teams – all teams in an organization)</span></span> | <span data-ttu-id="8b4fa-197">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-197">Not supported</span></span> | <span data-ttu-id="8b4fa-198">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-198">Not supported</span></span> | <span data-ttu-id="8b4fa-199">Team.ReadBasic.All、TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-199">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|<span data-ttu-id="8b4fa-200">[teams](../resources/team.md) (/teams/{id}) </span><span class="sxs-lookup"><span data-stu-id="8b4fa-200">[teams](../resources/team.md) (/teams/{id})</span></span> | <span data-ttu-id="8b4fa-201">Team.ReadBasic.All、TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-201">Team.ReadBasic.All, TeamSettings.Read.All</span></span> | <span data-ttu-id="8b4fa-202">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-202">Not supported</span></span> | <span data-ttu-id="8b4fa-203">Team.ReadBasic.All、TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-203">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|[<span data-ttu-id="8b4fa-204">todoTask</span><span class="sxs-lookup"><span data-stu-id="8b4fa-204">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="8b4fa-205">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b4fa-205">Tasks.ReadWrite</span></span> | <span data-ttu-id="8b4fa-206">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b4fa-206">Tasks.ReadWrite</span></span> | <span data-ttu-id="8b4fa-207">不支持</span><span class="sxs-lookup"><span data-stu-id="8b4fa-207">Not supported</span></span> |
|[<span data-ttu-id="8b4fa-208">用户</span><span class="sxs-lookup"><span data-stu-id="8b4fa-208">user</span></span>](../resources/user.md) | <span data-ttu-id="8b4fa-209">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-209">User.Read.All</span></span> | <span data-ttu-id="8b4fa-210">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-210">User.Read.All</span></span> | <span data-ttu-id="8b4fa-211">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b4fa-211">User.Read.All</span></span> |

> <span data-ttu-id="8b4fa-212">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-212">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="8b4fa-213">driveItem</span><span class="sxs-lookup"><span data-stu-id="8b4fa-213">driveItem</span></span>

<span data-ttu-id="8b4fa-214">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-214">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="8b4fa-215">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-215">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="8b4fa-216">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-216">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="8b4fa-217">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-217">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="8b4fa-218">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-218">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="8b4fa-219">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-219">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

<span data-ttu-id="8b4fa-220">OneDrive for Business 和 SharePoint 支持发送 **driveItem** 上发生的安全事件的应用程序通知。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-220">OneDrive for Business and SharePoint support sending your application notifications of security events that occur on a **driveItem**.</span></span> <span data-ttu-id="8b4fa-221">若要订阅这些事件，请向 `prefer:includesecuritywebhooks` 请求中添加 标头以创建订阅。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-221">To subscribe to these events, add the `prefer:includesecuritywebhooks` header to your request to create a subscription.</span></span> <span data-ttu-id="8b4fa-222">创建订阅后，当项目权限更改时，您将收到通知。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-222">After the subscription is created, you will receive notifications when the permissions on an item change.</span></span> <span data-ttu-id="8b4fa-223">此标头适用于用户帐户SharePoint OneDrive for Business但不适用于使用者OneDrive帐户。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-223">This header is applicable to SharePoint and OneDrive for Business but not consumer OneDrive accounts.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="8b4fa-224">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="8b4fa-224">contact, event, and message</span></span>

<span data-ttu-id="8b4fa-225">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-225">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="8b4fa-226">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-226">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="8b4fa-227">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-227">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="8b4fa-228">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-228">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="8b4fa-229">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="8b4fa-229">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="8b4fa-230">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-230">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="8b4fa-231">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-231">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="8b4fa-232">状态</span><span class="sxs-lookup"><span data-stu-id="8b4fa-232">presence</span></span>

<span data-ttu-id="8b4fa-233">**状态** 订阅需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-233">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="8b4fa-234">如果未指定 [encryptionCertificate](../resources/subscription.md)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-234">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="8b4fa-235">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8b4fa-235">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="8b4fa-236">请求标头</span><span class="sxs-lookup"><span data-stu-id="8b4fa-236">Request headers</span></span>

| <span data-ttu-id="8b4fa-237">名称</span><span class="sxs-lookup"><span data-stu-id="8b4fa-237">Name</span></span>       | <span data-ttu-id="8b4fa-238">类型</span><span class="sxs-lookup"><span data-stu-id="8b4fa-238">Type</span></span> | <span data-ttu-id="8b4fa-239">说明</span><span class="sxs-lookup"><span data-stu-id="8b4fa-239">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8b4fa-240">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b4fa-240">Authorization</span></span>  | <span data-ttu-id="8b4fa-241">string</span><span class="sxs-lookup"><span data-stu-id="8b4fa-241">string</span></span>  | <span data-ttu-id="8b4fa-p109">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-p109">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8b4fa-244">响应</span><span class="sxs-lookup"><span data-stu-id="8b4fa-244">Response</span></span>

<span data-ttu-id="8b4fa-245">如果成功，此方法在响应 `201 Created` 正文中返回 [响应](../resources/subscription.md) 代码和 subscription 对象。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-245">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="8b4fa-246">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-246">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="8b4fa-247">示例</span><span class="sxs-lookup"><span data-stu-id="8b4fa-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b4fa-248">请求</span><span class="sxs-lookup"><span data-stu-id="8b4fa-248">Request</span></span>

<span data-ttu-id="8b4fa-249">在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-249">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="8b4fa-250">`clientState` 和 `latestSupportedTlsVersion` 是可选字段。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-250">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="8b4fa-251">此请求为当前登录用户收到的新邮件更改通知创建订阅。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-251">This request creates a subscription for change notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="8b4fa-252">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b4fa-252">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8b4fa-253">C#</span><span class="sxs-lookup"><span data-stu-id="8b4fa-253">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b4fa-254">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b4fa-254">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b4fa-255">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b4fa-255">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b4fa-256">Java</span><span class="sxs-lookup"><span data-stu-id="8b4fa-256">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="8b4fa-257">在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-257">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="8b4fa-258">`clientState` 和 `latestSupportedTlsVersion` 是可选字段。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-258">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

#### <a name="resources-examples"></a><span data-ttu-id="8b4fa-259">资源示例</span><span class="sxs-lookup"><span data-stu-id="8b4fa-259">Resources examples</span></span>

<span data-ttu-id="8b4fa-260">以下是资源属性的有效值。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-260">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="8b4fa-261">资源类型</span><span class="sxs-lookup"><span data-stu-id="8b4fa-261">Resource type</span></span> | <span data-ttu-id="8b4fa-262">示例</span><span class="sxs-lookup"><span data-stu-id="8b4fa-262">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="8b4fa-263">通话记录</span><span class="sxs-lookup"><span data-stu-id="8b4fa-263">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="8b4fa-264">频道</span><span class="sxs-lookup"><span data-stu-id="8b4fa-264">Channels</span></span>](../resources/channel.md)|<span data-ttu-id="8b4fa-265">`/teams/getAllChannels`, `/teams/{id}/channels`</span><span class="sxs-lookup"><span data-stu-id="8b4fa-265">`/teams/getAllChannels`, `/teams/{id}/channels`</span></span>|
|[<span data-ttu-id="8b4fa-266">聊天消息</span><span class="sxs-lookup"><span data-stu-id="8b4fa-266">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="8b4fa-267">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="8b4fa-267">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="8b4fa-268">联系人</span><span class="sxs-lookup"><span data-stu-id="8b4fa-268">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="8b4fa-269">ConversationMember</span><span class="sxs-lookup"><span data-stu-id="8b4fa-269">ConversationMember</span></span>](../resources/conversationmember.md)|`/teams/{id}/members`|
|[<span data-ttu-id="8b4fa-270">对话</span><span class="sxs-lookup"><span data-stu-id="8b4fa-270">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="8b4fa-271">驱动器</span><span class="sxs-lookup"><span data-stu-id="8b4fa-271">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="8b4fa-272">事件</span><span class="sxs-lookup"><span data-stu-id="8b4fa-272">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="8b4fa-273">组</span><span class="sxs-lookup"><span data-stu-id="8b4fa-273">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="8b4fa-274">列表</span><span class="sxs-lookup"><span data-stu-id="8b4fa-274">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="8b4fa-275">邮件</span><span class="sxs-lookup"><span data-stu-id="8b4fa-275">Mail</span></span>](../resources/message.md)|<span data-ttu-id="8b4fa-276">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="8b4fa-276">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="8b4fa-277">状态</span><span class="sxs-lookup"><span data-stu-id="8b4fa-277">Presence</span></span>](../resources/presence.md)| <span data-ttu-id="8b4fa-278">`/communications/presences/{id}` (单个用户) ， (`/communications/presences?$filter=id in ({id},{id}…)` 多个) </span><span class="sxs-lookup"><span data-stu-id="8b4fa-278">`/communications/presences/{id}` (single user), `/communications/presences?$filter=id in ({id},{id}…)` (multiple users)</span></span>|
|[<span data-ttu-id="8b4fa-279">打印机</span><span class="sxs-lookup"><span data-stu-id="8b4fa-279">printer</span></span>](../resources/printer.md) |`print/printers/{id}/jobs`|
|[<span data-ttu-id="8b4fa-280">PrintTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="8b4fa-280">PrintTaskDefinition</span></span>](../resources/printtaskdefinition.md)|`print/taskDefinitions/{id}/tasks`|
|[<span data-ttu-id="8b4fa-281">Teams</span><span class="sxs-lookup"><span data-stu-id="8b4fa-281">Teams</span></span>](../resources/team.md)|<span data-ttu-id="8b4fa-282">`/teams`, `/teams/{id}`</span><span class="sxs-lookup"><span data-stu-id="8b4fa-282">`/teams`, `/teams/{id}`</span></span>|
|[<span data-ttu-id="8b4fa-283">用户</span><span class="sxs-lookup"><span data-stu-id="8b4fa-283">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="8b4fa-284">todoTask</span><span class="sxs-lookup"><span data-stu-id="8b4fa-284">todoTask</span></span>](../resources/todotask.md) | `/me/todo/lists/{todoTaskListId}/tasks`
|[<span data-ttu-id="8b4fa-285">安全警报</span><span class="sxs-lookup"><span data-stu-id="8b4fa-285">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'NewAlert'`|

> <span data-ttu-id="8b4fa-286">**注意：** 以 `me` 开头的任何路径也可与 `users/{id}`（而不是 `me`）一起使用，从而以特定用户为目标，而不是以当前用户为目标。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-286">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

### <a name="response"></a><span data-ttu-id="8b4fa-287">响应</span><span class="sxs-lookup"><span data-stu-id="8b4fa-287">Response</span></span>

<span data-ttu-id="8b4fa-288">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-288">The following example shows the response.</span></span> 

><span data-ttu-id="8b4fa-289">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-289">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "latestSupportedTlsVersion": "v1_2",
  "notificationContentType": "application/json"
}
```

### <a name="notification-endpoint-validation"></a><span data-ttu-id="8b4fa-290">通知终结点验证</span><span class="sxs-lookup"><span data-stu-id="8b4fa-290">Notification endpoint validation</span></span>

<span data-ttu-id="8b4fa-291">notificationUrl (中指定的订阅通知终结点) 必须能够响应验证请求，如设置用户数据更改[的通知中所述](/graph/webhooks#notification-endpoint-validation)。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-291">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="8b4fa-292">如果验证失败，创建订阅请求返回错误“400 请求无效”。</span><span class="sxs-lookup"><span data-stu-id="8b4fa-292">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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


