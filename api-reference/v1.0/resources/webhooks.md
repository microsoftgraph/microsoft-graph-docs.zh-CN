---
title: 使用 Microsoft Graph API 获取更改通知
description: 为客户提供更改通知。
localization_priority: Priority
author: Jumaodhiss
ms.prod: change-notifications
doc_type: conceptualPageType
ms.openlocfilehash: 970c27a57f0dacaae0c4935c09db3434c72cbea6
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468973"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="9f937-103">使用 Microsoft Graph API 获取更改通知</span><span class="sxs-lookup"><span data-stu-id="9f937-103">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="9f937-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f937-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9f937-105">Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。</span><span class="sxs-lookup"><span data-stu-id="9f937-105">The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="9f937-106">客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。</span><span class="sxs-lookup"><span data-stu-id="9f937-106">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="9f937-107">客户端应用使用通知在更改时更新其状态。</span><span class="sxs-lookup"><span data-stu-id="9f937-107">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="9f937-108">有关详细信息（包括如何订阅和处理传入通知），请参阅[设置用户数据更改的通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="9f937-108">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="9f937-109">使用 Microsoft Graph API，应用可以订阅以下资源的更改：</span><span class="sxs-lookup"><span data-stu-id="9f937-109">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

| <span data-ttu-id="9f937-110">**资源**</span><span class="sxs-lookup"><span data-stu-id="9f937-110">**Resource**</span></span> | <span data-ttu-id="9f937-111">**支持的资源路径**</span><span class="sxs-lookup"><span data-stu-id="9f937-111">**Supported resource paths**</span></span> | <span data-ttu-id="9f937-112">**可包含在通知中的资源数据**</span><span class="sxs-lookup"><span data-stu-id="9f937-112">**Resource data can be included in notifications**</span></span>                  |
|:----------------|:------------|:-----------------------------------------|
| <span data-ttu-id="9f937-113">云打印 [打印机][]</span><span class="sxs-lookup"><span data-stu-id="9f937-113">Cloud printing [printer][]</span></span> | <span data-ttu-id="9f937-114">打印作业准备好下载时的变化（作业可打印事件）：</span><span class="sxs-lookup"><span data-stu-id="9f937-114">Changes when a print job is ready to be downloaded (JobFetchable event):</span></span><br>`/print/printers/{id}/jobs` | <span data-ttu-id="9f937-115">不支持</span><span class="sxs-lookup"><span data-stu-id="9f937-115">No</span></span> |
| <span data-ttu-id="9f937-116">云打印 [printTaskDefinition][]</span><span class="sxs-lookup"><span data-stu-id="9f937-116">Cloud printing [printTaskDefinition][]</span></span> | <span data-ttu-id="9f937-117">在队列中具有有效作业时的变化（作业启动事件）：</span><span class="sxs-lookup"><span data-stu-id="9f937-117">Changes when there is a valid job in the queue (JobStarted event) :</span></span><br>`/print/printtaskdefinition/{id}/tasks` | <span data-ttu-id="9f937-118">不支持</span><span class="sxs-lookup"><span data-stu-id="9f937-118">No</span></span> |
| <span data-ttu-id="9f937-119">Outlook [邮件][]</span><span class="sxs-lookup"><span data-stu-id="9f937-119">Outlook [message][]</span></span> | <span data-ttu-id="9f937-120">对用户邮箱中的所有邮件更改：</span><span class="sxs-lookup"><span data-stu-id="9f937-120">Changes to all messages in a user's mailbox:</span></span> <br>`/users/{id}/messages`<br><span data-ttu-id="9f937-121">对用户收件箱中的所有邮件更改：</span><span class="sxs-lookup"><span data-stu-id="9f937-121">Changes to messages in a user's Inbox:</span></span><br>`/users/{id}/mailFolders('inbox')/messages` | <span data-ttu-id="9f937-122">否</span><span class="sxs-lookup"><span data-stu-id="9f937-122">No</span></span> |
| <span data-ttu-id="9f937-123">Outlook [事件][]</span><span class="sxs-lookup"><span data-stu-id="9f937-123">Outlook [event][]</span></span> | <span data-ttu-id="9f937-124">对用户邮箱中的所有事件更改：</span><span class="sxs-lookup"><span data-stu-id="9f937-124">Changes to all events in a user's mailbox:</span></span><br>`/users/{id}/events` | <span data-ttu-id="9f937-125">否</span><span class="sxs-lookup"><span data-stu-id="9f937-125">No</span></span> |
| <span data-ttu-id="9f937-126">Outlook 个人[联系人][]</span><span class="sxs-lookup"><span data-stu-id="9f937-126">Outlook personal [contact][]</span></span> | <span data-ttu-id="9f937-127">对用户邮箱中的所有个人联系人更改：</span><span class="sxs-lookup"><span data-stu-id="9f937-127">Changes to all personal contacts in a user's mailbox:</span></span><br>`/users/{id}/contacts` | <span data-ttu-id="9f937-128">否</span><span class="sxs-lookup"><span data-stu-id="9f937-128">No</span></span> |
| <span data-ttu-id="9f937-129">[用户][]</span><span class="sxs-lookup"><span data-stu-id="9f937-129">[user][]</span></span> | <span data-ttu-id="9f937-130">对所有用户更改：</span><span class="sxs-lookup"><span data-stu-id="9f937-130">Changes to all users:</span></span><br>`/users` <br><span data-ttu-id="9f937-131">对特定用户更改：</span><span class="sxs-lookup"><span data-stu-id="9f937-131">Changes to a specific user:</span></span><br>`/users/{id}`| <span data-ttu-id="9f937-132">否</span><span class="sxs-lookup"><span data-stu-id="9f937-132">No</span></span> |
| <span data-ttu-id="9f937-133">[组][]</span><span class="sxs-lookup"><span data-stu-id="9f937-133">[group][]</span></span> | <span data-ttu-id="9f937-134">对所有组更改：</span><span class="sxs-lookup"><span data-stu-id="9f937-134">Changes to all groups:</span></span><br>`/groups` <br><span data-ttu-id="9f937-135">对特定组更改：</span><span class="sxs-lookup"><span data-stu-id="9f937-135">Changes to a specific group:</span></span><br>`/groups/{id}`<br><span data-ttu-id="9f937-136">对特定组的所有者所做的更改：</span><span class="sxs-lookup"><span data-stu-id="9f937-136">Changes to owners of a specific group:</span></span><br>`/groups/{id}/owners`<br><span data-ttu-id="9f937-137">对特定组成员所做的更改：</span><span class="sxs-lookup"><span data-stu-id="9f937-137">Changes to members of a specific group:</span></span><br>`/groups/{id}/members`  | <span data-ttu-id="9f937-138">否</span><span class="sxs-lookup"><span data-stu-id="9f937-138">No</span></span> |
| <span data-ttu-id="9f937-139">Microsoft 365 组[对话][]</span><span class="sxs-lookup"><span data-stu-id="9f937-139">Microsoft 365 group [conversation][]</span></span> | <span data-ttu-id="9f937-140">查看组的对话：</span><span class="sxs-lookup"><span data-stu-id="9f937-140">Changes to a group's conversations:</span></span><br>`groups/{id}/conversations` | <span data-ttu-id="9f937-141">否</span><span class="sxs-lookup"><span data-stu-id="9f937-141">No</span></span> |
| <span data-ttu-id="9f937-142">OneDrive（个人版）上的 [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="9f937-142">[driveItem][] on OneDrive (personal)</span></span> | <span data-ttu-id="9f937-143">对 _任何文件夹_ 的层次结构内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="9f937-143">Changes to content within the hierarchy of _any folder_:</span></span><br>`/users/{id}/drive/root` | <span data-ttu-id="9f937-144">否</span><span class="sxs-lookup"><span data-stu-id="9f937-144">No</span></span> |
| <span data-ttu-id="9f937-145">OneDrive for Business 上的 [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="9f937-145">[driveItem][] on OneDrive for Business</span></span> | <span data-ttu-id="9f937-146">对 _根文件夹_ 的层次结构内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="9f937-146">Changes to content within the hierarchy of the _root folder_:</span></span><br>`/drives/{id}/root`<br> `/users/{id}/drive/root` | <span data-ttu-id="9f937-147">否</span><span class="sxs-lookup"><span data-stu-id="9f937-147">No</span></span> |
| <span data-ttu-id="9f937-148">SharePoint [网站][]下的[列表][]</span><span class="sxs-lookup"><span data-stu-id="9f937-148">[list][] under a SharePoint [site][]</span></span> | <span data-ttu-id="9f937-149">_列表_ 内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="9f937-149">Changes to content within the _list_:</span></span> <br>`/sites/{id}/lists/{id}` | <span data-ttu-id="9f937-150">否</span><span class="sxs-lookup"><span data-stu-id="9f937-150">No</span></span> |
| <span data-ttu-id="9f937-151">安全[警报][]</span><span class="sxs-lookup"><span data-stu-id="9f937-151">Security [alert][]</span></span> | <span data-ttu-id="9f937-152">对特定警报更改：</span><span class="sxs-lookup"><span data-stu-id="9f937-152">Changes to a specific alert:</span></span><br>`/security/alerts/{id}` <br><span data-ttu-id="9f937-153">对已筛选的警报更改：</span><span class="sxs-lookup"><span data-stu-id="9f937-153">Changes to filtered alerts:</span></span><br> `/security/alerts/?$filter`| <span data-ttu-id="9f937-154">否</span><span class="sxs-lookup"><span data-stu-id="9f937-154">No</span></span> |
| <span data-ttu-id="9f937-155">Teams [callRecord][]</span><span class="sxs-lookup"><span data-stu-id="9f937-155">Teams [callRecord][]</span></span> | <span data-ttu-id="9f937-156">更改 _所有_ 呼叫记录： `/communications/callRecords`</span><span class="sxs-lookup"><span data-stu-id="9f937-156">Changes to _all_ call records: `/communications/callRecords`</span></span> | <span data-ttu-id="9f937-157">否</span><span class="sxs-lookup"><span data-stu-id="9f937-157">No</span></span> |
| <span data-ttu-id="9f937-158">Teams [chatmessage][]</span><span class="sxs-lookup"><span data-stu-id="9f937-158">Teams [chatmessage][]</span></span> | <span data-ttu-id="9f937-159">对所有团队中所有频道聊天消息更改：</span><span class="sxs-lookup"><span data-stu-id="9f937-159">Changes to chat messages in all channels in all teams:</span></span><br>`/teams/getAllMessages` <br><span data-ttu-id="9f937-160">对特定频道中的聊天消息更改：</span><span class="sxs-lookup"><span data-stu-id="9f937-160">Changes to chat messages in a specific channel:</span></span><br>`/teams/{id}/channels/{id}/messages`<br><span data-ttu-id="9f937-161">对所有聊天的消息更改：</span><span class="sxs-lookup"><span data-stu-id="9f937-161">Changes to chat messages in all chats:</span></span><br>`/chats/getAllMessages` <br><span data-ttu-id="9f937-162">对特定聊天中的消息更改：</span><span class="sxs-lookup"><span data-stu-id="9f937-162">Changes to chat messages in a specific chat:</span></span><br>`/chats/{id}/messages` | <span data-ttu-id="9f937-163">是</span><span class="sxs-lookup"><span data-stu-id="9f937-163">Yes</span></span> |

> <span data-ttu-id="9f937-164">**注意**：以 `/users/{id}` 开头的任何资源路径还可接受 `/me` 以引用已登录的用户。</span><span class="sxs-lookup"><span data-stu-id="9f937-164">**Note**: Any resource path that begins with `/users/{id}` can also accept `/me` to reference the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f937-165">权限</span><span class="sxs-lookup"><span data-stu-id="9f937-165">Permissions</span></span>

<span data-ttu-id="9f937-166">通常订阅操作需要拥有对资源的读取权限。</span><span class="sxs-lookup"><span data-stu-id="9f937-166">In general, subscription operations require read permission to the resource.</span></span> <span data-ttu-id="9f937-167">例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。</span><span class="sxs-lookup"><span data-stu-id="9f937-167">For example, to get notifications for messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="9f937-168">[创建订阅](../api/subscription-post-subscriptions.md)一文列出了各个资源类型所需的权限。</span><span class="sxs-lookup"><span data-stu-id="9f937-168">The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type.</span></span> <span data-ttu-id="9f937-169">下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。</span><span class="sxs-lookup"><span data-stu-id="9f937-169">The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="9f937-170">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f937-170">Permission type</span></span>                        | <span data-ttu-id="9f937-171">支持的资源类型</span><span class="sxs-lookup"><span data-stu-id="9f937-171">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="9f937-172">委派 - 工作或学校帐户</span><span class="sxs-lookup"><span data-stu-id="9f937-172">Delegated - work or school account</span></span>     | <span data-ttu-id="9f937-173">[警报][]、[联系人][]、[对话][]、[driveItem][]、[列表][]、 [事件][]、[组][]、[邮件][]、[用户][]</span><span class="sxs-lookup"><span data-stu-id="9f937-173">[alert][], [contact][], [conversation][], [driveItem][], [list][], [event][], [group][], [message][], [user][]</span></span>|
| <span data-ttu-id="9f937-174">委派 - 个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="9f937-174">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="9f937-175">[联系人][]、[driveItem][]、[列表][]、[事件][]、[邮件][]</span><span class="sxs-lookup"><span data-stu-id="9f937-175">[contact][], [driveItem][], [list][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="9f937-176">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f937-176">Application</span></span>                            | <span data-ttu-id="9f937-177">[警报][]、 [联系人][]、 [列表][]、 [driveItem][]、 [event][]、 [组][]、 [、][]， [用户][]、 [callRecord][]、 [chatMessage][]、 [打印机][]、 [printTaskDefinition][]</span><span class="sxs-lookup"><span data-stu-id="9f937-177">[alert][], [contact][], [list][], [driveItem][], [event][], [group][], [message][], [user][], [callRecord][], [chatMessage][], [printer][], [printTaskDefinition][]</span></span>|


## <a name="see-also"></a><span data-ttu-id="9f937-178">另请参阅</span><span class="sxs-lookup"><span data-stu-id="9f937-178">See also</span></span>

- [<span data-ttu-id="9f937-179">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="9f937-179">Subscription resource type</span></span>](./subscription.md)
- [<span data-ttu-id="9f937-180">列出订阅</span><span class="sxs-lookup"><span data-stu-id="9f937-180">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="9f937-181">获取订阅</span><span class="sxs-lookup"><span data-stu-id="9f937-181">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="9f937-182">创建订阅</span><span class="sxs-lookup"><span data-stu-id="9f937-182">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="9f937-183">更新订阅</span><span class="sxs-lookup"><span data-stu-id="9f937-183">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="9f937-184">删除订阅</span><span class="sxs-lookup"><span data-stu-id="9f937-184">Delete subscription</span></span>](../api/subscription-delete.md)

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

