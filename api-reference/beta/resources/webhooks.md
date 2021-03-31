---
title: 使用 Microsoft Graph API 获取更改通知
description: 向客户端传递更改通知。
localization_priority: Normal
author: Jumaodhiss
doc_type: conceptualPageType
ms.prod: change-notifications
ms.openlocfilehash: 941189d27c01222309a8011fe7701d811ac46a7c
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468682"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="e051c-103">使用 Microsoft Graph API 获取更改通知</span><span class="sxs-lookup"><span data-stu-id="e051c-103">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="e051c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e051c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e051c-105">Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。</span><span class="sxs-lookup"><span data-stu-id="e051c-105">The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="e051c-106">客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。</span><span class="sxs-lookup"><span data-stu-id="e051c-106">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="e051c-107">客户端应用使用通知在更改时更新其状态。</span><span class="sxs-lookup"><span data-stu-id="e051c-107">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="e051c-108">有关详细信息（包括如何订阅和处理传入通知），请参阅[设置用户数据更改的通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="e051c-108">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="e051c-109">使用 Microsoft Graph API，应用可以订阅以下资源的更改：</span><span class="sxs-lookup"><span data-stu-id="e051c-109">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

| <span data-ttu-id="e051c-110">**资源**</span><span class="sxs-lookup"><span data-stu-id="e051c-110">**Resource**</span></span> | <span data-ttu-id="e051c-111">**支持的资源路径**</span><span class="sxs-lookup"><span data-stu-id="e051c-111">**Supported resource paths**</span></span> | <span data-ttu-id="e051c-112">**可包含在通知中的资源数据**</span><span class="sxs-lookup"><span data-stu-id="e051c-112">**Resource data can be included in notifications**</span></span>                  |
|:----------------|:------------|:-----------------------------------------|
| <span data-ttu-id="e051c-113">云打印 [打印机][]</span><span class="sxs-lookup"><span data-stu-id="e051c-113">Cloud printing [printer][]</span></span> | <span data-ttu-id="e051c-114">打印作业准备好下载时的变化（作业可打印事件）：</span><span class="sxs-lookup"><span data-stu-id="e051c-114">Changes when a print job is ready to be downloaded (JobFetchable event):</span></span><br>`/print/printers/{id}/jobs` | <span data-ttu-id="e051c-115">不支持</span><span class="sxs-lookup"><span data-stu-id="e051c-115">No</span></span> |
| <span data-ttu-id="e051c-116">云打印 [printTaskDefinition][]</span><span class="sxs-lookup"><span data-stu-id="e051c-116">Cloud printing [printTaskDefinition][]</span></span> | <span data-ttu-id="e051c-117">在队列中具有有效作业时的变化（作业启动事件）：</span><span class="sxs-lookup"><span data-stu-id="e051c-117">Changes when there is a valid job in the queue (JobStarted event) :</span></span><br>`/print/printtaskdefinition/{id}/tasks` | <span data-ttu-id="e051c-118">否</span><span class="sxs-lookup"><span data-stu-id="e051c-118">No</span></span> |
| <span data-ttu-id="e051c-119">OneDrive for Business 上的 [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="e051c-119">[driveItem][] on OneDrive for Business</span></span> | <span data-ttu-id="e051c-120">对 _根文件夹_ 的层次结构内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="e051c-120">Changes to content within the hierarchy of the _root folder_:</span></span><br>`/drives/{id}/root`<br> `/users/{id}/drive/root` | <span data-ttu-id="e051c-121">否</span><span class="sxs-lookup"><span data-stu-id="e051c-121">No</span></span> |
| <span data-ttu-id="e051c-122">OneDrive（个人版）上的 [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="e051c-122">[driveItem][] on OneDrive (personal)</span></span> | <span data-ttu-id="e051c-123">对 _任何文件夹_ 的层次结构内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="e051c-123">Changes to content within the hierarchy of _any folder_:</span></span><br>`/users/{id}/drive/root` | <span data-ttu-id="e051c-124">否</span><span class="sxs-lookup"><span data-stu-id="e051c-124">No</span></span> |
| <span data-ttu-id="e051c-125">[组][]</span><span class="sxs-lookup"><span data-stu-id="e051c-125">[group][]</span></span> | <span data-ttu-id="e051c-126">对所有组更改：</span><span class="sxs-lookup"><span data-stu-id="e051c-126">Changes to all groups:</span></span><br>`/groups` <br><span data-ttu-id="e051c-127">对特定组更改：</span><span class="sxs-lookup"><span data-stu-id="e051c-127">Changes to a specific group:</span></span><br>`/groups/{id}`<br><span data-ttu-id="e051c-128">对特定组的所有者所做的更改：</span><span class="sxs-lookup"><span data-stu-id="e051c-128">Changes to owners of a specific group:</span></span><br>`/groups/{id}/owners`<br><span data-ttu-id="e051c-129">对特定组成员所做的更改：</span><span class="sxs-lookup"><span data-stu-id="e051c-129">Changes to members of a specific group:</span></span><br>`/groups/{id}/members` | <span data-ttu-id="e051c-130">否</span><span class="sxs-lookup"><span data-stu-id="e051c-130">No</span></span> |
| <span data-ttu-id="e051c-131">SharePoint [网站][]下的[列表][]</span><span class="sxs-lookup"><span data-stu-id="e051c-131">[list][] under a SharePoint [site][]</span></span> | `/sites/{id}/lists/{id}` | <span data-ttu-id="e051c-132">否</span><span class="sxs-lookup"><span data-stu-id="e051c-132">No</span></span> |
| <span data-ttu-id="e051c-133">Microsoft 365 组[对话][]</span><span class="sxs-lookup"><span data-stu-id="e051c-133">Microsoft 365 group [conversation][]</span></span> | <span data-ttu-id="e051c-134">查看组的对话：</span><span class="sxs-lookup"><span data-stu-id="e051c-134">Changes to a group's conversations:</span></span><br>`groups/{id}/conversations` | <span data-ttu-id="e051c-135">否</span><span class="sxs-lookup"><span data-stu-id="e051c-135">No</span></span> |
| <span data-ttu-id="e051c-136">Outlook [事件][]</span><span class="sxs-lookup"><span data-stu-id="e051c-136">Outlook [event][]</span></span> | <span data-ttu-id="e051c-137">对用户邮箱中的所有事件更改：</span><span class="sxs-lookup"><span data-stu-id="e051c-137">Changes to all events in a user's mailbox:</span></span><br>`/users/{id}/events` | <span data-ttu-id="e051c-138">否</span><span class="sxs-lookup"><span data-stu-id="e051c-138">No</span></span> |
| <span data-ttu-id="e051c-139">Outlook [邮件][]</span><span class="sxs-lookup"><span data-stu-id="e051c-139">Outlook [message][]</span></span> | <span data-ttu-id="e051c-140">对用户邮箱中的所有邮件更改：</span><span class="sxs-lookup"><span data-stu-id="e051c-140">Changes to all messages in a user's mailbox:</span></span> <br>`/users/{id}/messages`<br><span data-ttu-id="e051c-141">对用户收件箱中的所有邮件更改：</span><span class="sxs-lookup"><span data-stu-id="e051c-141">Changes to messages in a user's Inbox:</span></span><br>`/users/{id}/mailFolders('inbox')/messages` | <span data-ttu-id="e051c-142">否</span><span class="sxs-lookup"><span data-stu-id="e051c-142">No</span></span> |
| <span data-ttu-id="e051c-143">Outlook 个人[联系人][]</span><span class="sxs-lookup"><span data-stu-id="e051c-143">Outlook personal [contact][]</span></span> | <span data-ttu-id="e051c-144">对用户邮箱中的所有个人联系人更改：</span><span class="sxs-lookup"><span data-stu-id="e051c-144">Changes to all personal contacts in a user's mailbox:</span></span><br>`/users/{id}/contacts` | <span data-ttu-id="e051c-145">否</span><span class="sxs-lookup"><span data-stu-id="e051c-145">No</span></span> |
| <span data-ttu-id="e051c-146">安全[警报][]</span><span class="sxs-lookup"><span data-stu-id="e051c-146">Security [alert][]</span></span> | <span data-ttu-id="e051c-147">对特定警报更改：</span><span class="sxs-lookup"><span data-stu-id="e051c-147">Changes to a specific alert:</span></span><br>`/security/alerts/{id}` <br><span data-ttu-id="e051c-148">对已筛选的警报更改：</span><span class="sxs-lookup"><span data-stu-id="e051c-148">Changes to filtered alerts:</span></span><br> `/security/alerts/?$filter`| <span data-ttu-id="e051c-149">否</span><span class="sxs-lookup"><span data-stu-id="e051c-149">No</span></span> |
| <span data-ttu-id="e051c-150">Teams [callRecord][]</span><span class="sxs-lookup"><span data-stu-id="e051c-150">Teams [callRecord][]</span></span> | <span data-ttu-id="e051c-151">更改 _所有_ 呼叫记录： `/communications/callRecords`</span><span class="sxs-lookup"><span data-stu-id="e051c-151">Changes to _all_ call records: `/communications/callRecords`</span></span> | <span data-ttu-id="e051c-152">否</span><span class="sxs-lookup"><span data-stu-id="e051c-152">No</span></span> |
| <span data-ttu-id="e051c-153">Teams [chatmessage][]</span><span class="sxs-lookup"><span data-stu-id="e051c-153">Teams [chatmessage][]</span></span> | <span data-ttu-id="e051c-154">对所有团队中所有频道聊天消息更改：</span><span class="sxs-lookup"><span data-stu-id="e051c-154">Changes to chat messages in all channels in all teams:</span></span><br>`/teams/getAllMessages` <br><span data-ttu-id="e051c-155">对特定频道中的聊天消息更改：</span><span class="sxs-lookup"><span data-stu-id="e051c-155">Changes to chat messages in a specific channel:</span></span><br>`/teams/{id}/channels/{id}/messages`<br><span data-ttu-id="e051c-156">对所有聊天的消息更改：</span><span class="sxs-lookup"><span data-stu-id="e051c-156">Changes to chat messages in all chats:</span></span><br>`/chats/getAllMessages` <br><span data-ttu-id="e051c-157">对特定聊天中的消息更改：</span><span class="sxs-lookup"><span data-stu-id="e051c-157">Changes to chat messages in a specific chat:</span></span><br>`/chats/{id}/messages` | <span data-ttu-id="e051c-158">是</span><span class="sxs-lookup"><span data-stu-id="e051c-158">Yes</span></span> |
| <span data-ttu-id="e051c-159">Teams [状态][]</span><span class="sxs-lookup"><span data-stu-id="e051c-159">Teams [presence][]</span></span> | <span data-ttu-id="e051c-160">对单个用户状态所做的更改： `/communications/presences/{id}`</span><span class="sxs-lookup"><span data-stu-id="e051c-160">Changes to a single user's presence: `/communications/presences/{id}`</span></span> <br> <span data-ttu-id="e051c-161">对多个用户状态所做的更改：</span><span class="sxs-lookup"><span data-stu-id="e051c-161">Changes to multiple user presences:</span></span><br> `/communications/presences?$filter=id in ({id},{id}...)` | <span data-ttu-id="e051c-162">是</span><span class="sxs-lookup"><span data-stu-id="e051c-162">Yes</span></span> |
| <span data-ttu-id="e051c-163">[todoTask][]</span><span class="sxs-lookup"><span data-stu-id="e051c-163">[todoTask][]</span></span> | <span data-ttu-id="e051c-164">对特定任务列表中所有任务的更改：</span><span class="sxs-lookup"><span data-stu-id="e051c-164">Changes to all task in a specific task list:</span></span><br>`/me/todo/lists/{todoTaskListId}/tasks` | <span data-ttu-id="e051c-165">否</span><span class="sxs-lookup"><span data-stu-id="e051c-165">No</span></span> |
| <span data-ttu-id="e051c-166">[用户][]</span><span class="sxs-lookup"><span data-stu-id="e051c-166">[user][]</span></span> | <span data-ttu-id="e051c-167">对所有用户更改：</span><span class="sxs-lookup"><span data-stu-id="e051c-167">Changes to all users:</span></span><br>`/users` <br><span data-ttu-id="e051c-168">对特定用户更改：</span><span class="sxs-lookup"><span data-stu-id="e051c-168">Changes to a specific user:</span></span><br>`/users/{id}`| <span data-ttu-id="e051c-169">否</span><span class="sxs-lookup"><span data-stu-id="e051c-169">No</span></span> |


> <span data-ttu-id="e051c-170">**注意**：以 `/users/{id}` 开头的任何资源路径还可接受 `/me` 以引用已登录的用户。</span><span class="sxs-lookup"><span data-stu-id="e051c-170">**Note**: Any resource path that begins with `/users/{id}` can also accept `/me` to reference the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="e051c-171">权限</span><span class="sxs-lookup"><span data-stu-id="e051c-171">Permissions</span></span>

<span data-ttu-id="e051c-172">通常订阅操作需要拥有对资源的读取权限。</span><span class="sxs-lookup"><span data-stu-id="e051c-172">In general, subscription operations require read permission to the resource.</span></span> <span data-ttu-id="e051c-173">例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。</span><span class="sxs-lookup"><span data-stu-id="e051c-173">For example, to get notifications for messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="e051c-174">[创建订阅](../api/subscription-post-subscriptions.md)一文列出了各个资源类型所需的权限。</span><span class="sxs-lookup"><span data-stu-id="e051c-174">The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type.</span></span> <span data-ttu-id="e051c-175">下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。</span><span class="sxs-lookup"><span data-stu-id="e051c-175">The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="e051c-176">权限类型</span><span class="sxs-lookup"><span data-stu-id="e051c-176">Permission type</span></span>                        | <span data-ttu-id="e051c-177">支持的资源类型</span><span class="sxs-lookup"><span data-stu-id="e051c-177">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="e051c-178">委派 - 工作或学校帐户</span><span class="sxs-lookup"><span data-stu-id="e051c-178">Delegated - work or school account</span></span>     | <span data-ttu-id="e051c-179">[alert][]、 [contact][]、 [conversation][]、 [driveItem][]、 [list][]、 [event][]、 [group][]、 [message][]、 [user][]、 [presence][]、 [chatMessage][] (preview) ， [todoTask][]</span><span class="sxs-lookup"><span data-stu-id="e051c-179">[alert][], [contact][], [conversation][], [driveItem][], [list][], [event][], [group][], [message][], [user][], [presence][], [chatMessage][] (preview), [todoTask][]</span></span> |
| <span data-ttu-id="e051c-180">委派 - 个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="e051c-180">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="e051c-181">[contact][]、 [driveItem][]、 [list][]、 [event][]、 [message][]、[todoTask][]</span><span class="sxs-lookup"><span data-stu-id="e051c-181">[contact][], [driveItem][], [list][], [event][], [message][],[todoTask][]</span></span>                                     |
| <span data-ttu-id="e051c-182">Application</span><span class="sxs-lookup"><span data-stu-id="e051c-182">Application</span></span>                            | <span data-ttu-id="e051c-183">[alert][]、 [contact][]、 [driveItem][]、 [list][]、 [event][]、 [group][]、 [message][]、 [user][]、 [callRecord][]、 [chatMessage][]、 [printer][]、 [printTaskDefinition][]</span><span class="sxs-lookup"><span data-stu-id="e051c-183">[alert][], [contact][], [driveItem][], [list][], [event][], [group][], [message][], [user][], [callRecord][], [chatMessage][], [printer][], [printTaskDefinition][]</span></span>|

## <a name="see-also"></a><span data-ttu-id="e051c-184">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e051c-184">See also</span></span>

- [<span data-ttu-id="e051c-185">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="e051c-185">Subscription resource type</span></span>](subscription.md)
- [<span data-ttu-id="e051c-186">列出订阅</span><span class="sxs-lookup"><span data-stu-id="e051c-186">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="e051c-187">获取订阅</span><span class="sxs-lookup"><span data-stu-id="e051c-187">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="e051c-188">创建订阅</span><span class="sxs-lookup"><span data-stu-id="e051c-188">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="e051c-189">更新订阅</span><span class="sxs-lookup"><span data-stu-id="e051c-189">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="e051c-190">删除订阅</span><span class="sxs-lookup"><span data-stu-id="e051c-190">Delete subscription</span></span>](../api/subscription-delete.md)

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

