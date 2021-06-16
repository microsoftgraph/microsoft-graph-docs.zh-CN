---
title: 删除订阅
description: 删除订阅。
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: d2692e1af87fd7449829ab646d14dd6c3d5a067a
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941485"
---
# <a name="delete-subscription"></a><span data-ttu-id="a75fb-103">删除订阅</span><span class="sxs-lookup"><span data-stu-id="a75fb-103">Delete subscription</span></span>

<span data-ttu-id="a75fb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a75fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a75fb-105">删除订阅。</span><span class="sxs-lookup"><span data-stu-id="a75fb-105">Delete a subscription.</span></span>

<span data-ttu-id="a75fb-106">请参阅" [权限](#permissions) 部分中的表格，了解支持订阅以更改通知的资源列表。</span><span class="sxs-lookup"><span data-stu-id="a75fb-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="a75fb-107">权限</span><span class="sxs-lookup"><span data-stu-id="a75fb-107">Permissions</span></span>

<span data-ttu-id="a75fb-108">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="a75fb-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="a75fb-109">若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a75fb-109">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a75fb-110">支持的资源</span><span class="sxs-lookup"><span data-stu-id="a75fb-110">Supported resource</span></span> | <span data-ttu-id="a75fb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a75fb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a75fb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a75fb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a75fb-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="a75fb-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="a75fb-114">callRecord</span><span class="sxs-lookup"><span data-stu-id="a75fb-114">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="a75fb-115">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-115">Not supported</span></span> | <span data-ttu-id="a75fb-116">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-116">Not supported</span></span> | <span data-ttu-id="a75fb-117">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-117">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="a75fb-118">[channels](../resources/channel.md) (/teams/getAllChannels – 组织中所有频道) </span><span class="sxs-lookup"><span data-stu-id="a75fb-118">[channels](../resources/channel.md) (/teams/getAllChannels – all channels in an organization)</span></span> | <span data-ttu-id="a75fb-119">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-119">Not supported</span></span>  | <span data-ttu-id="a75fb-120">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-120">Not supported</span></span> | <span data-ttu-id="a75fb-121">Channel.ReadBasic.All、ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-121">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span> |
|<span data-ttu-id="a75fb-122">[频道 (](../resources/channel.md) /teams/{id}/channels) </span><span class="sxs-lookup"><span data-stu-id="a75fb-122">[channels](../resources/channel.md) (/teams/{id}/channels)</span></span> | <span data-ttu-id="a75fb-123">Channel.ReadBasic.All、ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-123">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  | <span data-ttu-id="a75fb-124">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-124">Not supported</span></span> | <span data-ttu-id="a75fb-125">Channel.ReadBasic.All、ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-125">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  |
|<span data-ttu-id="a75fb-126">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="a75fb-126">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="a75fb-127">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-127">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="a75fb-128">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-128">Not supported</span></span> | <span data-ttu-id="a75fb-129">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-129">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="a75fb-130">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="a75fb-130">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="a75fb-131">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-131">Not supported</span></span> | <span data-ttu-id="a75fb-132">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-132">Not supported</span></span> | <span data-ttu-id="a75fb-133">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-133">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="a75fb-134">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="a75fb-134">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="a75fb-135">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a75fb-135">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="a75fb-136">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-136">Not supported</span></span> | <span data-ttu-id="a75fb-137">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-137">Chat.Read.All</span></span>  |
|<span data-ttu-id="a75fb-138">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="a75fb-138">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="a75fb-139">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-139">Not supported</span></span> | <span data-ttu-id="a75fb-140">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-140">Not supported</span></span> | <span data-ttu-id="a75fb-141">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-141">Chat.Read.All</span></span>  |
|[<span data-ttu-id="a75fb-142">contact</span><span class="sxs-lookup"><span data-stu-id="a75fb-142">contact</span></span>](../resources/contact.md) | <span data-ttu-id="a75fb-143">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a75fb-143">Contacts.Read</span></span> | <span data-ttu-id="a75fb-144">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a75fb-144">Contacts.Read</span></span> | <span data-ttu-id="a75fb-145">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a75fb-145">Contacts.Read</span></span> |
|<span data-ttu-id="a75fb-146">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members) </span><span class="sxs-lookup"><span data-stu-id="a75fb-146">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span></span> | <span data-ttu-id="a75fb-147">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-147">TeamMember.Read.All</span></span> | <span data-ttu-id="a75fb-148">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-148">Not supported</span></span> | <span data-ttu-id="a75fb-149">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-149">TeamMember.Read.All</span></span> |
|<span data-ttu-id="a75fb-150">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="a75fb-150">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="a75fb-151">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-151">Not supported</span></span> | <span data-ttu-id="a75fb-152">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a75fb-152">Files.ReadWrite</span></span> | <span data-ttu-id="a75fb-153">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-153">Not supported</span></span> |
|<span data-ttu-id="a75fb-154">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="a75fb-154">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="a75fb-155">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-155">Files.ReadWrite.All</span></span> | <span data-ttu-id="a75fb-156">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-156">Not supported</span></span> | <span data-ttu-id="a75fb-157">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-157">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="a75fb-158">事件</span><span class="sxs-lookup"><span data-stu-id="a75fb-158">event</span></span>](../resources/event.md) | <span data-ttu-id="a75fb-159">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a75fb-159">Calendars.Read</span></span> | <span data-ttu-id="a75fb-160">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a75fb-160">Calendars.Read</span></span> | <span data-ttu-id="a75fb-161">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a75fb-161">Calendars.Read</span></span> |
|[<span data-ttu-id="a75fb-162">组</span><span class="sxs-lookup"><span data-stu-id="a75fb-162">group</span></span>](../resources/group.md) | <span data-ttu-id="a75fb-163">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-163">Group.Read.All</span></span> | <span data-ttu-id="a75fb-164">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-164">Not supported</span></span> | <span data-ttu-id="a75fb-165">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-165">Group.Read.All</span></span> |
|[<span data-ttu-id="a75fb-166">组对话</span><span class="sxs-lookup"><span data-stu-id="a75fb-166">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="a75fb-167">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-167">Group.Read.All</span></span> | <span data-ttu-id="a75fb-168">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-168">Not supported</span></span> | <span data-ttu-id="a75fb-169">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-169">Not supported</span></span> |
|[<span data-ttu-id="a75fb-170">列表</span><span class="sxs-lookup"><span data-stu-id="a75fb-170">list</span></span>](../resources/list.md) | <span data-ttu-id="a75fb-171">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-171">Sites.ReadWrite.All</span></span> | <span data-ttu-id="a75fb-172">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-172">Not supported</span></span> | <span data-ttu-id="a75fb-173">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-173">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="a75fb-174">邮件</span><span class="sxs-lookup"><span data-stu-id="a75fb-174">message</span></span>](../resources/message.md) | <span data-ttu-id="a75fb-175">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a75fb-175">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="a75fb-176">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a75fb-176">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="a75fb-177">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a75fb-177">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="a75fb-178">状态</span><span class="sxs-lookup"><span data-stu-id="a75fb-178">presence</span></span>](../resources/presence.md) | <span data-ttu-id="a75fb-179">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-179">Presence.Read.All</span></span> | <span data-ttu-id="a75fb-180">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-180">Not supported</span></span> | <span data-ttu-id="a75fb-181">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-181">Not supported</span></span> |
|[<span data-ttu-id="a75fb-182">打印机</span><span class="sxs-lookup"><span data-stu-id="a75fb-182">printer</span></span>](../resources/printer.md) | <span data-ttu-id="a75fb-183">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-183">Not supported</span></span> | <span data-ttu-id="a75fb-184">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-184">Not supported</span></span> | <span data-ttu-id="a75fb-185">打印机。阅读.All，Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-185">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="a75fb-186">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="a75fb-186">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="a75fb-187">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-187">Not supported</span></span> | <span data-ttu-id="a75fb-188">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-188">Not supported</span></span> | <span data-ttu-id="a75fb-189">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-189">PrintTaskDefinition.ReadWrite.All</span></span> |
|<span data-ttu-id="a75fb-190">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="a75fb-190">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="a75fb-191">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-191">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="a75fb-192">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-192">Not supported</span></span> | <span data-ttu-id="a75fb-193">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-193">SecurityEvents.ReadWrite.All</span></span> |
|<span data-ttu-id="a75fb-194">[teams](../resources/team.md) (/teams – 组织内部的所有) </span><span class="sxs-lookup"><span data-stu-id="a75fb-194">[teams](../resources/team.md) (/teams – all teams in an organization)</span></span> | <span data-ttu-id="a75fb-195">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-195">Not supported</span></span> | <span data-ttu-id="a75fb-196">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-196">Not supported</span></span> | <span data-ttu-id="a75fb-197">Team.ReadBasic.All、TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-197">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|<span data-ttu-id="a75fb-198">[teams](../resources/team.md) (/teams/{id}) </span><span class="sxs-lookup"><span data-stu-id="a75fb-198">[teams](../resources/team.md) (/teams/{id})</span></span> | <span data-ttu-id="a75fb-199">Team.ReadBasic.All、TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-199">Team.ReadBasic.All, TeamSettings.Read.All</span></span> | <span data-ttu-id="a75fb-200">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-200">Not supported</span></span> | <span data-ttu-id="a75fb-201">Team.ReadBasic.All、TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-201">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|[<span data-ttu-id="a75fb-202">todoTask</span><span class="sxs-lookup"><span data-stu-id="a75fb-202">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="a75fb-203">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a75fb-203">Tasks.ReadWrite</span></span> | <span data-ttu-id="a75fb-204">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a75fb-204">Tasks.ReadWrite</span></span> | <span data-ttu-id="a75fb-205">不支持</span><span class="sxs-lookup"><span data-stu-id="a75fb-205">Not supported</span></span> |
|[<span data-ttu-id="a75fb-206">用户</span><span class="sxs-lookup"><span data-stu-id="a75fb-206">user</span></span>](../resources/user.md) | <span data-ttu-id="a75fb-207">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-207">User.Read.All</span></span> | <span data-ttu-id="a75fb-208">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-208">User.Read.All</span></span> | <span data-ttu-id="a75fb-209">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a75fb-209">User.Read.All</span></span> |

> <span data-ttu-id="a75fb-210">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="a75fb-210">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="a75fb-211">driveItem</span><span class="sxs-lookup"><span data-stu-id="a75fb-211">driveItem</span></span>

<span data-ttu-id="a75fb-212">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="a75fb-212">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="a75fb-213">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="a75fb-213">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="a75fb-214">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="a75fb-214">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="a75fb-215">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="a75fb-215">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="a75fb-216">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="a75fb-216">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="a75fb-217">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="a75fb-217">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="a75fb-218">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="a75fb-218">contact, event, and message</span></span>

<span data-ttu-id="a75fb-219">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="a75fb-219">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="a75fb-220">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="a75fb-220">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="a75fb-221">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="a75fb-221">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="a75fb-222">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="a75fb-222">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="a75fb-223">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="a75fb-223">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="a75fb-224">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="a75fb-224">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="a75fb-225">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="a75fb-225">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="a75fb-226">状态</span><span class="sxs-lookup"><span data-stu-id="a75fb-226">presence</span></span>

<span data-ttu-id="a75fb-227">**状态** 订阅需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="a75fb-227">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="a75fb-228">如果未指定 [encryptionCertificate](../resources/subscription.md)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="a75fb-228">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="a75fb-229">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a75fb-229">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="a75fb-230">请求标头</span><span class="sxs-lookup"><span data-stu-id="a75fb-230">Request headers</span></span>

| <span data-ttu-id="a75fb-231">名称</span><span class="sxs-lookup"><span data-stu-id="a75fb-231">Name</span></span>       | <span data-ttu-id="a75fb-232">类型</span><span class="sxs-lookup"><span data-stu-id="a75fb-232">Type</span></span> | <span data-ttu-id="a75fb-233">说明</span><span class="sxs-lookup"><span data-stu-id="a75fb-233">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a75fb-234">Authorization</span><span class="sxs-lookup"><span data-stu-id="a75fb-234">Authorization</span></span>  | <span data-ttu-id="a75fb-235">string</span><span class="sxs-lookup"><span data-stu-id="a75fb-235">string</span></span>  | <span data-ttu-id="a75fb-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a75fb-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a75fb-238">请求正文</span><span class="sxs-lookup"><span data-stu-id="a75fb-238">Request body</span></span>

<span data-ttu-id="a75fb-239">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a75fb-239">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a75fb-240">响应</span><span class="sxs-lookup"><span data-stu-id="a75fb-240">Response</span></span>

<span data-ttu-id="a75fb-241">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a75fb-241">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="a75fb-242">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="a75fb-242">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="a75fb-243">示例</span><span class="sxs-lookup"><span data-stu-id="a75fb-243">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a75fb-244">请求</span><span class="sxs-lookup"><span data-stu-id="a75fb-244">Request</span></span>

<span data-ttu-id="a75fb-245">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a75fb-245">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a75fb-246">HTTP</span><span class="sxs-lookup"><span data-stu-id="a75fb-246">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="a75fb-247">C#</span><span class="sxs-lookup"><span data-stu-id="a75fb-247">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a75fb-248">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a75fb-248">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a75fb-249">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a75fb-249">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a75fb-250">Java</span><span class="sxs-lookup"><span data-stu-id="a75fb-250">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a75fb-251">响应</span><span class="sxs-lookup"><span data-stu-id="a75fb-251">Response</span></span>

<span data-ttu-id="a75fb-252">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a75fb-252">Here is an example of the response.</span></span>
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


