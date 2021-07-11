---
title: 更新订阅
description: 通过延长到期时间续订订阅。
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 96680ebb1cedf85f7272bc09b8ab1c55a04c7591
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366919"
---
# <a name="update-subscription"></a><span data-ttu-id="8b758-103">更新订阅</span><span class="sxs-lookup"><span data-stu-id="8b758-103">Update subscription</span></span>

<span data-ttu-id="8b758-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b758-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b758-105">通过延长到期时间续订订阅。</span><span class="sxs-lookup"><span data-stu-id="8b758-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="8b758-106">"权限 ["部分](#permissions) 中的表列出了支持订阅更改通知的资源。</span><span class="sxs-lookup"><span data-stu-id="8b758-106">The table in the [Permissions](#permissions) section lists the resources that support subscribing to change notifications.</span></span>

<span data-ttu-id="8b758-107">订阅在时间长度因资源类型而异后过期。</span><span class="sxs-lookup"><span data-stu-id="8b758-107">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="8b758-108">为了避免缺少更改通知，应用应在到期日期之前提前续订其订阅。</span><span class="sxs-lookup"><span data-stu-id="8b758-108">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="8b758-109">请参阅 [订阅](../resources/subscription.md) ，了解每种资源类型的订阅的最大长度。</span><span class="sxs-lookup"><span data-stu-id="8b758-109">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b758-110">权限</span><span class="sxs-lookup"><span data-stu-id="8b758-110">Permissions</span></span>

<span data-ttu-id="8b758-111">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="8b758-111">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="8b758-112">若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8b758-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b758-113">支持的资源</span><span class="sxs-lookup"><span data-stu-id="8b758-113">Supported resource</span></span> | <span data-ttu-id="8b758-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8b758-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8b758-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8b758-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b758-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8b758-116">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="8b758-117">callRecord</span><span class="sxs-lookup"><span data-stu-id="8b758-117">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="8b758-118">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-118">Not supported</span></span> | <span data-ttu-id="8b758-119">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-119">Not supported</span></span> | <span data-ttu-id="8b758-120">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b758-120">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="8b758-121">[channels](../resources/channel.md) (/teams/getAllChannels – 组织中所有频道) </span><span class="sxs-lookup"><span data-stu-id="8b758-121">[channels](../resources/channel.md) (/teams/getAllChannels – all channels in an organization)</span></span> | <span data-ttu-id="8b758-122">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-122">Not supported</span></span>  | <span data-ttu-id="8b758-123">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-123">Not supported</span></span> | <span data-ttu-id="8b758-124">Channel.ReadBasic.All，ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b758-124">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span> |
|<span data-ttu-id="8b758-125">[频道 (](../resources/channel.md) /teams/{id}/channels) </span><span class="sxs-lookup"><span data-stu-id="8b758-125">[channels](../resources/channel.md) (/teams/{id}/channels)</span></span> | <span data-ttu-id="8b758-126">Channel.ReadBasic.All，ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b758-126">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  | <span data-ttu-id="8b758-127">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-127">Not supported</span></span> | <span data-ttu-id="8b758-128">Channel.ReadBasic.All，ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b758-128">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  |
|<span data-ttu-id="8b758-129">[chat](../resources/chat.md) (/chats – 组织内部的所有) </span><span class="sxs-lookup"><span data-stu-id="8b758-129">[chat](../resources/chat.md) (/chats – all chats in an organization)</span></span> | <span data-ttu-id="8b758-130">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-130">Not supported</span></span> | <span data-ttu-id="8b758-131">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-131">Not supported</span></span> | <span data-ttu-id="8b758-132">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b758-132">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="8b758-133">[chat](../resources/chat.md) (/chats/{id}) </span><span class="sxs-lookup"><span data-stu-id="8b758-133">[chat](../resources/chat.md) (/chats/{id})</span></span> | <span data-ttu-id="8b758-134">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b758-134">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="8b758-135">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-135">Not supported</span></span> | <span data-ttu-id="8b758-136">ChatSettings.Read.Chat *、ChatSettings.ReadWrite.Chat*、Chat.Manage.Chat\*、Chat.ReadBasic.All、Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b758-136">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="8b758-137">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="8b758-137">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="8b758-138">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b758-138">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="8b758-139">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-139">Not supported</span></span> | <span data-ttu-id="8b758-140">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b758-140">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="8b758-141">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="8b758-141">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="8b758-142">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-142">Not supported</span></span> | <span data-ttu-id="8b758-143">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-143">Not supported</span></span> | <span data-ttu-id="8b758-144">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b758-144">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="8b758-145">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="8b758-145">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="8b758-146">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b758-146">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="8b758-147">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-147">Not supported</span></span> | <span data-ttu-id="8b758-148">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b758-148">Chat.Read.All</span></span>  |
|<span data-ttu-id="8b758-149">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="8b758-149">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="8b758-150">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-150">Not supported</span></span> | <span data-ttu-id="8b758-151">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-151">Not supported</span></span> | <span data-ttu-id="8b758-152">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b758-152">Chat.Read.All</span></span>  |
|[<span data-ttu-id="8b758-153">contact</span><span class="sxs-lookup"><span data-stu-id="8b758-153">contact</span></span>](../resources/contact.md) | <span data-ttu-id="8b758-154">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8b758-154">Contacts.Read</span></span> | <span data-ttu-id="8b758-155">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8b758-155">Contacts.Read</span></span> | <span data-ttu-id="8b758-156">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8b758-156">Contacts.Read</span></span> |
|<span data-ttu-id="8b758-157">[conversationMember](../resources/conversationmember.md) (/chats/getAllMembers) </span><span class="sxs-lookup"><span data-stu-id="8b758-157">[conversationMember](../resources/conversationmember.md) (/chats/getAllMembers)</span></span> | <span data-ttu-id="8b758-158">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-158">Not supported</span></span> | <span data-ttu-id="8b758-159">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-159">Not supported</span></span> | <span data-ttu-id="8b758-160">ChatMember.Read.All、ChatMember.ReadWrite.All、Chat.ReadBasic.All、Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b758-160">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="8b758-161">[conversationMember](../resources/conversationmember.md) (/chats/{id}/members) </span><span class="sxs-lookup"><span data-stu-id="8b758-161">[conversationMember](../resources/conversationmember.md) (/chats/{id}/members)</span></span> | <span data-ttu-id="8b758-162">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b758-162">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="8b758-163">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-163">Not supported</span></span> | <span data-ttu-id="8b758-164">ChatMember.Read.Chat *、Chat.Manage.Chat*、ChatMember.Read.All、ChatMember.ReadWrite.All、Chat.ReadBasic.All、Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b758-164">ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="8b758-165">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members) </span><span class="sxs-lookup"><span data-stu-id="8b758-165">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span></span> | <span data-ttu-id="8b758-166">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b758-166">TeamMember.Read.All</span></span> | <span data-ttu-id="8b758-167">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-167">Not supported</span></span> | <span data-ttu-id="8b758-168">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b758-168">TeamMember.Read.All</span></span> |
|<span data-ttu-id="8b758-169">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="8b758-169">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="8b758-170">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-170">Not supported</span></span> | <span data-ttu-id="8b758-171">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b758-171">Files.ReadWrite</span></span> | <span data-ttu-id="8b758-172">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-172">Not supported</span></span> |
|<span data-ttu-id="8b758-173">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="8b758-173">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="8b758-174">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b758-174">Files.ReadWrite.All</span></span> | <span data-ttu-id="8b758-175">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-175">Not supported</span></span> | <span data-ttu-id="8b758-176">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b758-176">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="8b758-177">事件</span><span class="sxs-lookup"><span data-stu-id="8b758-177">event</span></span>](../resources/event.md) | <span data-ttu-id="8b758-178">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8b758-178">Calendars.Read</span></span> | <span data-ttu-id="8b758-179">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8b758-179">Calendars.Read</span></span> | <span data-ttu-id="8b758-180">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8b758-180">Calendars.Read</span></span> |
|[<span data-ttu-id="8b758-181">组</span><span class="sxs-lookup"><span data-stu-id="8b758-181">group</span></span>](../resources/group.md) | <span data-ttu-id="8b758-182">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b758-182">Group.Read.All</span></span> | <span data-ttu-id="8b758-183">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-183">Not supported</span></span> | <span data-ttu-id="8b758-184">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b758-184">Group.Read.All</span></span> |
|[<span data-ttu-id="8b758-185">组对话</span><span class="sxs-lookup"><span data-stu-id="8b758-185">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="8b758-186">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b758-186">Group.Read.All</span></span> | <span data-ttu-id="8b758-187">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-187">Not supported</span></span> | <span data-ttu-id="8b758-188">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-188">Not supported</span></span> |
|[<span data-ttu-id="8b758-189">列表</span><span class="sxs-lookup"><span data-stu-id="8b758-189">list</span></span>](../resources/list.md) | <span data-ttu-id="8b758-190">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b758-190">Sites.ReadWrite.All</span></span> | <span data-ttu-id="8b758-191">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-191">Not supported</span></span> | <span data-ttu-id="8b758-192">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b758-192">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="8b758-193">邮件</span><span class="sxs-lookup"><span data-stu-id="8b758-193">message</span></span>](../resources/message.md) | <span data-ttu-id="8b758-194">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8b758-194">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="8b758-195">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8b758-195">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="8b758-196">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8b758-196">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="8b758-197">状态</span><span class="sxs-lookup"><span data-stu-id="8b758-197">presence</span></span>](../resources/presence.md) | <span data-ttu-id="8b758-198">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b758-198">Presence.Read.All</span></span> | <span data-ttu-id="8b758-199">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-199">Not supported</span></span> | <span data-ttu-id="8b758-200">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-200">Not supported</span></span> |
|[<span data-ttu-id="8b758-201">打印机</span><span class="sxs-lookup"><span data-stu-id="8b758-201">printer</span></span>](../resources/printer.md) | <span data-ttu-id="8b758-202">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-202">Not supported</span></span> | <span data-ttu-id="8b758-203">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-203">Not supported</span></span> | <span data-ttu-id="8b758-204">打印机。阅读.All，Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b758-204">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="8b758-205">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="8b758-205">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="8b758-206">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-206">Not supported</span></span> | <span data-ttu-id="8b758-207">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-207">Not supported</span></span> | <span data-ttu-id="8b758-208">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b758-208">PrintTaskDefinition.ReadWrite.All</span></span> |
|<span data-ttu-id="8b758-209">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="8b758-209">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="8b758-210">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b758-210">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="8b758-211">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-211">Not supported</span></span> | <span data-ttu-id="8b758-212">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b758-212">SecurityEvents.ReadWrite.All</span></span> |
|<span data-ttu-id="8b758-213">[teams](../resources/team.md) (/teams – 组织内部的所有) </span><span class="sxs-lookup"><span data-stu-id="8b758-213">[teams](../resources/team.md) (/teams – all teams in an organization)</span></span> | <span data-ttu-id="8b758-214">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-214">Not supported</span></span> | <span data-ttu-id="8b758-215">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-215">Not supported</span></span> | <span data-ttu-id="8b758-216">Team.ReadBasic.All，TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b758-216">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|<span data-ttu-id="8b758-217">[teams](../resources/team.md) (/teams/{id}) </span><span class="sxs-lookup"><span data-stu-id="8b758-217">[teams](../resources/team.md) (/teams/{id})</span></span> | <span data-ttu-id="8b758-218">Team.ReadBasic.All，TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b758-218">Team.ReadBasic.All, TeamSettings.Read.All</span></span> | <span data-ttu-id="8b758-219">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-219">Not supported</span></span> | <span data-ttu-id="8b758-220">Team.ReadBasic.All，TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b758-220">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|[<span data-ttu-id="8b758-221">todoTask</span><span class="sxs-lookup"><span data-stu-id="8b758-221">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="8b758-222">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b758-222">Tasks.ReadWrite</span></span> | <span data-ttu-id="8b758-223">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b758-223">Tasks.ReadWrite</span></span> | <span data-ttu-id="8b758-224">不支持</span><span class="sxs-lookup"><span data-stu-id="8b758-224">Not supported</span></span> |
|[<span data-ttu-id="8b758-225">用户</span><span class="sxs-lookup"><span data-stu-id="8b758-225">user</span></span>](../resources/user.md) | <span data-ttu-id="8b758-226">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b758-226">User.Read.All</span></span> | <span data-ttu-id="8b758-227">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b758-227">User.Read.All</span></span> | <span data-ttu-id="8b758-228">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b758-228">User.Read.All</span></span> |

> <span data-ttu-id="8b758-229">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="8b758-229">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="8b758-230">driveItem</span><span class="sxs-lookup"><span data-stu-id="8b758-230">driveItem</span></span>

<span data-ttu-id="8b758-231">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="8b758-231">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="8b758-232">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="8b758-232">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="8b758-233">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="8b758-233">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="8b758-234">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="8b758-234">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="8b758-235">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="8b758-235">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="8b758-236">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="8b758-236">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="8b758-237">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="8b758-237">contact, event, and message</span></span>

<span data-ttu-id="8b758-238">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="8b758-238">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="8b758-239">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="8b758-239">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="8b758-240">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="8b758-240">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="8b758-241">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="8b758-241">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="8b758-242">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="8b758-242">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="8b758-243">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="8b758-243">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="8b758-244">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="8b758-244">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="8b758-245">状态</span><span class="sxs-lookup"><span data-stu-id="8b758-245">presence</span></span>

<span data-ttu-id="8b758-246">**状态** 订阅需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="8b758-246">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="8b758-247">如果未指定 [encryptionCertificate](../resources/subscription.md)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="8b758-247">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="8b758-248">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8b758-248">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8b758-249">请求标头</span><span class="sxs-lookup"><span data-stu-id="8b758-249">Request headers</span></span>

| <span data-ttu-id="8b758-250">名称</span><span class="sxs-lookup"><span data-stu-id="8b758-250">Name</span></span>       | <span data-ttu-id="8b758-251">类型</span><span class="sxs-lookup"><span data-stu-id="8b758-251">Type</span></span> | <span data-ttu-id="8b758-252">说明</span><span class="sxs-lookup"><span data-stu-id="8b758-252">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8b758-253">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b758-253">Authorization</span></span>  | <span data-ttu-id="8b758-254">string</span><span class="sxs-lookup"><span data-stu-id="8b758-254">string</span></span>  | <span data-ttu-id="8b758-p108">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8b758-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8b758-257">响应</span><span class="sxs-lookup"><span data-stu-id="8b758-257">Response</span></span>

<span data-ttu-id="8b758-258">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8b758-258">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="8b758-259">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="8b758-259">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="8b758-260">示例</span><span class="sxs-lookup"><span data-stu-id="8b758-260">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8b758-261">请求</span><span class="sxs-lookup"><span data-stu-id="8b758-261">Request</span></span>

<span data-ttu-id="8b758-262">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8b758-262">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8b758-263">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b758-263">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8b758-264">C#</span><span class="sxs-lookup"><span data-stu-id="8b758-264">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b758-265">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b758-265">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b758-266">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b758-266">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b758-267">Java</span><span class="sxs-lookup"><span data-stu-id="8b758-267">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8b758-268">响应</span><span class="sxs-lookup"><span data-stu-id="8b758-268">Response</span></span>

<span data-ttu-id="8b758-269">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8b758-269">Here is an example of the response.</span></span>
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


