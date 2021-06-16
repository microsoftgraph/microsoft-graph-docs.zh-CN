---
title: 更新订阅
description: 通过延长到期时间续订订阅。
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 592631033cc411e034433d8fe33648b513da403f
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941504"
---
# <a name="update-subscription"></a><span data-ttu-id="6073c-103">更新订阅</span><span class="sxs-lookup"><span data-stu-id="6073c-103">Update subscription</span></span>

<span data-ttu-id="6073c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6073c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6073c-105">通过延长到期时间续订订阅。</span><span class="sxs-lookup"><span data-stu-id="6073c-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="6073c-106">"权限 ["部分](#permissions) 中的表列出了支持订阅更改通知的资源。</span><span class="sxs-lookup"><span data-stu-id="6073c-106">The table in the [Permissions](#permissions) section lists the resources that support subscribing to change notifications.</span></span>

<span data-ttu-id="6073c-107">订阅在时间长度因资源类型而异后过期。</span><span class="sxs-lookup"><span data-stu-id="6073c-107">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="6073c-108">为了避免缺少更改通知，应用应在到期日期之前提前续订其订阅。</span><span class="sxs-lookup"><span data-stu-id="6073c-108">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="6073c-109">请参阅 [订阅](../resources/subscription.md) ，了解每种资源类型的订阅的最大长度。</span><span class="sxs-lookup"><span data-stu-id="6073c-109">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="6073c-110">权限</span><span class="sxs-lookup"><span data-stu-id="6073c-110">Permissions</span></span>

<span data-ttu-id="6073c-111">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="6073c-111">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="6073c-112">若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6073c-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6073c-113">支持的资源</span><span class="sxs-lookup"><span data-stu-id="6073c-113">Supported resource</span></span> | <span data-ttu-id="6073c-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6073c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6073c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6073c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6073c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6073c-116">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="6073c-117">callRecord</span><span class="sxs-lookup"><span data-stu-id="6073c-117">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="6073c-118">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-118">Not supported</span></span> | <span data-ttu-id="6073c-119">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-119">Not supported</span></span> | <span data-ttu-id="6073c-120">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="6073c-120">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="6073c-121">[channels](../resources/channel.md) (/teams/getAllChannels – 组织中所有频道) </span><span class="sxs-lookup"><span data-stu-id="6073c-121">[channels](../resources/channel.md) (/teams/getAllChannels – all channels in an organization)</span></span> | <span data-ttu-id="6073c-122">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-122">Not supported</span></span>  | <span data-ttu-id="6073c-123">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-123">Not supported</span></span> | <span data-ttu-id="6073c-124">Channel.ReadBasic.All、ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="6073c-124">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span> |
|<span data-ttu-id="6073c-125">[频道 (](../resources/channel.md) /teams/{id}/channels) </span><span class="sxs-lookup"><span data-stu-id="6073c-125">[channels](../resources/channel.md) (/teams/{id}/channels)</span></span> | <span data-ttu-id="6073c-126">Channel.ReadBasic.All、ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="6073c-126">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  | <span data-ttu-id="6073c-127">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-127">Not supported</span></span> | <span data-ttu-id="6073c-128">Channel.ReadBasic.All、ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="6073c-128">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  |
|<span data-ttu-id="6073c-129">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="6073c-129">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="6073c-130">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6073c-130">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="6073c-131">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-131">Not supported</span></span> | <span data-ttu-id="6073c-132">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="6073c-132">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="6073c-133">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="6073c-133">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="6073c-134">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-134">Not supported</span></span> | <span data-ttu-id="6073c-135">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-135">Not supported</span></span> | <span data-ttu-id="6073c-136">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="6073c-136">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="6073c-137">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="6073c-137">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="6073c-138">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6073c-138">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="6073c-139">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-139">Not supported</span></span> | <span data-ttu-id="6073c-140">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="6073c-140">Chat.Read.All</span></span>  |
|<span data-ttu-id="6073c-141">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="6073c-141">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="6073c-142">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-142">Not supported</span></span> | <span data-ttu-id="6073c-143">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-143">Not supported</span></span> | <span data-ttu-id="6073c-144">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="6073c-144">Chat.Read.All</span></span>  |
|[<span data-ttu-id="6073c-145">contact</span><span class="sxs-lookup"><span data-stu-id="6073c-145">contact</span></span>](../resources/contact.md) | <span data-ttu-id="6073c-146">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6073c-146">Contacts.Read</span></span> | <span data-ttu-id="6073c-147">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6073c-147">Contacts.Read</span></span> | <span data-ttu-id="6073c-148">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6073c-148">Contacts.Read</span></span> |
|<span data-ttu-id="6073c-149">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members) </span><span class="sxs-lookup"><span data-stu-id="6073c-149">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span></span> | <span data-ttu-id="6073c-150">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="6073c-150">TeamMember.Read.All</span></span> | <span data-ttu-id="6073c-151">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-151">Not supported</span></span> | <span data-ttu-id="6073c-152">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="6073c-152">TeamMember.Read.All</span></span> |
|<span data-ttu-id="6073c-153">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="6073c-153">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="6073c-154">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-154">Not supported</span></span> | <span data-ttu-id="6073c-155">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6073c-155">Files.ReadWrite</span></span> | <span data-ttu-id="6073c-156">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-156">Not supported</span></span> |
|<span data-ttu-id="6073c-157">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="6073c-157">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="6073c-158">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6073c-158">Files.ReadWrite.All</span></span> | <span data-ttu-id="6073c-159">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-159">Not supported</span></span> | <span data-ttu-id="6073c-160">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6073c-160">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="6073c-161">事件</span><span class="sxs-lookup"><span data-stu-id="6073c-161">event</span></span>](../resources/event.md) | <span data-ttu-id="6073c-162">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6073c-162">Calendars.Read</span></span> | <span data-ttu-id="6073c-163">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6073c-163">Calendars.Read</span></span> | <span data-ttu-id="6073c-164">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6073c-164">Calendars.Read</span></span> |
|[<span data-ttu-id="6073c-165">组</span><span class="sxs-lookup"><span data-stu-id="6073c-165">group</span></span>](../resources/group.md) | <span data-ttu-id="6073c-166">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6073c-166">Group.Read.All</span></span> | <span data-ttu-id="6073c-167">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-167">Not supported</span></span> | <span data-ttu-id="6073c-168">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6073c-168">Group.Read.All</span></span> |
|[<span data-ttu-id="6073c-169">组对话</span><span class="sxs-lookup"><span data-stu-id="6073c-169">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="6073c-170">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6073c-170">Group.Read.All</span></span> | <span data-ttu-id="6073c-171">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-171">Not supported</span></span> | <span data-ttu-id="6073c-172">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-172">Not supported</span></span> |
|[<span data-ttu-id="6073c-173">列表</span><span class="sxs-lookup"><span data-stu-id="6073c-173">list</span></span>](../resources/list.md) | <span data-ttu-id="6073c-174">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6073c-174">Sites.ReadWrite.All</span></span> | <span data-ttu-id="6073c-175">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-175">Not supported</span></span> | <span data-ttu-id="6073c-176">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6073c-176">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="6073c-177">邮件</span><span class="sxs-lookup"><span data-stu-id="6073c-177">message</span></span>](../resources/message.md) | <span data-ttu-id="6073c-178">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6073c-178">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="6073c-179">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6073c-179">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="6073c-180">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6073c-180">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="6073c-181">状态</span><span class="sxs-lookup"><span data-stu-id="6073c-181">presence</span></span>](../resources/presence.md) | <span data-ttu-id="6073c-182">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="6073c-182">Presence.Read.All</span></span> | <span data-ttu-id="6073c-183">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-183">Not supported</span></span> | <span data-ttu-id="6073c-184">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-184">Not supported</span></span> |
|[<span data-ttu-id="6073c-185">打印机</span><span class="sxs-lookup"><span data-stu-id="6073c-185">printer</span></span>](../resources/printer.md) | <span data-ttu-id="6073c-186">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-186">Not supported</span></span> | <span data-ttu-id="6073c-187">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-187">Not supported</span></span> | <span data-ttu-id="6073c-188">打印机。阅读.All，Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6073c-188">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="6073c-189">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="6073c-189">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="6073c-190">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-190">Not supported</span></span> | <span data-ttu-id="6073c-191">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-191">Not supported</span></span> | <span data-ttu-id="6073c-192">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6073c-192">PrintTaskDefinition.ReadWrite.All</span></span> |
|<span data-ttu-id="6073c-193">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="6073c-193">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="6073c-194">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6073c-194">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="6073c-195">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-195">Not supported</span></span> | <span data-ttu-id="6073c-196">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6073c-196">SecurityEvents.ReadWrite.All</span></span> |
|<span data-ttu-id="6073c-197">[teams](../resources/team.md) (/teams – 组织内部的所有) </span><span class="sxs-lookup"><span data-stu-id="6073c-197">[teams](../resources/team.md) (/teams – all teams in an organization)</span></span> | <span data-ttu-id="6073c-198">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-198">Not supported</span></span> | <span data-ttu-id="6073c-199">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-199">Not supported</span></span> | <span data-ttu-id="6073c-200">Team.ReadBasic.All、TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="6073c-200">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|<span data-ttu-id="6073c-201">[teams](../resources/team.md) (/teams/{id}) </span><span class="sxs-lookup"><span data-stu-id="6073c-201">[teams](../resources/team.md) (/teams/{id})</span></span> | <span data-ttu-id="6073c-202">Team.ReadBasic.All、TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="6073c-202">Team.ReadBasic.All, TeamSettings.Read.All</span></span> | <span data-ttu-id="6073c-203">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-203">Not supported</span></span> | <span data-ttu-id="6073c-204">Team.ReadBasic.All、TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="6073c-204">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|[<span data-ttu-id="6073c-205">todoTask</span><span class="sxs-lookup"><span data-stu-id="6073c-205">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="6073c-206">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6073c-206">Tasks.ReadWrite</span></span> | <span data-ttu-id="6073c-207">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6073c-207">Tasks.ReadWrite</span></span> | <span data-ttu-id="6073c-208">不支持</span><span class="sxs-lookup"><span data-stu-id="6073c-208">Not supported</span></span> |
|[<span data-ttu-id="6073c-209">用户</span><span class="sxs-lookup"><span data-stu-id="6073c-209">user</span></span>](../resources/user.md) | <span data-ttu-id="6073c-210">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6073c-210">User.Read.All</span></span> | <span data-ttu-id="6073c-211">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6073c-211">User.Read.All</span></span> | <span data-ttu-id="6073c-212">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6073c-212">User.Read.All</span></span> |

> <span data-ttu-id="6073c-213">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="6073c-213">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="6073c-214">driveItem</span><span class="sxs-lookup"><span data-stu-id="6073c-214">driveItem</span></span>

<span data-ttu-id="6073c-215">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="6073c-215">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="6073c-216">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="6073c-216">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="6073c-217">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="6073c-217">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="6073c-218">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="6073c-218">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="6073c-219">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="6073c-219">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="6073c-220">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="6073c-220">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="6073c-221">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="6073c-221">contact, event, and message</span></span>

<span data-ttu-id="6073c-222">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="6073c-222">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="6073c-223">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="6073c-223">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="6073c-224">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="6073c-224">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="6073c-225">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="6073c-225">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="6073c-226">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="6073c-226">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="6073c-227">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="6073c-227">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="6073c-228">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="6073c-228">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="6073c-229">状态</span><span class="sxs-lookup"><span data-stu-id="6073c-229">presence</span></span>

<span data-ttu-id="6073c-230">**状态** 订阅需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="6073c-230">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="6073c-231">如果未指定 [encryptionCertificate](../resources/subscription.md)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="6073c-231">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="6073c-232">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6073c-232">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6073c-233">请求标头</span><span class="sxs-lookup"><span data-stu-id="6073c-233">Request headers</span></span>

| <span data-ttu-id="6073c-234">名称</span><span class="sxs-lookup"><span data-stu-id="6073c-234">Name</span></span>       | <span data-ttu-id="6073c-235">类型</span><span class="sxs-lookup"><span data-stu-id="6073c-235">Type</span></span> | <span data-ttu-id="6073c-236">说明</span><span class="sxs-lookup"><span data-stu-id="6073c-236">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6073c-237">Authorization</span><span class="sxs-lookup"><span data-stu-id="6073c-237">Authorization</span></span>  | <span data-ttu-id="6073c-238">string</span><span class="sxs-lookup"><span data-stu-id="6073c-238">string</span></span>  | <span data-ttu-id="6073c-p108">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6073c-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6073c-241">响应</span><span class="sxs-lookup"><span data-stu-id="6073c-241">Response</span></span>

<span data-ttu-id="6073c-242">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6073c-242">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="6073c-243">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="6073c-243">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="6073c-244">示例</span><span class="sxs-lookup"><span data-stu-id="6073c-244">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6073c-245">请求</span><span class="sxs-lookup"><span data-stu-id="6073c-245">Request</span></span>

<span data-ttu-id="6073c-246">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6073c-246">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6073c-247">HTTP</span><span class="sxs-lookup"><span data-stu-id="6073c-247">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6073c-248">C#</span><span class="sxs-lookup"><span data-stu-id="6073c-248">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6073c-249">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6073c-249">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6073c-250">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6073c-250">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6073c-251">Java</span><span class="sxs-lookup"><span data-stu-id="6073c-251">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6073c-252">响应</span><span class="sxs-lookup"><span data-stu-id="6073c-252">Response</span></span>

<span data-ttu-id="6073c-253">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6073c-253">Here is an example of the response.</span></span>
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
  "includeResourceData": false,
  "notificationContentType": "application/json"
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


