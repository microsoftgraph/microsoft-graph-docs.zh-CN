---
title: 使用 Microsoft Graph API 获取更改通知
description: Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。 客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。 客户端应用使用通知在更改时更新其状态。 有关详细信息（包括如何订阅和处理传入通知），请参阅“设置用户数据更改的通知”。
localization_priority: Normal
author: davidmu1
doc_type: conceptualPageType
ms.prod: ''
ms.openlocfilehash: 27a67797830513a951c778e994bc8033ddab5bea
ms.sourcegitcommit: 74a1fb3874e04c488e1b87dcee80d76cc586c1f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51030993"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="dc070-106">使用 Microsoft Graph API 获取更改通知</span><span class="sxs-lookup"><span data-stu-id="dc070-106">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="dc070-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc070-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc070-108">Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。</span><span class="sxs-lookup"><span data-stu-id="dc070-108">The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="dc070-109">客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。</span><span class="sxs-lookup"><span data-stu-id="dc070-109">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="dc070-110">客户端应用使用通知在更改时更新其状态。</span><span class="sxs-lookup"><span data-stu-id="dc070-110">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="dc070-111">有关详细信息（包括如何订阅和处理传入通知），请参阅[设置用户数据更改的通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="dc070-111">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="dc070-112">使用 Microsoft Graph API，应用可以订阅以下资源的更改：</span><span class="sxs-lookup"><span data-stu-id="dc070-112">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

| <span data-ttu-id="dc070-113">**资源**</span><span class="sxs-lookup"><span data-stu-id="dc070-113">**Resource**</span></span> | <span data-ttu-id="dc070-114">**支持的资源路径**</span><span class="sxs-lookup"><span data-stu-id="dc070-114">**Supported resource paths**</span></span> | <span data-ttu-id="dc070-115">**可包含在通知中的资源数据**</span><span class="sxs-lookup"><span data-stu-id="dc070-115">**Resource data can be included in notifications**</span></span>                  |
|:----------------|:------------|:-----------------------------------------|
| <span data-ttu-id="dc070-116">云打印 [打印机][]</span><span class="sxs-lookup"><span data-stu-id="dc070-116">Cloud printing [printer][]</span></span> | <span data-ttu-id="dc070-117">打印作业准备好下载作业时更改 (JobFetchable 事件) ：</span><span class="sxs-lookup"><span data-stu-id="dc070-117">Changes when a print job is ready to be downloaded (JobFetchable event):</span></span><br>`/print/printers/{id}/jobs` | <span data-ttu-id="dc070-118">否</span><span class="sxs-lookup"><span data-stu-id="dc070-118">No</span></span> |
| <span data-ttu-id="dc070-119">云打印 [printTaskDefinition][]</span><span class="sxs-lookup"><span data-stu-id="dc070-119">Cloud printing [printTaskDefinition][]</span></span> | <span data-ttu-id="dc070-120">当队列中存在有效作业时 (JobStarted 事件) ：</span><span class="sxs-lookup"><span data-stu-id="dc070-120">Changes when there is a valid job in the queue (JobStarted event) :</span></span><br>`/print/printtaskdefinition/{id}/tasks` | <span data-ttu-id="dc070-121">否</span><span class="sxs-lookup"><span data-stu-id="dc070-121">No</span></span> |
| <span data-ttu-id="dc070-122">OneDrive for Business 上的 [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="dc070-122">[driveItem][] on OneDrive for Business</span></span> | <span data-ttu-id="dc070-123">对 _根文件夹_ 的层次结构内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="dc070-123">Changes to content within the hierarchy of the _root folder_:</span></span><br>`/drives/{id}/root`<br> `/users/{id}/drive/root` | <span data-ttu-id="dc070-124">否</span><span class="sxs-lookup"><span data-stu-id="dc070-124">No</span></span> |
| <span data-ttu-id="dc070-125">OneDrive（个人版）上的 [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="dc070-125">[driveItem][] on OneDrive (personal)</span></span> | <span data-ttu-id="dc070-126">对 _任何文件夹_ 的层次结构内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="dc070-126">Changes to content within the hierarchy of _any folder_:</span></span><br>`/users/{id}/drive/root` | <span data-ttu-id="dc070-127">否</span><span class="sxs-lookup"><span data-stu-id="dc070-127">No</span></span> |
| <span data-ttu-id="dc070-128">[组][]</span><span class="sxs-lookup"><span data-stu-id="dc070-128">[group][]</span></span> | <span data-ttu-id="dc070-129">对所有组更改：</span><span class="sxs-lookup"><span data-stu-id="dc070-129">Changes to all groups:</span></span><br>`/groups` <br><span data-ttu-id="dc070-130">对特定组更改：</span><span class="sxs-lookup"><span data-stu-id="dc070-130">Changes to a specific group:</span></span><br>`/groups/{id}`<br><span data-ttu-id="dc070-131">对特定组的所有者所做的更改：</span><span class="sxs-lookup"><span data-stu-id="dc070-131">Changes to owners of a specific group:</span></span><br>`/groups/{id}/owners`<br><span data-ttu-id="dc070-132">对特定组成员所做的更改：</span><span class="sxs-lookup"><span data-stu-id="dc070-132">Changes to members of a specific group:</span></span><br>`/groups/{id}/members` | <span data-ttu-id="dc070-133">否</span><span class="sxs-lookup"><span data-stu-id="dc070-133">No</span></span> |
| <span data-ttu-id="dc070-134">SharePoint [网站][]下的[列表][]</span><span class="sxs-lookup"><span data-stu-id="dc070-134">[list][] under a SharePoint [site][]</span></span> | `/sites/{id}/lists/{id}` | <span data-ttu-id="dc070-135">否</span><span class="sxs-lookup"><span data-stu-id="dc070-135">No</span></span> |
| <span data-ttu-id="dc070-136">Microsoft 365 组[对话][]</span><span class="sxs-lookup"><span data-stu-id="dc070-136">Microsoft 365 group [conversation][]</span></span> | <span data-ttu-id="dc070-137">查看组的对话：</span><span class="sxs-lookup"><span data-stu-id="dc070-137">Changes to a group's conversations:</span></span><br>`groups/{id}/conversations` | <span data-ttu-id="dc070-138">否</span><span class="sxs-lookup"><span data-stu-id="dc070-138">No</span></span> |
| <span data-ttu-id="dc070-139">Outlook [事件][]</span><span class="sxs-lookup"><span data-stu-id="dc070-139">Outlook [event][]</span></span> | <span data-ttu-id="dc070-140">对用户邮箱中的所有事件更改：</span><span class="sxs-lookup"><span data-stu-id="dc070-140">Changes to all events in a user's mailbox:</span></span><br>`/users/{id}/events` | <span data-ttu-id="dc070-141">否</span><span class="sxs-lookup"><span data-stu-id="dc070-141">No</span></span> |
| <span data-ttu-id="dc070-142">Outlook [邮件][]</span><span class="sxs-lookup"><span data-stu-id="dc070-142">Outlook [message][]</span></span> | <span data-ttu-id="dc070-143">对用户邮箱中的所有邮件更改：</span><span class="sxs-lookup"><span data-stu-id="dc070-143">Changes to all messages in a user's mailbox:</span></span> <br>`/users/{id}/messages`<br><span data-ttu-id="dc070-144">对用户收件箱中的所有邮件更改：</span><span class="sxs-lookup"><span data-stu-id="dc070-144">Changes to messages in a user's Inbox:</span></span><br>`/users/{id}/mailFolders('inbox')/messages` | <span data-ttu-id="dc070-145">否</span><span class="sxs-lookup"><span data-stu-id="dc070-145">No</span></span> |
| <span data-ttu-id="dc070-146">Outlook 个人[联系人][]</span><span class="sxs-lookup"><span data-stu-id="dc070-146">Outlook personal [contact][]</span></span> | <span data-ttu-id="dc070-147">对用户邮箱中的所有个人联系人更改：</span><span class="sxs-lookup"><span data-stu-id="dc070-147">Changes to all personal contacts in a user's mailbox:</span></span><br>`/users/{id}/contacts` | <span data-ttu-id="dc070-148">否</span><span class="sxs-lookup"><span data-stu-id="dc070-148">No</span></span> |
| <span data-ttu-id="dc070-149">安全[警报][]</span><span class="sxs-lookup"><span data-stu-id="dc070-149">Security [alert][]</span></span> | <span data-ttu-id="dc070-150">对特定警报更改：</span><span class="sxs-lookup"><span data-stu-id="dc070-150">Changes to a specific alert:</span></span><br>`/security/alerts/{id}` <br><span data-ttu-id="dc070-151">对已筛选的警报更改：</span><span class="sxs-lookup"><span data-stu-id="dc070-151">Changes to filtered alerts:</span></span><br> `/security/alerts/?$filter`| <span data-ttu-id="dc070-152">否</span><span class="sxs-lookup"><span data-stu-id="dc070-152">No</span></span> |
| <span data-ttu-id="dc070-153">Teams [callRecord][]</span><span class="sxs-lookup"><span data-stu-id="dc070-153">Teams [callRecord][]</span></span> | <span data-ttu-id="dc070-154">更改 _所有_ 呼叫记录： `/communications/callRecords`</span><span class="sxs-lookup"><span data-stu-id="dc070-154">Changes to _all_ call records: `/communications/callRecords`</span></span> | <span data-ttu-id="dc070-155">否</span><span class="sxs-lookup"><span data-stu-id="dc070-155">No</span></span> |
| <span data-ttu-id="dc070-156">Teams [chatmessage][]</span><span class="sxs-lookup"><span data-stu-id="dc070-156">Teams [chatmessage][]</span></span> | <span data-ttu-id="dc070-157">对所有团队中所有频道聊天消息更改：</span><span class="sxs-lookup"><span data-stu-id="dc070-157">Changes to chat messages in all channels in all teams:</span></span><br>`/teams/getAllMessages` <br><span data-ttu-id="dc070-158">对特定频道中的聊天消息更改：</span><span class="sxs-lookup"><span data-stu-id="dc070-158">Changes to chat messages in a specific channel:</span></span><br>`/teams/{id}/channels/{id}/messages`<br><span data-ttu-id="dc070-159">对所有聊天的消息更改：</span><span class="sxs-lookup"><span data-stu-id="dc070-159">Changes to chat messages in all chats:</span></span><br>`/chats/getAllMessages` <br><span data-ttu-id="dc070-160">对特定聊天中的消息更改：</span><span class="sxs-lookup"><span data-stu-id="dc070-160">Changes to chat messages in a specific chat:</span></span><br>`/chats/{id}/messages` | <span data-ttu-id="dc070-161">是</span><span class="sxs-lookup"><span data-stu-id="dc070-161">Yes</span></span> |
| <span data-ttu-id="dc070-162">Teams [状态][]</span><span class="sxs-lookup"><span data-stu-id="dc070-162">Teams [presence][]</span></span> | <span data-ttu-id="dc070-163">对单个用户状态所做的更改： `/communications/presences/{id}`</span><span class="sxs-lookup"><span data-stu-id="dc070-163">Changes to a single user's presence: `/communications/presences/{id}`</span></span> <br> <span data-ttu-id="dc070-164">对多个用户状态所做的更改：</span><span class="sxs-lookup"><span data-stu-id="dc070-164">Changes to multiple user presences:</span></span><br> `/communications/presences?$filter=id in ({id},{id}...)` | <span data-ttu-id="dc070-165">是</span><span class="sxs-lookup"><span data-stu-id="dc070-165">Yes</span></span> |
| <span data-ttu-id="dc070-166">[todoTask][]</span><span class="sxs-lookup"><span data-stu-id="dc070-166">[todoTask][]</span></span> | <span data-ttu-id="dc070-167">对特定任务列表中所有任务的更改：</span><span class="sxs-lookup"><span data-stu-id="dc070-167">Changes to all task in a specific task list:</span></span><br>`/me/todo/lists/{todoTaskListId}/tasks` | <span data-ttu-id="dc070-168">否</span><span class="sxs-lookup"><span data-stu-id="dc070-168">No</span></span> |
| <span data-ttu-id="dc070-169">[用户][]</span><span class="sxs-lookup"><span data-stu-id="dc070-169">[user][]</span></span> | <span data-ttu-id="dc070-170">对所有用户更改：</span><span class="sxs-lookup"><span data-stu-id="dc070-170">Changes to all users:</span></span><br>`/users` <br><span data-ttu-id="dc070-171">对特定用户更改：</span><span class="sxs-lookup"><span data-stu-id="dc070-171">Changes to a specific user:</span></span><br>`/users/{id}`| <span data-ttu-id="dc070-172">否</span><span class="sxs-lookup"><span data-stu-id="dc070-172">No</span></span> |


> <span data-ttu-id="dc070-173">**注意**：以 `/users/{id}` 开头的任何资源路径还可接受 `/me` 以引用已登录的用户。</span><span class="sxs-lookup"><span data-stu-id="dc070-173">**Note**: Any resource path that begins with `/users/{id}` can also accept `/me` to reference the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc070-174">权限</span><span class="sxs-lookup"><span data-stu-id="dc070-174">Permissions</span></span>

<span data-ttu-id="dc070-175">通常订阅操作需要拥有对资源的读取权限。</span><span class="sxs-lookup"><span data-stu-id="dc070-175">In general, subscription operations require read permission to the resource.</span></span> <span data-ttu-id="dc070-176">例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。</span><span class="sxs-lookup"><span data-stu-id="dc070-176">For example, to get notifications for messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="dc070-177">[创建订阅](../api/subscription-post-subscriptions.md)一文列出了各个资源类型所需的权限。</span><span class="sxs-lookup"><span data-stu-id="dc070-177">The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type.</span></span> <span data-ttu-id="dc070-178">下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。</span><span class="sxs-lookup"><span data-stu-id="dc070-178">The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="dc070-179">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc070-179">Permission type</span></span>                        | <span data-ttu-id="dc070-180">支持的资源类型</span><span class="sxs-lookup"><span data-stu-id="dc070-180">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="dc070-181">委派 - 工作或学校帐户</span><span class="sxs-lookup"><span data-stu-id="dc070-181">Delegated - work or school account</span></span>     | <span data-ttu-id="dc070-182">[alert][]、 [contact][]、 [conversation][]、 [driveItem][]、 [list][]、 [event][]、 [group][]、 [message][]、 [user][]、 [presence][]、 [chatMessage][] (preview) ， [todoTask][]</span><span class="sxs-lookup"><span data-stu-id="dc070-182">[alert][], [contact][], [conversation][], [driveItem][], [list][], [event][], [group][], [message][], [user][], [presence][], [chatMessage][] (preview), [todoTask][]</span></span> |
| <span data-ttu-id="dc070-183">委派 - 个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="dc070-183">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="dc070-184">[contact][]、 [driveItem][]、 [list][]、 [event][]、 [message][]、[todoTask][]</span><span class="sxs-lookup"><span data-stu-id="dc070-184">[contact][], [driveItem][], [list][], [event][], [message][],[todoTask][]</span></span>                                     |
| <span data-ttu-id="dc070-185">应用程序</span><span class="sxs-lookup"><span data-stu-id="dc070-185">Application</span></span>                            | <span data-ttu-id="dc070-186">[alert][]、 [contact][]、 [driveItem][]、 [list][]、 [event][]、 [group][]、 [message][]、 [user][]、 [callRecord][]、 [chatMessage][]、 [printer][]、 [printTaskDefinition][]</span><span class="sxs-lookup"><span data-stu-id="dc070-186">[alert][], [contact][], [driveItem][], [list][], [event][], [group][], [message][], [user][], [callRecord][], [chatMessage][], [printer][], [printTaskDefinition][]</span></span>|

## <a name="see-also"></a><span data-ttu-id="dc070-187">另请参阅</span><span class="sxs-lookup"><span data-stu-id="dc070-187">See also</span></span>

- [<span data-ttu-id="dc070-188">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="dc070-188">Subscription resource type</span></span>](subscription.md)
- [<span data-ttu-id="dc070-189">列出订阅</span><span class="sxs-lookup"><span data-stu-id="dc070-189">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="dc070-190">获取订阅</span><span class="sxs-lookup"><span data-stu-id="dc070-190">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="dc070-191">创建订阅</span><span class="sxs-lookup"><span data-stu-id="dc070-191">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="dc070-192">更新订阅</span><span class="sxs-lookup"><span data-stu-id="dc070-192">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="dc070-193">删除订阅</span><span class="sxs-lookup"><span data-stu-id="dc070-193">Delete subscription</span></span>](../api/subscription-delete.md)

[chatMessage]: ./chatmessage.md
[contact]: ./contact.md
[对话]: ./conversation.md
[conversation]: ./conversation.md
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
[todoTask]: ./todoTask.md

