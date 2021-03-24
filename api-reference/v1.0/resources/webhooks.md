---
title: 使用 Microsoft Graph API 获取更改通知
description: Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。 客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。 客户端应用使用通知在更改时更新其状态。 有关详细信息（包括如何订阅和处理传入通知），请参阅“设置用户数据更改的通知”。
localization_priority: Priority
author: davidmu1
ms.prod: change-notifications
doc_type: conceptualPageType
ms.openlocfilehash: 19ff391309089802dcb15494eba1ac6345325b24
ms.sourcegitcommit: 74a1fb3874e04c488e1b87dcee80d76cc586c1f3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51030979"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="46e8c-106">使用 Microsoft Graph API 获取更改通知</span><span class="sxs-lookup"><span data-stu-id="46e8c-106">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="46e8c-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46e8c-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="46e8c-108">Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。</span><span class="sxs-lookup"><span data-stu-id="46e8c-108">The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="46e8c-109">客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。</span><span class="sxs-lookup"><span data-stu-id="46e8c-109">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="46e8c-110">客户端应用使用通知在更改时更新其状态。</span><span class="sxs-lookup"><span data-stu-id="46e8c-110">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="46e8c-111">有关详细信息（包括如何订阅和处理传入通知），请参阅[设置用户数据更改的通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="46e8c-111">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="46e8c-112">使用 Microsoft Graph API，应用可以订阅以下资源的更改：</span><span class="sxs-lookup"><span data-stu-id="46e8c-112">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

| <span data-ttu-id="46e8c-113">**资源**</span><span class="sxs-lookup"><span data-stu-id="46e8c-113">**Resource**</span></span> | <span data-ttu-id="46e8c-114">**支持的资源路径**</span><span class="sxs-lookup"><span data-stu-id="46e8c-114">**Supported resource paths**</span></span> | <span data-ttu-id="46e8c-115">**可包含在通知中的资源数据**</span><span class="sxs-lookup"><span data-stu-id="46e8c-115">**Resource data can be included in notifications**</span></span>                  |
|:----------------|:------------|:-----------------------------------------|
| <span data-ttu-id="46e8c-116">云打印 [打印机][]</span><span class="sxs-lookup"><span data-stu-id="46e8c-116">Cloud printing [printer][]</span></span> | <span data-ttu-id="46e8c-117">打印作业准备好下载时的变化（作业可打印事件）：</span><span class="sxs-lookup"><span data-stu-id="46e8c-117">Changes when a print job is ready to be downloaded (JobFetchable event):</span></span><br>`/print/printers/{id}/jobs` | <span data-ttu-id="46e8c-118">不支持</span><span class="sxs-lookup"><span data-stu-id="46e8c-118">No</span></span> |
| <span data-ttu-id="46e8c-119">云打印 [printTaskDefinition][]</span><span class="sxs-lookup"><span data-stu-id="46e8c-119">Cloud printing [printTaskDefinition][]</span></span> | <span data-ttu-id="46e8c-120">在队列中具有有效作业时的变化（作业启动事件）：</span><span class="sxs-lookup"><span data-stu-id="46e8c-120">Changes when there is a valid job in the queue (JobStarted event) :</span></span><br>`/print/printtaskdefinition/{id}/tasks` | <span data-ttu-id="46e8c-121">不支持</span><span class="sxs-lookup"><span data-stu-id="46e8c-121">No</span></span> |
| <span data-ttu-id="46e8c-122">Outlook [邮件][]</span><span class="sxs-lookup"><span data-stu-id="46e8c-122">Outlook [message][]</span></span> | <span data-ttu-id="46e8c-123">对用户邮箱中的所有邮件更改：</span><span class="sxs-lookup"><span data-stu-id="46e8c-123">Changes to all messages in a user's mailbox:</span></span> <br>`/users/{id}/messages`<br><span data-ttu-id="46e8c-124">对用户收件箱中的所有邮件更改：</span><span class="sxs-lookup"><span data-stu-id="46e8c-124">Changes to messages in a user's Inbox:</span></span><br>`/users/{id}/mailFolders('inbox')/messages` | <span data-ttu-id="46e8c-125">否</span><span class="sxs-lookup"><span data-stu-id="46e8c-125">No</span></span> |
| <span data-ttu-id="46e8c-126">Outlook [事件][]</span><span class="sxs-lookup"><span data-stu-id="46e8c-126">Outlook [event][]</span></span> | <span data-ttu-id="46e8c-127">对用户邮箱中的所有事件更改：</span><span class="sxs-lookup"><span data-stu-id="46e8c-127">Changes to all events in a user's mailbox:</span></span><br>`/users/{id}/events` | <span data-ttu-id="46e8c-128">否</span><span class="sxs-lookup"><span data-stu-id="46e8c-128">No</span></span> |
| <span data-ttu-id="46e8c-129">Outlook 个人[联系人][]</span><span class="sxs-lookup"><span data-stu-id="46e8c-129">Outlook personal [contact][]</span></span> | <span data-ttu-id="46e8c-130">对用户邮箱中的所有个人联系人更改：</span><span class="sxs-lookup"><span data-stu-id="46e8c-130">Changes to all personal contacts in a user's mailbox:</span></span><br>`/users/{id}/contacts` | <span data-ttu-id="46e8c-131">否</span><span class="sxs-lookup"><span data-stu-id="46e8c-131">No</span></span> |
| <span data-ttu-id="46e8c-132">[用户][]</span><span class="sxs-lookup"><span data-stu-id="46e8c-132">[user][]</span></span> | <span data-ttu-id="46e8c-133">对所有用户更改：</span><span class="sxs-lookup"><span data-stu-id="46e8c-133">Changes to all users:</span></span><br>`/users` <br><span data-ttu-id="46e8c-134">对特定用户更改：</span><span class="sxs-lookup"><span data-stu-id="46e8c-134">Changes to a specific user:</span></span><br>`/users/{id}`| <span data-ttu-id="46e8c-135">否</span><span class="sxs-lookup"><span data-stu-id="46e8c-135">No</span></span> |
| <span data-ttu-id="46e8c-136">[组][]</span><span class="sxs-lookup"><span data-stu-id="46e8c-136">[group][]</span></span> | <span data-ttu-id="46e8c-137">对所有组更改：</span><span class="sxs-lookup"><span data-stu-id="46e8c-137">Changes to all groups:</span></span><br>`/groups` <br><span data-ttu-id="46e8c-138">对特定组更改：</span><span class="sxs-lookup"><span data-stu-id="46e8c-138">Changes to a specific group:</span></span><br>`/groups/{id}`<br><span data-ttu-id="46e8c-139">对特定组的所有者所做的更改：</span><span class="sxs-lookup"><span data-stu-id="46e8c-139">Changes to owners of a specific group:</span></span><br>`/groups/{id}/owners`<br><span data-ttu-id="46e8c-140">对特定组成员所做的更改：</span><span class="sxs-lookup"><span data-stu-id="46e8c-140">Changes to members of a specific group:</span></span><br>`/groups/{id}/members`  | <span data-ttu-id="46e8c-141">否</span><span class="sxs-lookup"><span data-stu-id="46e8c-141">No</span></span> |
| <span data-ttu-id="46e8c-142">Microsoft 365 组[对话][]</span><span class="sxs-lookup"><span data-stu-id="46e8c-142">Microsoft 365 group [conversation][]</span></span> | <span data-ttu-id="46e8c-143">查看组的对话：</span><span class="sxs-lookup"><span data-stu-id="46e8c-143">Changes to a group's conversations:</span></span><br>`groups/{id}/conversations` | <span data-ttu-id="46e8c-144">否</span><span class="sxs-lookup"><span data-stu-id="46e8c-144">No</span></span> |
| <span data-ttu-id="46e8c-145">OneDrive（个人版）上的 [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="46e8c-145">[driveItem][] on OneDrive (personal)</span></span> | <span data-ttu-id="46e8c-146">对 _任何文件夹_ 的层次结构内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="46e8c-146">Changes to content within the hierarchy of _any folder_:</span></span><br>`/users/{id}/drive/root` | <span data-ttu-id="46e8c-147">否</span><span class="sxs-lookup"><span data-stu-id="46e8c-147">No</span></span> |
| <span data-ttu-id="46e8c-148">OneDrive for Business 上的 [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="46e8c-148">[driveItem][] on OneDrive for Business</span></span> | <span data-ttu-id="46e8c-149">对 _根文件夹_ 的层次结构内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="46e8c-149">Changes to content within the hierarchy of the _root folder_:</span></span><br>`/drives/{id}/root`<br> `/users/{id}/drive/root` | <span data-ttu-id="46e8c-150">否</span><span class="sxs-lookup"><span data-stu-id="46e8c-150">No</span></span> |
| <span data-ttu-id="46e8c-151">SharePoint [网站][]下的[列表][]</span><span class="sxs-lookup"><span data-stu-id="46e8c-151">[list][] under a SharePoint [site][]</span></span> | <span data-ttu-id="46e8c-152">_列表_ 内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="46e8c-152">Changes to content within the _list_:</span></span> <br>`/sites/{id}/lists/{id}` | <span data-ttu-id="46e8c-153">否</span><span class="sxs-lookup"><span data-stu-id="46e8c-153">No</span></span> |
| <span data-ttu-id="46e8c-154">安全[警报][]</span><span class="sxs-lookup"><span data-stu-id="46e8c-154">Security [alert][]</span></span> | <span data-ttu-id="46e8c-155">对特定警报更改：</span><span class="sxs-lookup"><span data-stu-id="46e8c-155">Changes to a specific alert:</span></span><br>`/security/alerts/{id}` <br><span data-ttu-id="46e8c-156">对已筛选的警报更改：</span><span class="sxs-lookup"><span data-stu-id="46e8c-156">Changes to filtered alerts:</span></span><br> `/security/alerts/?$filter`| <span data-ttu-id="46e8c-157">否</span><span class="sxs-lookup"><span data-stu-id="46e8c-157">No</span></span> |
| <span data-ttu-id="46e8c-158">Teams [callRecord][]</span><span class="sxs-lookup"><span data-stu-id="46e8c-158">Teams [callRecord][]</span></span> | <span data-ttu-id="46e8c-159">更改 _所有_ 呼叫记录： `/communications/callRecords`</span><span class="sxs-lookup"><span data-stu-id="46e8c-159">Changes to _all_ call records: `/communications/callRecords`</span></span> | <span data-ttu-id="46e8c-160">否</span><span class="sxs-lookup"><span data-stu-id="46e8c-160">No</span></span> |
| <span data-ttu-id="46e8c-161">Teams [chatmessage][]</span><span class="sxs-lookup"><span data-stu-id="46e8c-161">Teams [chatmessage][]</span></span> | <span data-ttu-id="46e8c-162">对所有团队中所有频道聊天消息更改：</span><span class="sxs-lookup"><span data-stu-id="46e8c-162">Changes to chat messages in all channels in all teams:</span></span><br>`/teams/getAllMessages` <br><span data-ttu-id="46e8c-163">对特定频道中的聊天消息更改：</span><span class="sxs-lookup"><span data-stu-id="46e8c-163">Changes to chat messages in a specific channel:</span></span><br>`/teams/{id}/channels/{id}/messages`<br><span data-ttu-id="46e8c-164">对所有聊天的消息更改：</span><span class="sxs-lookup"><span data-stu-id="46e8c-164">Changes to chat messages in all chats:</span></span><br>`/chats/getAllMessages` <br><span data-ttu-id="46e8c-165">对特定聊天中的消息更改：</span><span class="sxs-lookup"><span data-stu-id="46e8c-165">Changes to chat messages in a specific chat:</span></span><br>`/chats/{id}/messages` | <span data-ttu-id="46e8c-166">是</span><span class="sxs-lookup"><span data-stu-id="46e8c-166">Yes</span></span> |

> <span data-ttu-id="46e8c-167">**注意**：以 `/users/{id}` 开头的任何资源路径还可接受 `/me` 以引用已登录的用户。</span><span class="sxs-lookup"><span data-stu-id="46e8c-167">**Note**: Any resource path that begins with `/users/{id}` can also accept `/me` to reference the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="46e8c-168">权限</span><span class="sxs-lookup"><span data-stu-id="46e8c-168">Permissions</span></span>

<span data-ttu-id="46e8c-169">通常订阅操作需要拥有对资源的读取权限。</span><span class="sxs-lookup"><span data-stu-id="46e8c-169">In general, subscription operations require read permission to the resource.</span></span> <span data-ttu-id="46e8c-170">例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。</span><span class="sxs-lookup"><span data-stu-id="46e8c-170">For example, to get notifications for messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="46e8c-171">[创建订阅](../api/subscription-post-subscriptions.md)一文列出了各个资源类型所需的权限。</span><span class="sxs-lookup"><span data-stu-id="46e8c-171">The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type.</span></span> <span data-ttu-id="46e8c-172">下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。</span><span class="sxs-lookup"><span data-stu-id="46e8c-172">The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="46e8c-173">权限类型</span><span class="sxs-lookup"><span data-stu-id="46e8c-173">Permission type</span></span>                        | <span data-ttu-id="46e8c-174">支持的资源类型</span><span class="sxs-lookup"><span data-stu-id="46e8c-174">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="46e8c-175">委派 - 工作或学校帐户</span><span class="sxs-lookup"><span data-stu-id="46e8c-175">Delegated - work or school account</span></span>     | <span data-ttu-id="46e8c-176">[警报][]、[联系人][]、[对话][]、[driveItem][]、[列表][]、 [事件][]、[组][]、[邮件][]、[用户][]</span><span class="sxs-lookup"><span data-stu-id="46e8c-176">[alert][], [contact][], [conversation][], [driveItem][], [list][], [event][], [group][], [message][], [user][]</span></span>|
| <span data-ttu-id="46e8c-177">委派 - 个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="46e8c-177">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="46e8c-178">[联系人][]、[driveItem][]、[列表][]、[事件][]、[邮件][]</span><span class="sxs-lookup"><span data-stu-id="46e8c-178">[contact][], [driveItem][], [list][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="46e8c-179">应用程序</span><span class="sxs-lookup"><span data-stu-id="46e8c-179">Application</span></span>                            | <span data-ttu-id="46e8c-180">[警报][]、 [联系人][]、 [列表][]、 [driveItem][]、 [event][]、 [组][]、 [、][]， [用户][]、 [callRecord][]、 [chatMessage][]、 [打印机][]、 [printTaskDefinition][]</span><span class="sxs-lookup"><span data-stu-id="46e8c-180">[alert][], [contact][], [list][], [driveItem][], [event][], [group][], [message][], [user][], [callRecord][], [chatMessage][], [printer][], [printTaskDefinition][]</span></span>|


## <a name="see-also"></a><span data-ttu-id="46e8c-181">另请参阅</span><span class="sxs-lookup"><span data-stu-id="46e8c-181">See also</span></span>

- [<span data-ttu-id="46e8c-182">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="46e8c-182">Subscription resource type</span></span>](./subscription.md)
- [<span data-ttu-id="46e8c-183">列出订阅</span><span class="sxs-lookup"><span data-stu-id="46e8c-183">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="46e8c-184">获取订阅</span><span class="sxs-lookup"><span data-stu-id="46e8c-184">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="46e8c-185">创建订阅</span><span class="sxs-lookup"><span data-stu-id="46e8c-185">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="46e8c-186">更新订阅</span><span class="sxs-lookup"><span data-stu-id="46e8c-186">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="46e8c-187">删除订阅</span><span class="sxs-lookup"><span data-stu-id="46e8c-187">Delete subscription</span></span>](../api/subscription-delete.md)

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
[打印机]: ./printer.md
[printer]: ./printer.md
[printTaskDefinition]: ./printtaskdefinition.md

