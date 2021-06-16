---
title: 获取订阅
description: 检索订阅的属性和关系。
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 03e1f8fe519f544537eb09bcd6948e23cc325c7e
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941478"
---
# <a name="get-subscription"></a><span data-ttu-id="75a77-103">获取订阅</span><span class="sxs-lookup"><span data-stu-id="75a77-103">Get subscription</span></span>

<span data-ttu-id="75a77-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75a77-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75a77-105">检索订阅的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="75a77-105">Retrieve the properties and relationships of a subscription.</span></span>

<span data-ttu-id="75a77-106">请参阅" [权限](#permissions) 部分中的表格，了解支持订阅以更改通知的资源列表。</span><span class="sxs-lookup"><span data-stu-id="75a77-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="75a77-107">权限</span><span class="sxs-lookup"><span data-stu-id="75a77-107">Permissions</span></span>

<span data-ttu-id="75a77-108">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="75a77-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="75a77-109">若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="75a77-109">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="75a77-110">支持的资源</span><span class="sxs-lookup"><span data-stu-id="75a77-110">Supported resource</span></span> | <span data-ttu-id="75a77-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="75a77-111">Delegated (work or school account)</span></span> | <span data-ttu-id="75a77-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="75a77-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75a77-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="75a77-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="75a77-114">callRecord</span><span class="sxs-lookup"><span data-stu-id="75a77-114">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="75a77-115">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-115">Not supported</span></span> | <span data-ttu-id="75a77-116">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-116">Not supported</span></span> | <span data-ttu-id="75a77-117">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="75a77-117">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="75a77-118">[channels](../resources/channel.md) (/teams/getAllChannels – 组织中所有频道) </span><span class="sxs-lookup"><span data-stu-id="75a77-118">[channels](../resources/channel.md) (/teams/getAllChannels – all channels in an organization)</span></span> | <span data-ttu-id="75a77-119">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-119">Not supported</span></span>  | <span data-ttu-id="75a77-120">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-120">Not supported</span></span> | <span data-ttu-id="75a77-121">Channel.ReadBasic.All，ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="75a77-121">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span> |
|<span data-ttu-id="75a77-122">[频道 (](../resources/channel.md) /teams/{id}/channels) </span><span class="sxs-lookup"><span data-stu-id="75a77-122">[channels](../resources/channel.md) (/teams/{id}/channels)</span></span> | <span data-ttu-id="75a77-123">Channel.ReadBasic.All，ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="75a77-123">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  | <span data-ttu-id="75a77-124">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-124">Not supported</span></span> | <span data-ttu-id="75a77-125">Channel.ReadBasic.All，ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="75a77-125">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  |
|<span data-ttu-id="75a77-126">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="75a77-126">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="75a77-127">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75a77-127">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="75a77-128">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-128">Not supported</span></span> | <span data-ttu-id="75a77-129">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="75a77-129">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="75a77-130">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="75a77-130">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="75a77-131">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-131">Not supported</span></span> | <span data-ttu-id="75a77-132">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-132">Not supported</span></span> | <span data-ttu-id="75a77-133">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="75a77-133">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="75a77-134">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="75a77-134">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="75a77-135">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75a77-135">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="75a77-136">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-136">Not supported</span></span> | <span data-ttu-id="75a77-137">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="75a77-137">Chat.Read.All</span></span>  |
|<span data-ttu-id="75a77-138">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="75a77-138">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="75a77-139">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-139">Not supported</span></span> | <span data-ttu-id="75a77-140">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-140">Not supported</span></span> | <span data-ttu-id="75a77-141">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="75a77-141">Chat.Read.All</span></span>  |
|[<span data-ttu-id="75a77-142">contact</span><span class="sxs-lookup"><span data-stu-id="75a77-142">contact</span></span>](../resources/contact.md) | <span data-ttu-id="75a77-143">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="75a77-143">Contacts.Read</span></span> | <span data-ttu-id="75a77-144">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="75a77-144">Contacts.Read</span></span> | <span data-ttu-id="75a77-145">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="75a77-145">Contacts.Read</span></span> |
|<span data-ttu-id="75a77-146">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members) </span><span class="sxs-lookup"><span data-stu-id="75a77-146">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span></span> | <span data-ttu-id="75a77-147">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="75a77-147">TeamMember.Read.All</span></span> | <span data-ttu-id="75a77-148">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-148">Not supported</span></span> | <span data-ttu-id="75a77-149">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="75a77-149">TeamMember.Read.All</span></span> |
|<span data-ttu-id="75a77-150">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="75a77-150">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="75a77-151">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-151">Not supported</span></span> | <span data-ttu-id="75a77-152">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75a77-152">Files.ReadWrite</span></span> | <span data-ttu-id="75a77-153">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-153">Not supported</span></span> |
|<span data-ttu-id="75a77-154">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="75a77-154">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="75a77-155">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75a77-155">Files.ReadWrite.All</span></span> | <span data-ttu-id="75a77-156">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-156">Not supported</span></span> | <span data-ttu-id="75a77-157">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75a77-157">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="75a77-158">事件</span><span class="sxs-lookup"><span data-stu-id="75a77-158">event</span></span>](../resources/event.md) | <span data-ttu-id="75a77-159">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="75a77-159">Calendars.Read</span></span> | <span data-ttu-id="75a77-160">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="75a77-160">Calendars.Read</span></span> | <span data-ttu-id="75a77-161">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="75a77-161">Calendars.Read</span></span> |
|[<span data-ttu-id="75a77-162">组</span><span class="sxs-lookup"><span data-stu-id="75a77-162">group</span></span>](../resources/group.md) | <span data-ttu-id="75a77-163">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="75a77-163">Group.Read.All</span></span> | <span data-ttu-id="75a77-164">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-164">Not supported</span></span> | <span data-ttu-id="75a77-165">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="75a77-165">Group.Read.All</span></span> |
|[<span data-ttu-id="75a77-166">组对话</span><span class="sxs-lookup"><span data-stu-id="75a77-166">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="75a77-167">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="75a77-167">Group.Read.All</span></span> | <span data-ttu-id="75a77-168">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-168">Not supported</span></span> | <span data-ttu-id="75a77-169">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-169">Not supported</span></span> |
|[<span data-ttu-id="75a77-170">列表</span><span class="sxs-lookup"><span data-stu-id="75a77-170">list</span></span>](../resources/list.md) | <span data-ttu-id="75a77-171">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75a77-171">Sites.ReadWrite.All</span></span> | <span data-ttu-id="75a77-172">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-172">Not supported</span></span> | <span data-ttu-id="75a77-173">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75a77-173">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="75a77-174">邮件</span><span class="sxs-lookup"><span data-stu-id="75a77-174">message</span></span>](../resources/message.md) | <span data-ttu-id="75a77-175">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="75a77-175">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="75a77-176">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="75a77-176">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="75a77-177">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="75a77-177">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="75a77-178">状态</span><span class="sxs-lookup"><span data-stu-id="75a77-178">presence</span></span>](../resources/presence.md) | <span data-ttu-id="75a77-179">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="75a77-179">Presence.Read.All</span></span> | <span data-ttu-id="75a77-180">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-180">Not supported</span></span> | <span data-ttu-id="75a77-181">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-181">Not supported</span></span> |
|[<span data-ttu-id="75a77-182">打印机</span><span class="sxs-lookup"><span data-stu-id="75a77-182">printer</span></span>](../resources/printer.md) | <span data-ttu-id="75a77-183">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-183">Not supported</span></span> | <span data-ttu-id="75a77-184">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-184">Not supported</span></span> | <span data-ttu-id="75a77-185">打印机。阅读.All，Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75a77-185">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="75a77-186">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="75a77-186">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="75a77-187">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-187">Not supported</span></span> | <span data-ttu-id="75a77-188">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-188">Not supported</span></span> | <span data-ttu-id="75a77-189">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75a77-189">PrintTaskDefinition.ReadWrite.All</span></span> |
|<span data-ttu-id="75a77-190">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="75a77-190">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="75a77-191">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75a77-191">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="75a77-192">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-192">Not supported</span></span> | <span data-ttu-id="75a77-193">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75a77-193">SecurityEvents.ReadWrite.All</span></span> |
|<span data-ttu-id="75a77-194">[teams](../resources/team.md) (/teams – 组织内部的所有) </span><span class="sxs-lookup"><span data-stu-id="75a77-194">[teams](../resources/team.md) (/teams – all teams in an organization)</span></span> | <span data-ttu-id="75a77-195">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-195">Not supported</span></span> | <span data-ttu-id="75a77-196">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-196">Not supported</span></span> | <span data-ttu-id="75a77-197">Team.ReadBasic.All，TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="75a77-197">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|<span data-ttu-id="75a77-198">[teams](../resources/team.md) (/teams/{id}) </span><span class="sxs-lookup"><span data-stu-id="75a77-198">[teams](../resources/team.md) (/teams/{id})</span></span> | <span data-ttu-id="75a77-199">Team.ReadBasic.All，TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="75a77-199">Team.ReadBasic.All, TeamSettings.Read.All</span></span> | <span data-ttu-id="75a77-200">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-200">Not supported</span></span> | <span data-ttu-id="75a77-201">Team.ReadBasic.All，TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="75a77-201">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|[<span data-ttu-id="75a77-202">todoTask</span><span class="sxs-lookup"><span data-stu-id="75a77-202">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="75a77-203">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75a77-203">Tasks.ReadWrite</span></span> | <span data-ttu-id="75a77-204">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75a77-204">Tasks.ReadWrite</span></span> | <span data-ttu-id="75a77-205">不支持</span><span class="sxs-lookup"><span data-stu-id="75a77-205">Not supported</span></span> |
|[<span data-ttu-id="75a77-206">用户</span><span class="sxs-lookup"><span data-stu-id="75a77-206">user</span></span>](../resources/user.md) | <span data-ttu-id="75a77-207">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="75a77-207">User.Read.All</span></span> | <span data-ttu-id="75a77-208">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="75a77-208">User.Read.All</span></span> | <span data-ttu-id="75a77-209">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="75a77-209">User.Read.All</span></span> |

> <span data-ttu-id="75a77-210">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="75a77-210">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="75a77-211">driveItem</span><span class="sxs-lookup"><span data-stu-id="75a77-211">driveItem</span></span>

<span data-ttu-id="75a77-212">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="75a77-212">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="75a77-213">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="75a77-213">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="75a77-214">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="75a77-214">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="75a77-215">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="75a77-215">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="75a77-216">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="75a77-216">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="75a77-217">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="75a77-217">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="75a77-218">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="75a77-218">contact, event, and message</span></span>

<span data-ttu-id="75a77-219">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="75a77-219">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="75a77-220">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="75a77-220">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="75a77-221">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="75a77-221">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="75a77-222">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="75a77-222">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="75a77-223">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="75a77-223">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="75a77-224">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="75a77-224">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="75a77-225">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="75a77-225">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="75a77-226">状态</span><span class="sxs-lookup"><span data-stu-id="75a77-226">presence</span></span>

<span data-ttu-id="75a77-227">**状态** 订阅需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="75a77-227">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="75a77-228">如果未指定 [encryptionCertificate](../resources/subscription.md)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="75a77-228">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="75a77-229">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="75a77-229">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="75a77-230">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="75a77-230">Optional query parameters</span></span>

<span data-ttu-id="75a77-231">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="75a77-231">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="75a77-232">请求标头</span><span class="sxs-lookup"><span data-stu-id="75a77-232">Request headers</span></span>

| <span data-ttu-id="75a77-233">名称</span><span class="sxs-lookup"><span data-stu-id="75a77-233">Name</span></span>       | <span data-ttu-id="75a77-234">类型</span><span class="sxs-lookup"><span data-stu-id="75a77-234">Type</span></span> | <span data-ttu-id="75a77-235">说明</span><span class="sxs-lookup"><span data-stu-id="75a77-235">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="75a77-236">Authorization</span><span class="sxs-lookup"><span data-stu-id="75a77-236">Authorization</span></span>  | <span data-ttu-id="75a77-237">string</span><span class="sxs-lookup"><span data-stu-id="75a77-237">string</span></span>  | <span data-ttu-id="75a77-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="75a77-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75a77-240">请求正文</span><span class="sxs-lookup"><span data-stu-id="75a77-240">Request body</span></span>

<span data-ttu-id="75a77-241">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="75a77-241">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75a77-242">响应</span><span class="sxs-lookup"><span data-stu-id="75a77-242">Response</span></span>

<span data-ttu-id="75a77-243">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="75a77-243">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75a77-244">示例</span><span class="sxs-lookup"><span data-stu-id="75a77-244">Example</span></span>

##### <a name="request"></a><span data-ttu-id="75a77-245">请求</span><span class="sxs-lookup"><span data-stu-id="75a77-245">Request</span></span>

<span data-ttu-id="75a77-246">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="75a77-246">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="75a77-247">HTTP</span><span class="sxs-lookup"><span data-stu-id="75a77-247">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="75a77-248">C#</span><span class="sxs-lookup"><span data-stu-id="75a77-248">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75a77-249">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75a77-249">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75a77-250">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75a77-250">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="75a77-251">Java</span><span class="sxs-lookup"><span data-stu-id="75a77-251">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="75a77-252">响应</span><span class="sxs-lookup"><span data-stu-id="75a77-252">Response</span></span>

<span data-ttu-id="75a77-253">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="75a77-253">Here is an example of the response.</span></span>
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
  "includeResourceData": false,
  "notificationContentType": "application/json"
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


