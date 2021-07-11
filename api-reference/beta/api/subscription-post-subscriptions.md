---
title: 创建订阅
description: 订阅侦听器应用程序，以在 Microsoft 数据或资源发生更改时Graph更改通知。
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 8f2e1524c63ceb77b092f0699f7bf1002a8420b0
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366918"
---
# <a name="create-subscription"></a><span data-ttu-id="37433-103">创建订阅</span><span class="sxs-lookup"><span data-stu-id="37433-103">Create subscription</span></span>

<span data-ttu-id="37433-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37433-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37433-105">订阅侦听器应用程序，以在 Microsoft Graph 中指定资源发生的更改属于请求的更改类型时接收更改通知。</span><span class="sxs-lookup"><span data-stu-id="37433-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

<span data-ttu-id="37433-106">请参阅" [权限](#permissions) 部分中的表格，了解支持订阅以更改通知的资源列表。</span><span class="sxs-lookup"><span data-stu-id="37433-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="37433-107">权限</span><span class="sxs-lookup"><span data-stu-id="37433-107">Permissions</span></span>

<span data-ttu-id="37433-108">创建订阅需要对资源的读取权限。</span><span class="sxs-lookup"><span data-stu-id="37433-108">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="37433-109">例如，若要获取邮件更改通知，您的应用程序需要 Mail.Read 权限。</span><span class="sxs-lookup"><span data-stu-id="37433-109">For example, to get change notifications on messages, your app needs the Mail.Read permission.</span></span> 

<span data-ttu-id="37433-110">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="37433-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="37433-111">若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="37433-111">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="37433-112">支持的资源</span><span class="sxs-lookup"><span data-stu-id="37433-112">Supported resource</span></span> | <span data-ttu-id="37433-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="37433-113">Delegated (work or school account)</span></span> | <span data-ttu-id="37433-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="37433-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37433-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="37433-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="37433-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="37433-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="37433-117">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-117">Not supported</span></span> | <span data-ttu-id="37433-118">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-118">Not supported</span></span> | <span data-ttu-id="37433-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="37433-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="37433-120">[channels](../resources/channel.md) (/teams/getAllChannels – 组织中所有频道) </span><span class="sxs-lookup"><span data-stu-id="37433-120">[channels](../resources/channel.md) (/teams/getAllChannels – all channels in an organization)</span></span> | <span data-ttu-id="37433-121">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-121">Not supported</span></span>  | <span data-ttu-id="37433-122">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-122">Not supported</span></span> | <span data-ttu-id="37433-123">Channel.ReadBasic.All，ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="37433-123">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span> |
|<span data-ttu-id="37433-124">[频道 (](../resources/channel.md) /teams/{id}/channels) </span><span class="sxs-lookup"><span data-stu-id="37433-124">[channels](../resources/channel.md) (/teams/{id}/channels)</span></span> | <span data-ttu-id="37433-125">Channel.ReadBasic.All，ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="37433-125">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  | <span data-ttu-id="37433-126">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-126">Not supported</span></span> | <span data-ttu-id="37433-127">Channel.ReadBasic.All，ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="37433-127">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  |
|<span data-ttu-id="37433-128">[chat](../resources/chat.md) (/chats – 组织内部的所有) </span><span class="sxs-lookup"><span data-stu-id="37433-128">[chat](../resources/chat.md) (/chats – all chats in an organization)</span></span> | <span data-ttu-id="37433-129">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-129">Not supported</span></span> | <span data-ttu-id="37433-130">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-130">Not supported</span></span> | <span data-ttu-id="37433-131">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37433-131">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="37433-132">[chat](../resources/chat.md) (/chats/{id}) </span><span class="sxs-lookup"><span data-stu-id="37433-132">[chat](../resources/chat.md) (/chats/{id})</span></span> | <span data-ttu-id="37433-133">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37433-133">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="37433-134">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-134">Not supported</span></span> | <span data-ttu-id="37433-135">ChatSettings.Read.Chat *、ChatSettings.ReadWrite.Chat*、Chat.Manage.Chat\*、Chat.ReadBasic.All、Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37433-135">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="37433-136">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="37433-136">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="37433-137">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37433-137">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="37433-138">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-138">Not supported</span></span> | <span data-ttu-id="37433-139">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="37433-139">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="37433-140">[chatMessage](../resources/chatmessage.md)（/teams/getAllMessages -- 组织中所有频道消息）</span><span class="sxs-lookup"><span data-stu-id="37433-140">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="37433-141">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-141">Not supported</span></span> | <span data-ttu-id="37433-142">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-142">Not supported</span></span> | <span data-ttu-id="37433-143">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="37433-143">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="37433-144">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="37433-144">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="37433-145">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37433-145">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="37433-146">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-146">Not supported</span></span> | <span data-ttu-id="37433-147">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="37433-147">Chat.Read.All</span></span>  |
|<span data-ttu-id="37433-148">[chatMessage](../resources/chatmessage.md)（/chats/getAllMessages -- 组织中所有聊天消息）</span><span class="sxs-lookup"><span data-stu-id="37433-148">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="37433-149">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-149">Not supported</span></span> | <span data-ttu-id="37433-150">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-150">Not supported</span></span> | <span data-ttu-id="37433-151">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="37433-151">Chat.Read.All</span></span>  |
|[<span data-ttu-id="37433-152">contact</span><span class="sxs-lookup"><span data-stu-id="37433-152">contact</span></span>](../resources/contact.md) | <span data-ttu-id="37433-153">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="37433-153">Contacts.Read</span></span> | <span data-ttu-id="37433-154">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="37433-154">Contacts.Read</span></span> | <span data-ttu-id="37433-155">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="37433-155">Contacts.Read</span></span> |
|<span data-ttu-id="37433-156">[conversationMember](../resources/conversationmember.md) (/chats/getAllMembers) </span><span class="sxs-lookup"><span data-stu-id="37433-156">[conversationMember](../resources/conversationmember.md) (/chats/getAllMembers)</span></span> | <span data-ttu-id="37433-157">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-157">Not supported</span></span> | <span data-ttu-id="37433-158">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-158">Not supported</span></span> | <span data-ttu-id="37433-159">ChatMember.Read.All、ChatMember.ReadWrite.All、Chat.ReadBasic.All、Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37433-159">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="37433-160">[conversationMember](../resources/conversationmember.md) (/chats/{id}/members) </span><span class="sxs-lookup"><span data-stu-id="37433-160">[conversationMember](../resources/conversationmember.md) (/chats/{id}/members)</span></span> | <span data-ttu-id="37433-161">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37433-161">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="37433-162">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-162">Not supported</span></span> | <span data-ttu-id="37433-163">ChatMember.Read.Chat *、Chat.Manage.Chat*、ChatMember.Read.All、ChatMember.ReadWrite.All、Chat.ReadBasic.All、Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37433-163">ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="37433-164">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members) </span><span class="sxs-lookup"><span data-stu-id="37433-164">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span></span> | <span data-ttu-id="37433-165">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="37433-165">TeamMember.Read.All</span></span> | <span data-ttu-id="37433-166">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-166">Not supported</span></span> | <span data-ttu-id="37433-167">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="37433-167">TeamMember.Read.All</span></span> |
|<span data-ttu-id="37433-168">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="37433-168">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="37433-169">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-169">Not supported</span></span> | <span data-ttu-id="37433-170">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37433-170">Files.ReadWrite</span></span> | <span data-ttu-id="37433-171">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-171">Not supported</span></span> |
|<span data-ttu-id="37433-172">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="37433-172">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="37433-173">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37433-173">Files.ReadWrite.All</span></span> | <span data-ttu-id="37433-174">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-174">Not supported</span></span> | <span data-ttu-id="37433-175">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37433-175">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="37433-176">事件</span><span class="sxs-lookup"><span data-stu-id="37433-176">event</span></span>](../resources/event.md) | <span data-ttu-id="37433-177">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="37433-177">Calendars.Read</span></span> | <span data-ttu-id="37433-178">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="37433-178">Calendars.Read</span></span> | <span data-ttu-id="37433-179">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="37433-179">Calendars.Read</span></span> |
|[<span data-ttu-id="37433-180">组</span><span class="sxs-lookup"><span data-stu-id="37433-180">group</span></span>](../resources/group.md) | <span data-ttu-id="37433-181">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="37433-181">Group.Read.All</span></span> | <span data-ttu-id="37433-182">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-182">Not supported</span></span> | <span data-ttu-id="37433-183">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="37433-183">Group.Read.All</span></span> |
|[<span data-ttu-id="37433-184">组对话</span><span class="sxs-lookup"><span data-stu-id="37433-184">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="37433-185">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="37433-185">Group.Read.All</span></span> | <span data-ttu-id="37433-186">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-186">Not supported</span></span> | <span data-ttu-id="37433-187">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-187">Not supported</span></span> |
|[<span data-ttu-id="37433-188">列表</span><span class="sxs-lookup"><span data-stu-id="37433-188">list</span></span>](../resources/list.md) | <span data-ttu-id="37433-189">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37433-189">Sites.ReadWrite.All</span></span> | <span data-ttu-id="37433-190">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-190">Not supported</span></span> | <span data-ttu-id="37433-191">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37433-191">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="37433-192">邮件</span><span class="sxs-lookup"><span data-stu-id="37433-192">message</span></span>](../resources/message.md) | <span data-ttu-id="37433-193">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="37433-193">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="37433-194">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="37433-194">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="37433-195">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="37433-195">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="37433-196">状态</span><span class="sxs-lookup"><span data-stu-id="37433-196">presence</span></span>](../resources/presence.md) | <span data-ttu-id="37433-197">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="37433-197">Presence.Read.All</span></span> | <span data-ttu-id="37433-198">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-198">Not supported</span></span> | <span data-ttu-id="37433-199">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-199">Not supported</span></span> |
|[<span data-ttu-id="37433-200">打印机</span><span class="sxs-lookup"><span data-stu-id="37433-200">printer</span></span>](../resources/printer.md) | <span data-ttu-id="37433-201">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-201">Not supported</span></span> | <span data-ttu-id="37433-202">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-202">Not supported</span></span> | <span data-ttu-id="37433-203">打印机。阅读.All，Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37433-203">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="37433-204">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="37433-204">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="37433-205">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-205">Not supported</span></span> | <span data-ttu-id="37433-206">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-206">Not supported</span></span> | <span data-ttu-id="37433-207">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37433-207">PrintTaskDefinition.ReadWrite.All</span></span> |
|<span data-ttu-id="37433-208">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="37433-208">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="37433-209">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37433-209">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="37433-210">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-210">Not supported</span></span> | <span data-ttu-id="37433-211">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37433-211">SecurityEvents.ReadWrite.All</span></span> |
|<span data-ttu-id="37433-212">[teams](../resources/team.md) (/teams – 组织内部的所有) </span><span class="sxs-lookup"><span data-stu-id="37433-212">[teams](../resources/team.md) (/teams – all teams in an organization)</span></span> | <span data-ttu-id="37433-213">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-213">Not supported</span></span> | <span data-ttu-id="37433-214">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-214">Not supported</span></span> | <span data-ttu-id="37433-215">Team.ReadBasic.All，TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="37433-215">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|<span data-ttu-id="37433-216">[teams](../resources/team.md) (/teams/{id}) </span><span class="sxs-lookup"><span data-stu-id="37433-216">[teams](../resources/team.md) (/teams/{id})</span></span> | <span data-ttu-id="37433-217">Team.ReadBasic.All，TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="37433-217">Team.ReadBasic.All, TeamSettings.Read.All</span></span> | <span data-ttu-id="37433-218">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-218">Not supported</span></span> | <span data-ttu-id="37433-219">Team.ReadBasic.All，TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="37433-219">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|[<span data-ttu-id="37433-220">todoTask</span><span class="sxs-lookup"><span data-stu-id="37433-220">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="37433-221">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37433-221">Tasks.ReadWrite</span></span> | <span data-ttu-id="37433-222">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37433-222">Tasks.ReadWrite</span></span> | <span data-ttu-id="37433-223">不支持</span><span class="sxs-lookup"><span data-stu-id="37433-223">Not supported</span></span> |
|[<span data-ttu-id="37433-224">用户</span><span class="sxs-lookup"><span data-stu-id="37433-224">user</span></span>](../resources/user.md) | <span data-ttu-id="37433-225">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="37433-225">User.Read.All</span></span> | <span data-ttu-id="37433-226">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="37433-226">User.Read.All</span></span> | <span data-ttu-id="37433-227">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="37433-227">User.Read.All</span></span> |

> <span data-ttu-id="37433-228">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="37433-228">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="37433-229">driveItem</span><span class="sxs-lookup"><span data-stu-id="37433-229">driveItem</span></span>

<span data-ttu-id="37433-230">其他限制适用于 OneDrive 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="37433-230">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="37433-231">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="37433-231">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="37433-232">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="37433-232">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="37433-233">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="37433-233">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="37433-234">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送更改通知。</span><span class="sxs-lookup"><span data-stu-id="37433-234">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="37433-235">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="37433-235">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

<span data-ttu-id="37433-236">OneDrive for Business 和 SharePoint 支持向应用程序发送有关在 **driveItem** 上发生的安全事件通知。</span><span class="sxs-lookup"><span data-stu-id="37433-236">OneDrive for Business and SharePoint support sending your application notifications of security events that occur on a **driveItem**.</span></span> <span data-ttu-id="37433-237">若要订阅这些事件，请为请求添加 `prefer:includesecuritywebhooks` 标头以创建订阅。</span><span class="sxs-lookup"><span data-stu-id="37433-237">To subscribe to these events, add the `prefer:includesecuritywebhooks` header to your request to create a subscription.</span></span> <span data-ttu-id="37433-238">创建订阅后，当项目权限更改时，你将收到通知。</span><span class="sxs-lookup"><span data-stu-id="37433-238">After the subscription is created, you will receive notifications when the permissions on an item change.</span></span> <span data-ttu-id="37433-239">此标头适用于 SharePoint 和 OneDrive for Business 帐户，但不适用于 OneDrive 消费者版本的帐户。</span><span class="sxs-lookup"><span data-stu-id="37433-239">This header is applicable to SharePoint and OneDrive for Business but not consumer OneDrive accounts.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="37433-240">联系人、事件和消息</span><span class="sxs-lookup"><span data-stu-id="37433-240">contact, event, and message</span></span>

<span data-ttu-id="37433-241">其他限制适用于 Outlook 项目的订阅。</span><span class="sxs-lookup"><span data-stu-id="37433-241">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="37433-242">这些限制适用于订阅的创建和管理（获取、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="37433-242">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="37433-243">委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="37433-243">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="37433-244">例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="37433-244">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="37433-245">订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="37433-245">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="37433-246">使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="37433-246">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="37433-247">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="37433-247">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="37433-248">状态</span><span class="sxs-lookup"><span data-stu-id="37433-248">presence</span></span>

<span data-ttu-id="37433-249">**状态** 订阅需要 [加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="37433-249">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="37433-250">如果未指定 [encryptionCertificate](../resources/subscription.md)，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="37433-250">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="37433-251">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="37433-251">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="37433-252">请求标头</span><span class="sxs-lookup"><span data-stu-id="37433-252">Request headers</span></span>

| <span data-ttu-id="37433-253">名称</span><span class="sxs-lookup"><span data-stu-id="37433-253">Name</span></span>       | <span data-ttu-id="37433-254">类型</span><span class="sxs-lookup"><span data-stu-id="37433-254">Type</span></span> | <span data-ttu-id="37433-255">说明</span><span class="sxs-lookup"><span data-stu-id="37433-255">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="37433-256">Authorization</span><span class="sxs-lookup"><span data-stu-id="37433-256">Authorization</span></span>  | <span data-ttu-id="37433-257">string</span><span class="sxs-lookup"><span data-stu-id="37433-257">string</span></span>  | <span data-ttu-id="37433-p109">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="37433-p109">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="37433-260">响应</span><span class="sxs-lookup"><span data-stu-id="37433-260">Response</span></span>

<span data-ttu-id="37433-261">如果成功，此方法在响应 `201 Created` 正文中返回 [响应](../resources/subscription.md) 代码和 subscription 对象。</span><span class="sxs-lookup"><span data-stu-id="37433-261">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="37433-262">要详细了解错误返回方式，请参阅[错误响应][error-response]。</span><span class="sxs-lookup"><span data-stu-id="37433-262">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="37433-263">示例</span><span class="sxs-lookup"><span data-stu-id="37433-263">Example</span></span>

### <a name="request"></a><span data-ttu-id="37433-264">请求</span><span class="sxs-lookup"><span data-stu-id="37433-264">Request</span></span>

<span data-ttu-id="37433-265">在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37433-265">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="37433-266">`clientState` 和 `latestSupportedTlsVersion` 是可选字段。</span><span class="sxs-lookup"><span data-stu-id="37433-266">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="37433-267">此请求为当前登录用户收到的新邮件更改通知创建订阅。</span><span class="sxs-lookup"><span data-stu-id="37433-267">This request creates a subscription for change notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="37433-268">HTTP</span><span class="sxs-lookup"><span data-stu-id="37433-268">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="37433-269">C#</span><span class="sxs-lookup"><span data-stu-id="37433-269">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37433-270">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37433-270">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37433-271">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37433-271">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37433-272">Java</span><span class="sxs-lookup"><span data-stu-id="37433-272">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="37433-273">在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37433-273">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="37433-274">`clientState` 和 `latestSupportedTlsVersion` 是可选字段。</span><span class="sxs-lookup"><span data-stu-id="37433-274">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

#### <a name="resources-examples"></a><span data-ttu-id="37433-275">资源示例</span><span class="sxs-lookup"><span data-stu-id="37433-275">Resources examples</span></span>

<span data-ttu-id="37433-276">以下是资源属性的有效值。</span><span class="sxs-lookup"><span data-stu-id="37433-276">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="37433-277">资源类型</span><span class="sxs-lookup"><span data-stu-id="37433-277">Resource type</span></span> | <span data-ttu-id="37433-278">示例</span><span class="sxs-lookup"><span data-stu-id="37433-278">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="37433-279">通话记录</span><span class="sxs-lookup"><span data-stu-id="37433-279">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="37433-280">频道</span><span class="sxs-lookup"><span data-stu-id="37433-280">Channels</span></span>](../resources/channel.md)|<span data-ttu-id="37433-281">`/teams/getAllChannels`, `/teams/{id}/channels`</span><span class="sxs-lookup"><span data-stu-id="37433-281">`/teams/getAllChannels`, `/teams/{id}/channels`</span></span>|
|[<span data-ttu-id="37433-282">聊天</span><span class="sxs-lookup"><span data-stu-id="37433-282">Chat</span></span>](../resources/chat.md)|<span data-ttu-id="37433-283">`/chats`, `/chats/{id}`</span><span class="sxs-lookup"><span data-stu-id="37433-283">`/chats`, `/chats/{id}`</span></span>|
|[<span data-ttu-id="37433-284">聊天消息</span><span class="sxs-lookup"><span data-stu-id="37433-284">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="37433-285">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="37433-285">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="37433-286">联系人</span><span class="sxs-lookup"><span data-stu-id="37433-286">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="37433-287">ConversationMember</span><span class="sxs-lookup"><span data-stu-id="37433-287">ConversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="37433-288">`/chats/{id}/members`, `/chats/getAllMembers`, `/teams/{id}/members`</span><span class="sxs-lookup"><span data-stu-id="37433-288">`/chats/{id}/members`, `/chats/getAllMembers`, `/teams/{id}/members`</span></span>|
|[<span data-ttu-id="37433-289">对话</span><span class="sxs-lookup"><span data-stu-id="37433-289">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="37433-290">驱动器</span><span class="sxs-lookup"><span data-stu-id="37433-290">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="37433-291">事件</span><span class="sxs-lookup"><span data-stu-id="37433-291">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="37433-292">组</span><span class="sxs-lookup"><span data-stu-id="37433-292">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="37433-293">列表</span><span class="sxs-lookup"><span data-stu-id="37433-293">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="37433-294">邮件</span><span class="sxs-lookup"><span data-stu-id="37433-294">Mail</span></span>](../resources/message.md)|<span data-ttu-id="37433-295">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="37433-295">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="37433-296">状态</span><span class="sxs-lookup"><span data-stu-id="37433-296">Presence</span></span>](../resources/presence.md)| <span data-ttu-id="37433-297">`/communications/presences/{id}` (单个用户) ， (`/communications/presences?$filter=id in ({id},{id}…)` 多个) </span><span class="sxs-lookup"><span data-stu-id="37433-297">`/communications/presences/{id}` (single user), `/communications/presences?$filter=id in ({id},{id}…)` (multiple users)</span></span>|
|[<span data-ttu-id="37433-298">打印机</span><span class="sxs-lookup"><span data-stu-id="37433-298">printer</span></span>](../resources/printer.md) |`print/printers/{id}/jobs`|
|[<span data-ttu-id="37433-299">PrintTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="37433-299">PrintTaskDefinition</span></span>](../resources/printtaskdefinition.md)|`print/taskDefinitions/{id}/tasks`|
|[<span data-ttu-id="37433-300">Teams</span><span class="sxs-lookup"><span data-stu-id="37433-300">Teams</span></span>](../resources/team.md)|<span data-ttu-id="37433-301">`/teams`, `/teams/{id}`</span><span class="sxs-lookup"><span data-stu-id="37433-301">`/teams`, `/teams/{id}`</span></span>|
|[<span data-ttu-id="37433-302">用户</span><span class="sxs-lookup"><span data-stu-id="37433-302">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="37433-303">todoTask</span><span class="sxs-lookup"><span data-stu-id="37433-303">todoTask</span></span>](../resources/todotask.md) | `/me/todo/lists/{todoTaskListId}/tasks`
|[<span data-ttu-id="37433-304">安全警报</span><span class="sxs-lookup"><span data-stu-id="37433-304">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'NewAlert'`|

> <span data-ttu-id="37433-305">**注意：** 以 `me` 开头的任何路径也可与 `users/{id}`（而不是 `me`）一起使用，从而以特定用户为目标，而不是以当前用户为目标。</span><span class="sxs-lookup"><span data-stu-id="37433-305">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

### <a name="response"></a><span data-ttu-id="37433-306">响应</span><span class="sxs-lookup"><span data-stu-id="37433-306">Response</span></span>

<span data-ttu-id="37433-307">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="37433-307">The following example shows the response.</span></span> 

><span data-ttu-id="37433-308">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="37433-308">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="notification-endpoint-validation"></a><span data-ttu-id="37433-309">通知终结点验证</span><span class="sxs-lookup"><span data-stu-id="37433-309">Notification endpoint validation</span></span>

<span data-ttu-id="37433-310">notificationUrl (中指定的订阅通知终结点) 必须能够响应验证请求，如设置用户数据更改[的通知中所述](/graph/webhooks#notification-endpoint-validation)。</span><span class="sxs-lookup"><span data-stu-id="37433-310">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="37433-311">如果验证失败，创建订阅请求返回错误“400 请求无效”。</span><span class="sxs-lookup"><span data-stu-id="37433-311">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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


