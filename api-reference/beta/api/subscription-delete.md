---
title: 删除订阅
description: 删除订阅。
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 8f57db6f84ff0b4afa90a586532f80241d8537e8
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366980"
---
# <a name="delete-subscription"></a><span data-ttu-id="3ec29-103">删除订阅</span><span class="sxs-lookup"><span data-stu-id="3ec29-103">Delete subscription</span></span>

<span data-ttu-id="3ec29-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ec29-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ec29-105">删除订阅。</span><span class="sxs-lookup"><span data-stu-id="3ec29-105">Delete a subscription.</span></span>

<span data-ttu-id="3ec29-106">请参阅" [权限](#permissions) 部分中的表格，了解支持订阅以更改通知的资源列表。</span><span class="sxs-lookup"><span data-stu-id="3ec29-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ec29-107">权限</span><span class="sxs-lookup"><span data-stu-id="3ec29-107">Permissions</span></span>

<span data-ttu-id="3ec29-108">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="3ec29-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="3ec29-109">若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ec29-109">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3ec29-110">支持的资源</span><span class="sxs-lookup"><span data-stu-id="3ec29-110">Supported resource</span></span> | <span data-ttu-id="3ec29-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ec29-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3ec29-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ec29-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ec29-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ec29-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="3ec29-114">callRecord</span><span class="sxs-lookup"><span data-stu-id="3ec29-114">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="3ec29-115">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-115">Not supported</span></span> | <span data-ttu-id="3ec29-116">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-116">Not supported</span></span> | <span data-ttu-id="3ec29-117">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-117">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="3ec29-118">[channels](../resources/channel.md) (/teams/getAllChannels – 组织中所有频道) </span><span class="sxs-lookup"><span data-stu-id="3ec29-118">[channels](../resources/channel.md) (/teams/getAllChannels – all channels in an organization)</span></span> | <span data-ttu-id="3ec29-119">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-119">Not supported</span></span>  | <span data-ttu-id="3ec29-120">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-120">Not supported</span></span> | <span data-ttu-id="3ec29-121">Channel.ReadBasic.All，ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-121">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span> |
|<span data-ttu-id="3ec29-122">[频道 (](../resources/channel.md) /teams/{id}/channels) </span><span class="sxs-lookup"><span data-stu-id="3ec29-122">[channels](../resources/channel.md) (/teams/{id}/channels)</span></span> | <span data-ttu-id="3ec29-123">Channel.ReadBasic.All，ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-123">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  | <span data-ttu-id="3ec29-124">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-124">Not supported</span></span> | <span data-ttu-id="3ec29-125">Channel.ReadBasic.All，ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-125">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  |
|<span data-ttu-id="3ec29-126">[chat](../resources/chat.md) (/chats – 组织内部的所有) </span><span class="sxs-lookup"><span data-stu-id="3ec29-126">[chat](../resources/chat.md) (/chats – all chats in an organization)</span></span> | <span data-ttu-id="3ec29-127">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-127">Not supported</span></span> | <span data-ttu-id="3ec29-128">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-128">Not supported</span></span> | <span data-ttu-id="3ec29-129">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-129">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="3ec29-130">[chat](../resources/chat.md) (/chats/{id}) </span><span class="sxs-lookup"><span data-stu-id="3ec29-130">[chat](../resources/chat.md) (/chats/{id})</span></span> | <span data-ttu-id="3ec29-131">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ec29-131">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="3ec29-132">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-132">Not supported</span></span> | <span data-ttu-id="3ec29-133">ChatSettings.Read.Chat *、ChatSettings.ReadWrite.Chat*、Chat.Manage.Chat\*、Chat.ReadBasic.All、Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-133">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="3ec29-134">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="3ec29-134">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="3ec29-135">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-135">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="3ec29-136">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-136">Not supported</span></span> | <span data-ttu-id="3ec29-137">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-137">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="3ec29-138">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="3ec29-138">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="3ec29-139">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-139">Not supported</span></span> | <span data-ttu-id="3ec29-140">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-140">Not supported</span></span> | <span data-ttu-id="3ec29-141">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-141">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="3ec29-142">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="3ec29-142">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="3ec29-143">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ec29-143">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="3ec29-144">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-144">Not supported</span></span> | <span data-ttu-id="3ec29-145">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-145">Chat.Read.All</span></span>  |
|<span data-ttu-id="3ec29-146">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="3ec29-146">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="3ec29-147">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-147">Not supported</span></span> | <span data-ttu-id="3ec29-148">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-148">Not supported</span></span> | <span data-ttu-id="3ec29-149">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-149">Chat.Read.All</span></span>  |
|[<span data-ttu-id="3ec29-150">contact</span><span class="sxs-lookup"><span data-stu-id="3ec29-150">contact</span></span>](../resources/contact.md) | <span data-ttu-id="3ec29-151">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="3ec29-151">Contacts.Read</span></span> | <span data-ttu-id="3ec29-152">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="3ec29-152">Contacts.Read</span></span> | <span data-ttu-id="3ec29-153">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="3ec29-153">Contacts.Read</span></span> |
|<span data-ttu-id="3ec29-154">[conversationMember](../resources/conversationmember.md) (/chats/getAllMembers) </span><span class="sxs-lookup"><span data-stu-id="3ec29-154">[conversationMember](../resources/conversationmember.md) (/chats/getAllMembers)</span></span> | <span data-ttu-id="3ec29-155">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-155">Not supported</span></span> | <span data-ttu-id="3ec29-156">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-156">Not supported</span></span> | <span data-ttu-id="3ec29-157">ChatMember.Read.All、ChatMember.ReadWrite.All、Chat.ReadBasic.All、Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-157">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="3ec29-158">[conversationMember](../resources/conversationmember.md) (/chats/{id}/members) </span><span class="sxs-lookup"><span data-stu-id="3ec29-158">[conversationMember](../resources/conversationmember.md) (/chats/{id}/members)</span></span> | <span data-ttu-id="3ec29-159">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ec29-159">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="3ec29-160">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-160">Not supported</span></span> | <span data-ttu-id="3ec29-161">ChatMember.Read.Chat *、Chat.Manage.Chat*、ChatMember.Read.All、ChatMember.ReadWrite.All、Chat.ReadBasic.All、Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-161">ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="3ec29-162">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members) </span><span class="sxs-lookup"><span data-stu-id="3ec29-162">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span></span> | <span data-ttu-id="3ec29-163">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-163">TeamMember.Read.All</span></span> | <span data-ttu-id="3ec29-164">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-164">Not supported</span></span> | <span data-ttu-id="3ec29-165">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-165">TeamMember.Read.All</span></span> |
|<span data-ttu-id="3ec29-166">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="3ec29-166">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="3ec29-167">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-167">Not supported</span></span> | <span data-ttu-id="3ec29-168">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ec29-168">Files.ReadWrite</span></span> | <span data-ttu-id="3ec29-169">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-169">Not supported</span></span> |
|<span data-ttu-id="3ec29-170">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="3ec29-170">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="3ec29-171">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-171">Files.ReadWrite.All</span></span> | <span data-ttu-id="3ec29-172">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-172">Not supported</span></span> | <span data-ttu-id="3ec29-173">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-173">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="3ec29-174">事件</span><span class="sxs-lookup"><span data-stu-id="3ec29-174">event</span></span>](../resources/event.md) | <span data-ttu-id="3ec29-175">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3ec29-175">Calendars.Read</span></span> | <span data-ttu-id="3ec29-176">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3ec29-176">Calendars.Read</span></span> | <span data-ttu-id="3ec29-177">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3ec29-177">Calendars.Read</span></span> |
|[<span data-ttu-id="3ec29-178">组</span><span class="sxs-lookup"><span data-stu-id="3ec29-178">group</span></span>](../resources/group.md) | <span data-ttu-id="3ec29-179">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-179">Group.Read.All</span></span> | <span data-ttu-id="3ec29-180">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-180">Not supported</span></span> | <span data-ttu-id="3ec29-181">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-181">Group.Read.All</span></span> |
|[<span data-ttu-id="3ec29-182">组对话</span><span class="sxs-lookup"><span data-stu-id="3ec29-182">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="3ec29-183">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-183">Group.Read.All</span></span> | <span data-ttu-id="3ec29-184">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-184">Not supported</span></span> | <span data-ttu-id="3ec29-185">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-185">Not supported</span></span> |
|[<span data-ttu-id="3ec29-186">列表</span><span class="sxs-lookup"><span data-stu-id="3ec29-186">list</span></span>](../resources/list.md) | <span data-ttu-id="3ec29-187">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-187">Sites.ReadWrite.All</span></span> | <span data-ttu-id="3ec29-188">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-188">Not supported</span></span> | <span data-ttu-id="3ec29-189">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-189">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="3ec29-190">邮件</span><span class="sxs-lookup"><span data-stu-id="3ec29-190">message</span></span>](../resources/message.md) | <span data-ttu-id="3ec29-191">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3ec29-191">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="3ec29-192">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3ec29-192">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="3ec29-193">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3ec29-193">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="3ec29-194">状态</span><span class="sxs-lookup"><span data-stu-id="3ec29-194">presence</span></span>](../resources/presence.md) | <span data-ttu-id="3ec29-195">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-195">Presence.Read.All</span></span> | <span data-ttu-id="3ec29-196">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-196">Not supported</span></span> | <span data-ttu-id="3ec29-197">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-197">Not supported</span></span> |
|[<span data-ttu-id="3ec29-198">打印机</span><span class="sxs-lookup"><span data-stu-id="3ec29-198">printer</span></span>](../resources/printer.md) | <span data-ttu-id="3ec29-199">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-199">Not supported</span></span> | <span data-ttu-id="3ec29-200">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-200">Not supported</span></span> | <span data-ttu-id="3ec29-201">打印机。阅读.All，Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-201">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="3ec29-202">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="3ec29-202">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="3ec29-203">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-203">Not supported</span></span> | <span data-ttu-id="3ec29-204">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-204">Not supported</span></span> | <span data-ttu-id="3ec29-205">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-205">PrintTaskDefinition.ReadWrite.All</span></span> |
|<span data-ttu-id="3ec29-206">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="3ec29-206">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="3ec29-207">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-207">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="3ec29-208">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-208">Not supported</span></span> | <span data-ttu-id="3ec29-209">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-209">SecurityEvents.ReadWrite.All</span></span> |
|<span data-ttu-id="3ec29-210">[teams](../resources/team.md) (/teams – 组织内部的所有) </span><span class="sxs-lookup"><span data-stu-id="3ec29-210">[teams](../resources/team.md) (/teams – all teams in an organization)</span></span> | <span data-ttu-id="3ec29-211">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-211">Not supported</span></span> | <span data-ttu-id="3ec29-212">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-212">Not supported</span></span> | <span data-ttu-id="3ec29-213">Team.ReadBasic.All，TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-213">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|<span data-ttu-id="3ec29-214">[teams](../resources/team.md) (/teams/{id}) </span><span class="sxs-lookup"><span data-stu-id="3ec29-214">[teams](../resources/team.md) (/teams/{id})</span></span> | <span data-ttu-id="3ec29-215">Team.ReadBasic.All，TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-215">Team.ReadBasic.All, TeamSettings.Read.All</span></span> | <span data-ttu-id="3ec29-216">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-216">Not supported</span></span> | <span data-ttu-id="3ec29-217">Team.ReadBasic.All，TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-217">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|[<span data-ttu-id="3ec29-218">todoTask</span><span class="sxs-lookup"><span data-stu-id="3ec29-218">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="3ec29-219">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ec29-219">Tasks.ReadWrite</span></span> | <span data-ttu-id="3ec29-220">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ec29-220">Tasks.ReadWrite</span></span> | <span data-ttu-id="3ec29-221">不支持</span><span class="sxs-lookup"><span data-stu-id="3ec29-221">Not supported</span></span> |
|[<span data-ttu-id="3ec29-222">用户</span><span class="sxs-lookup"><span data-stu-id="3ec29-222">user</span></span>](../resources/user.md) | <span data-ttu-id="3ec29-223">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-223">User.Read.All</span></span> | <span data-ttu-id="3ec29-224">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-224">User.Read.All</span></span> | <span data-ttu-id="3ec29-225">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ec29-225">User.Read.All</span></span> |

> <span data-ttu-id="3ec29-226">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="3ec29-226">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="3ec29-227">driveItem</span><span class="sxs-lookup"><span data-stu-id="3ec29-227">driveItem</span></span>

<span data-ttu-id="3ec29-228">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="3ec29-228">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="3ec29-229">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="3ec29-229">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="3ec29-230">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="3ec29-230">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="3ec29-231">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="3ec29-231">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="3ec29-232">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="3ec29-232">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="3ec29-233">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="3ec29-233">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="3ec29-234">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="3ec29-234">contact, event, and message</span></span>

<span data-ttu-id="3ec29-235">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="3ec29-235">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="3ec29-236">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="3ec29-236">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="3ec29-237">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="3ec29-237">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="3ec29-238">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="3ec29-238">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="3ec29-239">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="3ec29-239">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="3ec29-240">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="3ec29-240">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="3ec29-241">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="3ec29-241">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="3ec29-242">状态</span><span class="sxs-lookup"><span data-stu-id="3ec29-242">presence</span></span>

<span data-ttu-id="3ec29-243">**状态** 订阅需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="3ec29-243">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="3ec29-244">如果未指定 [encryptionCertificate](../resources/subscription.md)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="3ec29-244">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="3ec29-245">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ec29-245">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="3ec29-246">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ec29-246">Request headers</span></span>

| <span data-ttu-id="3ec29-247">名称</span><span class="sxs-lookup"><span data-stu-id="3ec29-247">Name</span></span>       | <span data-ttu-id="3ec29-248">类型</span><span class="sxs-lookup"><span data-stu-id="3ec29-248">Type</span></span> | <span data-ttu-id="3ec29-249">说明</span><span class="sxs-lookup"><span data-stu-id="3ec29-249">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3ec29-250">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ec29-250">Authorization</span></span>  | <span data-ttu-id="3ec29-251">string</span><span class="sxs-lookup"><span data-stu-id="3ec29-251">string</span></span>  | <span data-ttu-id="3ec29-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3ec29-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ec29-254">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ec29-254">Request body</span></span>

<span data-ttu-id="3ec29-255">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3ec29-255">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ec29-256">响应</span><span class="sxs-lookup"><span data-stu-id="3ec29-256">Response</span></span>

<span data-ttu-id="3ec29-257">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="3ec29-257">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="3ec29-258">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="3ec29-258">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="3ec29-259">示例</span><span class="sxs-lookup"><span data-stu-id="3ec29-259">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3ec29-260">请求</span><span class="sxs-lookup"><span data-stu-id="3ec29-260">Request</span></span>

<span data-ttu-id="3ec29-261">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3ec29-261">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3ec29-262">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ec29-262">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="3ec29-263">C#</span><span class="sxs-lookup"><span data-stu-id="3ec29-263">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ec29-264">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ec29-264">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ec29-265">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ec29-265">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ec29-266">Java</span><span class="sxs-lookup"><span data-stu-id="3ec29-266">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3ec29-267">响应</span><span class="sxs-lookup"><span data-stu-id="3ec29-267">Response</span></span>

<span data-ttu-id="3ec29-268">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3ec29-268">Here is an example of the response.</span></span>
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


