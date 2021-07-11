---
title: 使用 Microsoft Graph API 获取更改通知
description: 为客户提供更改通知。
localization_priority: Normal
author: Jumaodhiss
doc_type: conceptualPageType
ms.prod: change-notifications
ms.openlocfilehash: 141d51a7e497124359b6d4cc78dfd0ba39b05f08
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366497"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="5ee72-103">使用 Microsoft Graph API 获取更改通知</span><span class="sxs-lookup"><span data-stu-id="5ee72-103">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="5ee72-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ee72-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ee72-105">Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。</span><span class="sxs-lookup"><span data-stu-id="5ee72-105">The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="5ee72-106">客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。</span><span class="sxs-lookup"><span data-stu-id="5ee72-106">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="5ee72-107">客户端应用使用通知在更改时更新其状态。</span><span class="sxs-lookup"><span data-stu-id="5ee72-107">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="5ee72-108">有关详细信息（包括如何订阅和处理传入通知），请参阅[设置用户数据更改的通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="5ee72-108">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="5ee72-109">使用 Microsoft Graph API，应用可以订阅以下资源的更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-109">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

| <span data-ttu-id="5ee72-110">**资源**</span><span class="sxs-lookup"><span data-stu-id="5ee72-110">**Resource**</span></span> | <span data-ttu-id="5ee72-111">**支持的资源路径**</span><span class="sxs-lookup"><span data-stu-id="5ee72-111">**Supported resource paths**</span></span> | <span data-ttu-id="5ee72-112">**可包含在通知中的资源数据**</span><span class="sxs-lookup"><span data-stu-id="5ee72-112">**Resource data can be included in notifications**</span></span>                  |
|:----------------|:------------|:-----------------------------------------|
| <span data-ttu-id="5ee72-113">云打印 [打印机][]</span><span class="sxs-lookup"><span data-stu-id="5ee72-113">Cloud printing [printer][]</span></span> | <span data-ttu-id="5ee72-114">打印作业准备好下载时的变化（作业可打印事件）：</span><span class="sxs-lookup"><span data-stu-id="5ee72-114">Changes when a print job is ready to be downloaded (JobFetchable event):</span></span><br>`/print/printers/{id}/jobs` | <span data-ttu-id="5ee72-115">不支持</span><span class="sxs-lookup"><span data-stu-id="5ee72-115">No</span></span> |
| <span data-ttu-id="5ee72-116">云打印 [printTaskDefinition][]</span><span class="sxs-lookup"><span data-stu-id="5ee72-116">Cloud printing [printTaskDefinition][]</span></span> | <span data-ttu-id="5ee72-117">在队列中具有有效作业时的变化（作业启动事件）：</span><span class="sxs-lookup"><span data-stu-id="5ee72-117">Changes when there is a valid job in the queue (JobStarted event) :</span></span><br>`/print/printtaskdefinition/{id}/tasks` | <span data-ttu-id="5ee72-118">否</span><span class="sxs-lookup"><span data-stu-id="5ee72-118">No</span></span> |
| <span data-ttu-id="5ee72-119">OneDrive for Business 上的 [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="5ee72-119">[driveItem][] on OneDrive for Business</span></span> | <span data-ttu-id="5ee72-120">对 _根文件夹_ 的层次结构内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-120">Changes to content within the hierarchy of the _root folder_:</span></span><br>`/drives/{id}/root`<br> `/users/{id}/drive/root` | <span data-ttu-id="5ee72-121">否</span><span class="sxs-lookup"><span data-stu-id="5ee72-121">No</span></span> |
| <span data-ttu-id="5ee72-122">OneDrive（个人版）上的 [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="5ee72-122">[driveItem][] on OneDrive (personal)</span></span> | <span data-ttu-id="5ee72-123">对 _任何文件夹_ 的层次结构内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-123">Changes to content within the hierarchy of _any folder_:</span></span><br>`/users/{id}/drive/root` | <span data-ttu-id="5ee72-124">否</span><span class="sxs-lookup"><span data-stu-id="5ee72-124">No</span></span> |
| <span data-ttu-id="5ee72-125">[组][]</span><span class="sxs-lookup"><span data-stu-id="5ee72-125">[group][]</span></span> | <span data-ttu-id="5ee72-126">对所有组更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-126">Changes to all groups:</span></span><br>`/groups` <br><span data-ttu-id="5ee72-127">对特定组更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-127">Changes to a specific group:</span></span><br>`/groups/{id}`<br><span data-ttu-id="5ee72-128">对特定组的所有者所做的更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-128">Changes to owners of a specific group:</span></span><br>`/groups/{id}/owners`<br><span data-ttu-id="5ee72-129">对特定组成员所做的更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-129">Changes to members of a specific group:</span></span><br>`/groups/{id}/members` | <span data-ttu-id="5ee72-130">否</span><span class="sxs-lookup"><span data-stu-id="5ee72-130">No</span></span> |
| <span data-ttu-id="5ee72-131">SharePoint [网站][]下的[列表][]</span><span class="sxs-lookup"><span data-stu-id="5ee72-131">[list][] under a SharePoint [site][]</span></span> | `/sites/{id}/lists/{id}` | <span data-ttu-id="5ee72-132">否</span><span class="sxs-lookup"><span data-stu-id="5ee72-132">No</span></span> |
| <span data-ttu-id="5ee72-133">Microsoft 365 组[对话][]</span><span class="sxs-lookup"><span data-stu-id="5ee72-133">Microsoft 365 group [conversation][]</span></span> | <span data-ttu-id="5ee72-134">查看组的对话：</span><span class="sxs-lookup"><span data-stu-id="5ee72-134">Changes to a group's conversations:</span></span><br>`groups/{id}/conversations` | <span data-ttu-id="5ee72-135">否</span><span class="sxs-lookup"><span data-stu-id="5ee72-135">No</span></span> |
| <span data-ttu-id="5ee72-136">Outlook [事件][]</span><span class="sxs-lookup"><span data-stu-id="5ee72-136">Outlook [event][]</span></span> | <span data-ttu-id="5ee72-137">对用户邮箱中的所有事件更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-137">Changes to all events in a user's mailbox:</span></span><br>`/users/{id}/events` | <span data-ttu-id="5ee72-138">否</span><span class="sxs-lookup"><span data-stu-id="5ee72-138">No</span></span> |
| <span data-ttu-id="5ee72-139">Outlook [邮件][]</span><span class="sxs-lookup"><span data-stu-id="5ee72-139">Outlook [message][]</span></span> | <span data-ttu-id="5ee72-140">对用户邮箱中的所有邮件更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-140">Changes to all messages in a user's mailbox:</span></span> <br>`/users/{id}/messages`<br><span data-ttu-id="5ee72-141">对用户收件箱中的所有邮件更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-141">Changes to messages in a user's Inbox:</span></span><br>`/users/{id}/mailFolders('inbox')/messages` | <span data-ttu-id="5ee72-142">否</span><span class="sxs-lookup"><span data-stu-id="5ee72-142">No</span></span> |
| <span data-ttu-id="5ee72-143">Outlook 个人[联系人][]</span><span class="sxs-lookup"><span data-stu-id="5ee72-143">Outlook personal [contact][]</span></span> | <span data-ttu-id="5ee72-144">对用户邮箱中的所有个人联系人更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-144">Changes to all personal contacts in a user's mailbox:</span></span><br>`/users/{id}/contacts` | <span data-ttu-id="5ee72-145">否</span><span class="sxs-lookup"><span data-stu-id="5ee72-145">No</span></span> |
| <span data-ttu-id="5ee72-146">安全[警报][]</span><span class="sxs-lookup"><span data-stu-id="5ee72-146">Security [alert][]</span></span> | <span data-ttu-id="5ee72-147">对特定警报更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-147">Changes to a specific alert:</span></span><br>`/security/alerts/{id}` <br><span data-ttu-id="5ee72-148">对已筛选的警报更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-148">Changes to filtered alerts:</span></span><br> `/security/alerts/?$filter`| <span data-ttu-id="5ee72-149">否</span><span class="sxs-lookup"><span data-stu-id="5ee72-149">No</span></span> |
| <span data-ttu-id="5ee72-150">Teams [callRecord][]</span><span class="sxs-lookup"><span data-stu-id="5ee72-150">Teams [callRecord][]</span></span> | <span data-ttu-id="5ee72-151">更改 _所有_ 呼叫记录： `/communications/callRecords`</span><span class="sxs-lookup"><span data-stu-id="5ee72-151">Changes to _all_ call records: `/communications/callRecords`</span></span> | <span data-ttu-id="5ee72-152">否</span><span class="sxs-lookup"><span data-stu-id="5ee72-152">No</span></span> |
| <span data-ttu-id="5ee72-153">Teams [频道][]</span><span class="sxs-lookup"><span data-stu-id="5ee72-153">Teams [channel][]</span></span> | <span data-ttu-id="5ee72-154">更改所有团队中的频道：</span><span class="sxs-lookup"><span data-stu-id="5ee72-154">Changes to channels in all teams:</span></span><br>`/teams/getAllChannels` <br><span data-ttu-id="5ee72-155">对特定团队中的频道的更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-155">Changes to channel in a specific team:</span></span><br>`/teams/{id}/channels` | <span data-ttu-id="5ee72-156">是</span><span class="sxs-lookup"><span data-stu-id="5ee72-156">Yes</span></span> |
| <span data-ttu-id="5ee72-157">Teams[聊天][]</span><span class="sxs-lookup"><span data-stu-id="5ee72-157">Teams [chat][]</span></span> | <span data-ttu-id="5ee72-158">对租户中任何聊天的更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-158">Changes to any chat in the tenant:</span></span><br>`/chats` <br><span data-ttu-id="5ee72-159">对特定聊天的更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-159">Changes to a specific chat:</span></span><br>`/chats/{id}` | <span data-ttu-id="5ee72-160">是</span><span class="sxs-lookup"><span data-stu-id="5ee72-160">Yes</span></span> |
| <span data-ttu-id="5ee72-161">Teams [chatmessage][]</span><span class="sxs-lookup"><span data-stu-id="5ee72-161">Teams [chatmessage][]</span></span> | <span data-ttu-id="5ee72-162">对所有团队中所有频道聊天消息更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-162">Changes to chat messages in all channels in all teams:</span></span><br>`/teams/getAllMessages` <br><span data-ttu-id="5ee72-163">对特定频道中的聊天消息更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-163">Changes to chat messages in a specific channel:</span></span><br>`/teams/{id}/channels/{id}/messages`<br><span data-ttu-id="5ee72-164">对所有聊天的消息更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-164">Changes to chat messages in all chats:</span></span><br>`/chats/getAllMessages` <br><span data-ttu-id="5ee72-165">对特定聊天中的消息更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-165">Changes to chat messages in a specific chat:</span></span><br>`/chats/{id}/messages` | <span data-ttu-id="5ee72-166">是</span><span class="sxs-lookup"><span data-stu-id="5ee72-166">Yes</span></span> |
| <span data-ttu-id="5ee72-167">Teams [conversationMember][]</span><span class="sxs-lookup"><span data-stu-id="5ee72-167">Teams [conversationMember][]</span></span> | <span data-ttu-id="5ee72-168">对特定团队中的成员身份的更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-168">Changes to membership in a specific team:</span></span><br>`/teams/{id}/members` <br> <span data-ttu-id="5ee72-169">对特定聊天中的成员身份的更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-169">Changes to membership in a specific chat:</span></span><br>`/chats/{id}/members` <br> <span data-ttu-id="5ee72-170">更改所有聊天中的成员身份：</span><span class="sxs-lookup"><span data-stu-id="5ee72-170">Changes to membership in all chats:</span></span><br>`/chats/getAllMembers` | <span data-ttu-id="5ee72-171">是</span><span class="sxs-lookup"><span data-stu-id="5ee72-171">Yes</span></span> |
| <span data-ttu-id="5ee72-172">Teams[状态][]</span><span class="sxs-lookup"><span data-stu-id="5ee72-172">Teams [presence][]</span></span> | <span data-ttu-id="5ee72-173">对单个用户状态所做的更改： `/communications/presences/{id}`</span><span class="sxs-lookup"><span data-stu-id="5ee72-173">Changes to a single user's presence: `/communications/presences/{id}`</span></span> <br> <span data-ttu-id="5ee72-174">对多个用户状态所做的更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-174">Changes to multiple user presences:</span></span><br> `/communications/presences?$filter=id in ({id},{id}...)` | <span data-ttu-id="5ee72-175">是</span><span class="sxs-lookup"><span data-stu-id="5ee72-175">Yes</span></span> |
| <span data-ttu-id="5ee72-176">Teams [团队][]</span><span class="sxs-lookup"><span data-stu-id="5ee72-176">Teams [team][]</span></span> | <span data-ttu-id="5ee72-177">对租户中任何团队的更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-177">Changes to any team in the tenant:</span></span><br>`/teams` <br><span data-ttu-id="5ee72-178">对特定团队的更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-178">Changes to a specific team:</span></span><br>`/teams/{id}` | <span data-ttu-id="5ee72-179">是</span><span class="sxs-lookup"><span data-stu-id="5ee72-179">Yes</span></span> |
| <span data-ttu-id="5ee72-180">[todoTask][]</span><span class="sxs-lookup"><span data-stu-id="5ee72-180">[todoTask][]</span></span> | <span data-ttu-id="5ee72-181">对特定任务列表中所有任务的更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-181">Changes to all task in a specific task list:</span></span><br>`/me/todo/lists/{todoTaskListId}/tasks` | <span data-ttu-id="5ee72-182">否</span><span class="sxs-lookup"><span data-stu-id="5ee72-182">No</span></span> |
| <span data-ttu-id="5ee72-183">[用户][]</span><span class="sxs-lookup"><span data-stu-id="5ee72-183">[user][]</span></span> | <span data-ttu-id="5ee72-184">对所有用户更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-184">Changes to all users:</span></span><br>`/users` <br><span data-ttu-id="5ee72-185">对特定用户更改：</span><span class="sxs-lookup"><span data-stu-id="5ee72-185">Changes to a specific user:</span></span><br>`/users/{id}`| <span data-ttu-id="5ee72-186">否</span><span class="sxs-lookup"><span data-stu-id="5ee72-186">No</span></span> |


> <span data-ttu-id="5ee72-187">**注意**：以 `/users/{id}` 开头的任何资源路径还可接受 `/me` 以引用已登录的用户。</span><span class="sxs-lookup"><span data-stu-id="5ee72-187">**Note**: Any resource path that begins with `/users/{id}` can also accept `/me` to reference the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ee72-188">权限</span><span class="sxs-lookup"><span data-stu-id="5ee72-188">Permissions</span></span>

<span data-ttu-id="5ee72-189">通常订阅操作需要拥有对资源的读取权限。</span><span class="sxs-lookup"><span data-stu-id="5ee72-189">In general, subscription operations require read permission to the resource.</span></span> <span data-ttu-id="5ee72-190">例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。</span><span class="sxs-lookup"><span data-stu-id="5ee72-190">For example, to get notifications for messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="5ee72-191">[创建订阅](../api/subscription-post-subscriptions.md)一文列出了各个资源类型所需的权限。</span><span class="sxs-lookup"><span data-stu-id="5ee72-191">The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type.</span></span> <span data-ttu-id="5ee72-192">下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。</span><span class="sxs-lookup"><span data-stu-id="5ee72-192">The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="5ee72-193">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ee72-193">Permission type</span></span>                        | <span data-ttu-id="5ee72-194">支持的资源类型</span><span class="sxs-lookup"><span data-stu-id="5ee72-194">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="5ee72-195">委派 - 工作或学校帐户</span><span class="sxs-lookup"><span data-stu-id="5ee72-195">Delegated - work or school account</span></span>     | <span data-ttu-id="5ee72-196">[][]alert、channel、chat、contact、conversation、conversationMember、driveItem、list、event、group、message、user、presence、chatMessage (preview) ， [team][]， [todoTask][] [][] [][] [][] [][] [][] [][] [][] [][] [][] [][] [][] [][] [][]</span><span class="sxs-lookup"><span data-stu-id="5ee72-196">[alert][], [channel][], [chat][], [contact][], [conversation][], [conversationMember][], [driveItem][], [list][], [event][], [group][], [message][], [user][], [presence][], [chatMessage][] (preview), [team][], [todoTask][]</span></span> |
| <span data-ttu-id="5ee72-197">委派 - 个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="5ee72-197">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="5ee72-198">[contact][]、 [driveItem][]、 [list][]、 [event][]、 [message][]、[todoTask][]</span><span class="sxs-lookup"><span data-stu-id="5ee72-198">[contact][], [driveItem][], [list][], [event][], [message][],[todoTask][]</span></span>                                     |
| <span data-ttu-id="5ee72-199">应用程序</span><span class="sxs-lookup"><span data-stu-id="5ee72-199">Application</span></span>                            | <span data-ttu-id="5ee72-200">[][]alert、channel、chat、contact、driveItem、list、event、group、message、user、callRecord、chatMessage、conversationMember、printer、printTaskDefinition、team [][] [][] [][] [][] [][] [][] [][] [][] [][] [][] [][] [][] [][] [][] [][]</span><span class="sxs-lookup"><span data-stu-id="5ee72-200">[alert][], [channel][], [chat][], [contact][], [driveItem][], [list][], [event][], [group][], [message][], [user][], [callRecord][], [chatMessage][], [conversationMember][], [printer][], [printTaskDefinition][], [team][]</span></span> |

## <a name="see-also"></a><span data-ttu-id="5ee72-201">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5ee72-201">See also</span></span>

- [<span data-ttu-id="5ee72-202">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="5ee72-202">Subscription resource type</span></span>](subscription.md)
- [<span data-ttu-id="5ee72-203">列出订阅</span><span class="sxs-lookup"><span data-stu-id="5ee72-203">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="5ee72-204">获取订阅</span><span class="sxs-lookup"><span data-stu-id="5ee72-204">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="5ee72-205">创建订阅</span><span class="sxs-lookup"><span data-stu-id="5ee72-205">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="5ee72-206">更新订阅</span><span class="sxs-lookup"><span data-stu-id="5ee72-206">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="5ee72-207">删除订阅</span><span class="sxs-lookup"><span data-stu-id="5ee72-207">Delete subscription</span></span>](../api/subscription-delete.md)

[聊天]: ./chat.md
[chat]: ./chat.md
[chatMessage]: ./chatmessage.md
[contact]: ./contact.md
[对话]: ./conversation.md
[conversation]: ./conversation.md
[conversationMember]: ./conversationmember.md
[频道]: ./channel.md
[channel]: ./channel.md
[driveItem]: ./driveitem.md
[list]: ./list.md
[site]: ./site.md
[事件]: ./event.md
[event]: ./event.md
[组]: ./group.md
[group]: ./group.md
[邮件]: ./message.md
[message]: ./message.md
[用户]: ./user.md
[user]: ./user.md
[callRecord]: ./callrecords-callrecord.md
[警报]: ./alert.md
[alert]: ./alert.md
[状态]: ./presence.md
[presence]: ./presence.md
[打印机]: ./printer.md
[printer]: ./printer.md
[printTaskDefinition]: ./printtaskdefinition.md
[团队]: ./team.md
[team]: ./team.md
[todoTask]: ./todoTask.md

