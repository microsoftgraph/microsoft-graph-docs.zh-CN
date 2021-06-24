---
title: 使用 Microsoft Graph API 获取更改通知
description: 为客户提供更改通知。
localization_priority: Normal
author: Jumaodhiss
doc_type: conceptualPageType
ms.prod: change-notifications
ms.openlocfilehash: 59bcc9f45b34508197494da7bc807cadbf214deb
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107751"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="2a095-103">使用 Microsoft Graph API 获取更改通知</span><span class="sxs-lookup"><span data-stu-id="2a095-103">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="2a095-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a095-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a095-105">Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。</span><span class="sxs-lookup"><span data-stu-id="2a095-105">The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="2a095-106">客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。</span><span class="sxs-lookup"><span data-stu-id="2a095-106">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="2a095-107">客户端应用使用通知在更改时更新其状态。</span><span class="sxs-lookup"><span data-stu-id="2a095-107">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="2a095-108">有关详细信息（包括如何订阅和处理传入通知），请参阅[设置用户数据更改的通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="2a095-108">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="2a095-109">使用 Microsoft Graph API，应用可以订阅以下资源的更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-109">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

| <span data-ttu-id="2a095-110">**资源**</span><span class="sxs-lookup"><span data-stu-id="2a095-110">**Resource**</span></span> | <span data-ttu-id="2a095-111">**支持的资源路径**</span><span class="sxs-lookup"><span data-stu-id="2a095-111">**Supported resource paths**</span></span> | <span data-ttu-id="2a095-112">**可包含在通知中的资源数据**</span><span class="sxs-lookup"><span data-stu-id="2a095-112">**Resource data can be included in notifications**</span></span>                  |
|:----------------|:------------|:-----------------------------------------|
| <span data-ttu-id="2a095-113">云打印 [打印机][]</span><span class="sxs-lookup"><span data-stu-id="2a095-113">Cloud printing [printer][]</span></span> | <span data-ttu-id="2a095-114">打印作业准备好下载时的变化（作业可打印事件）：</span><span class="sxs-lookup"><span data-stu-id="2a095-114">Changes when a print job is ready to be downloaded (JobFetchable event):</span></span><br>`/print/printers/{id}/jobs` | <span data-ttu-id="2a095-115">不支持</span><span class="sxs-lookup"><span data-stu-id="2a095-115">No</span></span> |
| <span data-ttu-id="2a095-116">云打印 [printTaskDefinition][]</span><span class="sxs-lookup"><span data-stu-id="2a095-116">Cloud printing [printTaskDefinition][]</span></span> | <span data-ttu-id="2a095-117">在队列中具有有效作业时的变化（作业启动事件）：</span><span class="sxs-lookup"><span data-stu-id="2a095-117">Changes when there is a valid job in the queue (JobStarted event) :</span></span><br>`/print/printtaskdefinition/{id}/tasks` | <span data-ttu-id="2a095-118">否</span><span class="sxs-lookup"><span data-stu-id="2a095-118">No</span></span> |
| <span data-ttu-id="2a095-119">OneDrive for Business 上的 [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="2a095-119">[driveItem][] on OneDrive for Business</span></span> | <span data-ttu-id="2a095-120">对 _根文件夹_ 的层次结构内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-120">Changes to content within the hierarchy of the _root folder_:</span></span><br>`/drives/{id}/root`<br> `/users/{id}/drive/root` | <span data-ttu-id="2a095-121">否</span><span class="sxs-lookup"><span data-stu-id="2a095-121">No</span></span> |
| <span data-ttu-id="2a095-122">OneDrive（个人版）上的 [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="2a095-122">[driveItem][] on OneDrive (personal)</span></span> | <span data-ttu-id="2a095-123">对 _任何文件夹_ 的层次结构内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-123">Changes to content within the hierarchy of _any folder_:</span></span><br>`/users/{id}/drive/root` | <span data-ttu-id="2a095-124">否</span><span class="sxs-lookup"><span data-stu-id="2a095-124">No</span></span> |
| <span data-ttu-id="2a095-125">[组][]</span><span class="sxs-lookup"><span data-stu-id="2a095-125">[group][]</span></span> | <span data-ttu-id="2a095-126">对所有组更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-126">Changes to all groups:</span></span><br>`/groups` <br><span data-ttu-id="2a095-127">对特定组更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-127">Changes to a specific group:</span></span><br>`/groups/{id}`<br><span data-ttu-id="2a095-128">对特定组的所有者所做的更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-128">Changes to owners of a specific group:</span></span><br>`/groups/{id}/owners`<br><span data-ttu-id="2a095-129">对特定组成员所做的更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-129">Changes to members of a specific group:</span></span><br>`/groups/{id}/members` | <span data-ttu-id="2a095-130">否</span><span class="sxs-lookup"><span data-stu-id="2a095-130">No</span></span> |
| <span data-ttu-id="2a095-131">SharePoint [网站][]下的[列表][]</span><span class="sxs-lookup"><span data-stu-id="2a095-131">[list][] under a SharePoint [site][]</span></span> | `/sites/{id}/lists/{id}` | <span data-ttu-id="2a095-132">否</span><span class="sxs-lookup"><span data-stu-id="2a095-132">No</span></span> |
| <span data-ttu-id="2a095-133">Microsoft 365 组[对话][]</span><span class="sxs-lookup"><span data-stu-id="2a095-133">Microsoft 365 group [conversation][]</span></span> | <span data-ttu-id="2a095-134">查看组的对话：</span><span class="sxs-lookup"><span data-stu-id="2a095-134">Changes to a group's conversations:</span></span><br>`groups/{id}/conversations` | <span data-ttu-id="2a095-135">否</span><span class="sxs-lookup"><span data-stu-id="2a095-135">No</span></span> |
| <span data-ttu-id="2a095-136">Outlook [事件][]</span><span class="sxs-lookup"><span data-stu-id="2a095-136">Outlook [event][]</span></span> | <span data-ttu-id="2a095-137">对用户邮箱中的所有事件更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-137">Changes to all events in a user's mailbox:</span></span><br>`/users/{id}/events` | <span data-ttu-id="2a095-138">否</span><span class="sxs-lookup"><span data-stu-id="2a095-138">No</span></span> |
| <span data-ttu-id="2a095-139">Outlook [邮件][]</span><span class="sxs-lookup"><span data-stu-id="2a095-139">Outlook [message][]</span></span> | <span data-ttu-id="2a095-140">对用户邮箱中的所有邮件更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-140">Changes to all messages in a user's mailbox:</span></span> <br>`/users/{id}/messages`<br><span data-ttu-id="2a095-141">对用户收件箱中的所有邮件更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-141">Changes to messages in a user's Inbox:</span></span><br>`/users/{id}/mailFolders('inbox')/messages` | <span data-ttu-id="2a095-142">否</span><span class="sxs-lookup"><span data-stu-id="2a095-142">No</span></span> |
| <span data-ttu-id="2a095-143">Outlook 个人[联系人][]</span><span class="sxs-lookup"><span data-stu-id="2a095-143">Outlook personal [contact][]</span></span> | <span data-ttu-id="2a095-144">对用户邮箱中的所有个人联系人更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-144">Changes to all personal contacts in a user's mailbox:</span></span><br>`/users/{id}/contacts` | <span data-ttu-id="2a095-145">否</span><span class="sxs-lookup"><span data-stu-id="2a095-145">No</span></span> |
| <span data-ttu-id="2a095-146">安全[警报][]</span><span class="sxs-lookup"><span data-stu-id="2a095-146">Security [alert][]</span></span> | <span data-ttu-id="2a095-147">对特定警报更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-147">Changes to a specific alert:</span></span><br>`/security/alerts/{id}` <br><span data-ttu-id="2a095-148">对已筛选的警报更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-148">Changes to filtered alerts:</span></span><br> `/security/alerts/?$filter`| <span data-ttu-id="2a095-149">否</span><span class="sxs-lookup"><span data-stu-id="2a095-149">No</span></span> |
| <span data-ttu-id="2a095-150">Teams [callRecord][]</span><span class="sxs-lookup"><span data-stu-id="2a095-150">Teams [callRecord][]</span></span> | <span data-ttu-id="2a095-151">更改 _所有_ 呼叫记录： `/communications/callRecords`</span><span class="sxs-lookup"><span data-stu-id="2a095-151">Changes to _all_ call records: `/communications/callRecords`</span></span> | <span data-ttu-id="2a095-152">否</span><span class="sxs-lookup"><span data-stu-id="2a095-152">No</span></span> |
| <span data-ttu-id="2a095-153">Teams [频道][]</span><span class="sxs-lookup"><span data-stu-id="2a095-153">Teams [channel][]</span></span> | <span data-ttu-id="2a095-154">更改所有团队中的频道：</span><span class="sxs-lookup"><span data-stu-id="2a095-154">Changes to channels in all teams:</span></span><br>`/teams/getAllChannels` <br><span data-ttu-id="2a095-155">对特定团队中的频道的更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-155">Changes to channel in a specific team:</span></span><br>`/teams/{id}/channels` | <span data-ttu-id="2a095-156">是</span><span class="sxs-lookup"><span data-stu-id="2a095-156">Yes</span></span> |
| <span data-ttu-id="2a095-157">Teams [chatmessage][]</span><span class="sxs-lookup"><span data-stu-id="2a095-157">Teams [chatmessage][]</span></span> | <span data-ttu-id="2a095-158">对所有团队中所有频道聊天消息更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-158">Changes to chat messages in all channels in all teams:</span></span><br>`/teams/getAllMessages` <br><span data-ttu-id="2a095-159">对特定频道中的聊天消息更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-159">Changes to chat messages in a specific channel:</span></span><br>`/teams/{id}/channels/{id}/messages`<br><span data-ttu-id="2a095-160">对所有聊天的消息更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-160">Changes to chat messages in all chats:</span></span><br>`/chats/getAllMessages` <br><span data-ttu-id="2a095-161">对特定聊天中的消息更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-161">Changes to chat messages in a specific chat:</span></span><br>`/chats/{id}/messages` | <span data-ttu-id="2a095-162">是</span><span class="sxs-lookup"><span data-stu-id="2a095-162">Yes</span></span> |
| <span data-ttu-id="2a095-163">Teams [conversationMember][]</span><span class="sxs-lookup"><span data-stu-id="2a095-163">Teams [conversationMember][]</span></span> | <span data-ttu-id="2a095-164">对特定团队中的成员身份的更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-164">Changes to membership in a specific team:</span></span><br>`/teams/{id}/members` | <span data-ttu-id="2a095-165">是</span><span class="sxs-lookup"><span data-stu-id="2a095-165">Yes</span></span> |
| <span data-ttu-id="2a095-166">Teams[状态][]</span><span class="sxs-lookup"><span data-stu-id="2a095-166">Teams [presence][]</span></span> | <span data-ttu-id="2a095-167">对单个用户状态所做的更改： `/communications/presences/{id}`</span><span class="sxs-lookup"><span data-stu-id="2a095-167">Changes to a single user's presence: `/communications/presences/{id}`</span></span> <br> <span data-ttu-id="2a095-168">对多个用户状态所做的更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-168">Changes to multiple user presences:</span></span><br> `/communications/presences?$filter=id in ({id},{id}...)` | <span data-ttu-id="2a095-169">是</span><span class="sxs-lookup"><span data-stu-id="2a095-169">Yes</span></span> |
| <span data-ttu-id="2a095-170">Teams [团队][]</span><span class="sxs-lookup"><span data-stu-id="2a095-170">Teams [team][]</span></span> | <span data-ttu-id="2a095-171">对租户中任何团队的更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-171">Changes to any team in the tenant:</span></span><br>`/teams` <br><span data-ttu-id="2a095-172">对特定团队的更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-172">Changes to a specific team:</span></span><br>`/teams/{id}` | <span data-ttu-id="2a095-173">是</span><span class="sxs-lookup"><span data-stu-id="2a095-173">Yes</span></span> |
| <span data-ttu-id="2a095-174">[todoTask][]</span><span class="sxs-lookup"><span data-stu-id="2a095-174">[todoTask][]</span></span> | <span data-ttu-id="2a095-175">对特定任务列表中所有任务的更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-175">Changes to all task in a specific task list:</span></span><br>`/me/todo/lists/{todoTaskListId}/tasks` | <span data-ttu-id="2a095-176">否</span><span class="sxs-lookup"><span data-stu-id="2a095-176">No</span></span> |
| <span data-ttu-id="2a095-177">[用户][]</span><span class="sxs-lookup"><span data-stu-id="2a095-177">[user][]</span></span> | <span data-ttu-id="2a095-178">对所有用户更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-178">Changes to all users:</span></span><br>`/users` <br><span data-ttu-id="2a095-179">对特定用户更改：</span><span class="sxs-lookup"><span data-stu-id="2a095-179">Changes to a specific user:</span></span><br>`/users/{id}`| <span data-ttu-id="2a095-180">否</span><span class="sxs-lookup"><span data-stu-id="2a095-180">No</span></span> |


> <span data-ttu-id="2a095-181">**注意**：以 `/users/{id}` 开头的任何资源路径还可接受 `/me` 以引用已登录的用户。</span><span class="sxs-lookup"><span data-stu-id="2a095-181">**Note**: Any resource path that begins with `/users/{id}` can also accept `/me` to reference the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a095-182">权限</span><span class="sxs-lookup"><span data-stu-id="2a095-182">Permissions</span></span>

<span data-ttu-id="2a095-183">通常订阅操作需要拥有对资源的读取权限。</span><span class="sxs-lookup"><span data-stu-id="2a095-183">In general, subscription operations require read permission to the resource.</span></span> <span data-ttu-id="2a095-184">例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。</span><span class="sxs-lookup"><span data-stu-id="2a095-184">For example, to get notifications for messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="2a095-185">[创建订阅](../api/subscription-post-subscriptions.md)一文列出了各个资源类型所需的权限。</span><span class="sxs-lookup"><span data-stu-id="2a095-185">The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type.</span></span> <span data-ttu-id="2a095-186">下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。</span><span class="sxs-lookup"><span data-stu-id="2a095-186">The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="2a095-187">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a095-187">Permission type</span></span>                        | <span data-ttu-id="2a095-188">支持的资源类型</span><span class="sxs-lookup"><span data-stu-id="2a095-188">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="2a095-189">委派 - 工作或学校帐户</span><span class="sxs-lookup"><span data-stu-id="2a095-189">Delegated - work or school account</span></span>     | <span data-ttu-id="2a095-190">[alert][]、 [channel][]、 [contact][]、 [conversation][]、 [conversationMember][]、 [driveItem][]、 [list][]、 [event][]、 [group][]、 [message][]、 [user][]、 [presence][]、 [chatMessage][] (preview) ， [team][]， [todoTask][]</span><span class="sxs-lookup"><span data-stu-id="2a095-190">[alert][], [channel][], [contact][], [conversation][], [conversationMember][], [driveItem][], [list][], [event][], [group][], [message][], [user][], [presence][], [chatMessage][] (preview), [team][], [todoTask][]</span></span> |
| <span data-ttu-id="2a095-191">委派 - 个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="2a095-191">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="2a095-192">[contact][]、 [driveItem][]、 [list][]、 [event][]、 [message][]、[todoTask][]</span><span class="sxs-lookup"><span data-stu-id="2a095-192">[contact][], [driveItem][], [list][], [event][], [message][],[todoTask][]</span></span>                                     |
| <span data-ttu-id="2a095-193">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a095-193">Application</span></span>                            | <span data-ttu-id="2a095-194">[alert][]、 [channel][]、 [contact][]、 [driveItem][]、 [list][]、 [event][]、 [group][]、 [message][]、 [user][]、 [callRecord][]、 [chatMessage][]、 [conversationMember][]、 [printer][]、 [printTaskDefinition][]、 [team][]</span><span class="sxs-lookup"><span data-stu-id="2a095-194">[alert][], [channel][], [contact][], [driveItem][], [list][], [event][], [group][], [message][], [user][], [callRecord][], [chatMessage][], [conversationMember][], [printer][], [printTaskDefinition][], [team][]</span></span> |

## <a name="see-also"></a><span data-ttu-id="2a095-195">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2a095-195">See also</span></span>

- [<span data-ttu-id="2a095-196">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="2a095-196">Subscription resource type</span></span>](subscription.md)
- [<span data-ttu-id="2a095-197">列出订阅</span><span class="sxs-lookup"><span data-stu-id="2a095-197">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="2a095-198">获取订阅</span><span class="sxs-lookup"><span data-stu-id="2a095-198">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="2a095-199">创建订阅</span><span class="sxs-lookup"><span data-stu-id="2a095-199">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="2a095-200">更新订阅</span><span class="sxs-lookup"><span data-stu-id="2a095-200">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="2a095-201">删除订阅</span><span class="sxs-lookup"><span data-stu-id="2a095-201">Delete subscription</span></span>](../api/subscription-delete.md)

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

