---
title: 使用 Microsoft Graph API 获取更改通知
description: Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。 客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。 客户端应用使用通知在更改时更新其状态。 有关详细信息（包括如何订阅和处理传入通知），请参阅“设置用户数据更改的通知”。
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: dfd7991070e29d948ab03511726fbc59cd86ea62
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897475"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="4a732-106">使用 Microsoft Graph API 获取更改通知</span><span class="sxs-lookup"><span data-stu-id="4a732-106">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="4a732-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a732-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4a732-108">Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。</span><span class="sxs-lookup"><span data-stu-id="4a732-108">The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="4a732-109">客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。</span><span class="sxs-lookup"><span data-stu-id="4a732-109">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="4a732-110">客户端应用使用通知在更改时更新其状态。</span><span class="sxs-lookup"><span data-stu-id="4a732-110">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="4a732-111">有关详细信息（包括如何订阅和处理传入通知），请参阅[设置用户数据更改的通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="4a732-111">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="4a732-112">使用 Microsoft Graph API，应用可以订阅以下资源的更改：</span><span class="sxs-lookup"><span data-stu-id="4a732-112">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

| <span data-ttu-id="4a732-113">**资源**</span><span class="sxs-lookup"><span data-stu-id="4a732-113">**Resource**</span></span> | <span data-ttu-id="4a732-114">**支持的资源路径**</span><span class="sxs-lookup"><span data-stu-id="4a732-114">**Supported resource paths**</span></span> | <span data-ttu-id="4a732-115">**可包含在通知中的资源数据**</span><span class="sxs-lookup"><span data-stu-id="4a732-115">**Resource data can be included in notifications**</span></span>                  |
|:----------------|:------------|:-----------------------------------------|
| <span data-ttu-id="4a732-116">Outlook [邮件][]</span><span class="sxs-lookup"><span data-stu-id="4a732-116">Outlook [message][]</span></span> | <span data-ttu-id="4a732-117">对用户邮箱中的所有邮件更改：</span><span class="sxs-lookup"><span data-stu-id="4a732-117">Changes to all messages in a user's mailbox:</span></span> <br>`/users/{id}/messages`<br><span data-ttu-id="4a732-118">对用户收件箱中的所有邮件更改：</span><span class="sxs-lookup"><span data-stu-id="4a732-118">Changes to messages in a user's Inbox:</span></span><br>`/users/{id}/mailFolders('inbox')/messages` | <span data-ttu-id="4a732-119">否</span><span class="sxs-lookup"><span data-stu-id="4a732-119">No</span></span> |
| <span data-ttu-id="4a732-120">Outlook [事件][]</span><span class="sxs-lookup"><span data-stu-id="4a732-120">Outlook [event][]</span></span> | <span data-ttu-id="4a732-121">对用户邮箱中的所有事件更改：</span><span class="sxs-lookup"><span data-stu-id="4a732-121">Changes to all events in a user's mailbox:</span></span><br>`/users/{id}/events` | <span data-ttu-id="4a732-122">否</span><span class="sxs-lookup"><span data-stu-id="4a732-122">No</span></span> |
| <span data-ttu-id="4a732-123">Outlook 个人[联系人][]</span><span class="sxs-lookup"><span data-stu-id="4a732-123">Outlook personal [contact][]</span></span> | <span data-ttu-id="4a732-124">对用户邮箱中的所有个人联系人更改：</span><span class="sxs-lookup"><span data-stu-id="4a732-124">Changes to all personal contacts in a user's mailbox:</span></span><br>`/users/{id}/contacts` | <span data-ttu-id="4a732-125">否</span><span class="sxs-lookup"><span data-stu-id="4a732-125">No</span></span> |
| <span data-ttu-id="4a732-126">[用户][]</span><span class="sxs-lookup"><span data-stu-id="4a732-126">[user][]</span></span> | <span data-ttu-id="4a732-127">对所有用户更改：</span><span class="sxs-lookup"><span data-stu-id="4a732-127">Changes to all users:</span></span><br>`/users` <br><span data-ttu-id="4a732-128">对特定用户更改：</span><span class="sxs-lookup"><span data-stu-id="4a732-128">Changes to a specific user:</span></span><br>`/users/{id}`| <span data-ttu-id="4a732-129">否</span><span class="sxs-lookup"><span data-stu-id="4a732-129">No</span></span> |
| <span data-ttu-id="4a732-130">[组][]</span><span class="sxs-lookup"><span data-stu-id="4a732-130">[group][]</span></span> | <span data-ttu-id="4a732-131">对所有组更改：</span><span class="sxs-lookup"><span data-stu-id="4a732-131">Changes to all groups:</span></span><br>`/groups` <br><span data-ttu-id="4a732-132">对特定组更改：</span><span class="sxs-lookup"><span data-stu-id="4a732-132">Changes to a specific group:</span></span><br>`/groups/{id}`<br><span data-ttu-id="4a732-133">对特定组的所有者所做的更改：</span><span class="sxs-lookup"><span data-stu-id="4a732-133">Changes to owners of a specific group:</span></span><br>`/groups/{id}/owners`<br><span data-ttu-id="4a732-134">对特定组的成员所做的更改：</span><span class="sxs-lookup"><span data-stu-id="4a732-134">Changes to members of a specific group:</span></span><br>`/groups/{id}/members`  | <span data-ttu-id="4a732-135">否</span><span class="sxs-lookup"><span data-stu-id="4a732-135">No</span></span> |
| <span data-ttu-id="4a732-136">Microsoft 365 组[对话][]</span><span class="sxs-lookup"><span data-stu-id="4a732-136">Microsoft 365 group [conversation][]</span></span> | <span data-ttu-id="4a732-137">查看组的对话：</span><span class="sxs-lookup"><span data-stu-id="4a732-137">Changes to a group's conversations:</span></span><br>`groups/{id}/conversations` | <span data-ttu-id="4a732-138">否</span><span class="sxs-lookup"><span data-stu-id="4a732-138">No</span></span> |
| <span data-ttu-id="4a732-139">OneDrive（个人版）上的 [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="4a732-139">[driveItem][] on OneDrive (personal)</span></span> | <span data-ttu-id="4a732-140">对_任何文件夹_的层次结构内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="4a732-140">Changes to content within the hierarchy of _any folder_:</span></span><br>`/users/{id}/drive/root` | <span data-ttu-id="4a732-141">否</span><span class="sxs-lookup"><span data-stu-id="4a732-141">No</span></span> |
| <span data-ttu-id="4a732-142">OneDrive for Business 上的 [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="4a732-142">[driveItem][] on OneDrive for Business</span></span> | <span data-ttu-id="4a732-143">对_根文件夹_的层次结构内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="4a732-143">Changes to content within the hierarchy of the _root folder_:</span></span><br>`/drives/{id}/root`<br> `/users/{id}/drive/root` | <span data-ttu-id="4a732-144">否</span><span class="sxs-lookup"><span data-stu-id="4a732-144">No</span></span> |
| <span data-ttu-id="4a732-145">SharePoint [网站][]下的[列表][]</span><span class="sxs-lookup"><span data-stu-id="4a732-145">[list][] under a SharePoint [site][]</span></span> | <span data-ttu-id="4a732-146">_列表_内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="4a732-146">Changes to content within the _list_:</span></span> <br>`/sites/{id}/lists/{id}` | <span data-ttu-id="4a732-147">否</span><span class="sxs-lookup"><span data-stu-id="4a732-147">No</span></span> |
| <span data-ttu-id="4a732-148">安全[警报][]</span><span class="sxs-lookup"><span data-stu-id="4a732-148">Security [alert][]</span></span> | <span data-ttu-id="4a732-149">对特定警报更改：</span><span class="sxs-lookup"><span data-stu-id="4a732-149">Changes to a specific alert:</span></span><br>`/security/alerts/{id}` <br><span data-ttu-id="4a732-150">对已筛选的警报更改：</span><span class="sxs-lookup"><span data-stu-id="4a732-150">Changes to filtered alerts:</span></span><br> `/security/alerts/?$filter`| <span data-ttu-id="4a732-151">否</span><span class="sxs-lookup"><span data-stu-id="4a732-151">No</span></span> |
| <span data-ttu-id="4a732-152">团队[callRecord][]</span><span class="sxs-lookup"><span data-stu-id="4a732-152">Teams [callRecord][]</span></span> | <span data-ttu-id="4a732-153">对_所有_呼叫记录的更改：`/communications/callRecords`</span><span class="sxs-lookup"><span data-stu-id="4a732-153">Changes to _all_ call records: `/communications/callRecords`</span></span> | <span data-ttu-id="4a732-154">否</span><span class="sxs-lookup"><span data-stu-id="4a732-154">No</span></span> |
| <span data-ttu-id="4a732-155">Teams [chatmessage](/graph/api/resources/subscription?view=graph-rest-v1.0)</span><span class="sxs-lookup"><span data-stu-id="4a732-155">Teams [chatmessage](/graph/api/resources/subscription?view=graph-rest-v1.0)</span></span> | <span data-ttu-id="4a732-156">对所有团队中所有频道聊天消息更改：</span><span class="sxs-lookup"><span data-stu-id="4a732-156">Changes to chat messages in all channels in all teams:</span></span><br>`/teams/allMessages` <br><span data-ttu-id="4a732-157">对特定频道中的聊天消息更改：</span><span class="sxs-lookup"><span data-stu-id="4a732-157">Changes to chat messages in a specific channel:</span></span><br>`/teams/{id}/channels/{id}/messages`<br><span data-ttu-id="4a732-158">对所有聊天的消息更改：</span><span class="sxs-lookup"><span data-stu-id="4a732-158">Changes to chat messages in all chats:</span></span><br>`/chats/allMessages` <br><span data-ttu-id="4a732-159">对特定聊天中的消息更改：</span><span class="sxs-lookup"><span data-stu-id="4a732-159">Changes to chat messages in a specific chat:</span></span><br>`/chats/{id}/messages` | <span data-ttu-id="4a732-160">是</span><span class="sxs-lookup"><span data-stu-id="4a732-160">Yes</span></span> |

> <span data-ttu-id="4a732-161">**注意**：以 `/users/{id}` 开头的任何资源路径还可接受 `/me` 以引用已登录的用户。</span><span class="sxs-lookup"><span data-stu-id="4a732-161">**Note**: Any resource path that begins with `/users/{id}` can also accept `/me` to reference the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a732-162">权限</span><span class="sxs-lookup"><span data-stu-id="4a732-162">Permissions</span></span>

<span data-ttu-id="4a732-163">通常订阅操作需要拥有对资源的读取权限。</span><span class="sxs-lookup"><span data-stu-id="4a732-163">In general, subscription operations require read permission to the resource.</span></span> <span data-ttu-id="4a732-164">例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。</span><span class="sxs-lookup"><span data-stu-id="4a732-164">For example, to get notifications for messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="4a732-165">[创建订阅](../api/subscription-post-subscriptions.md)一文列出了各个资源类型所需的权限。</span><span class="sxs-lookup"><span data-stu-id="4a732-165">The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type.</span></span> <span data-ttu-id="4a732-166">下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。</span><span class="sxs-lookup"><span data-stu-id="4a732-166">The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="4a732-167">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a732-167">Permission type</span></span>                        | <span data-ttu-id="4a732-168">支持的资源类型</span><span class="sxs-lookup"><span data-stu-id="4a732-168">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="4a732-169">委派 - 工作或学校帐户</span><span class="sxs-lookup"><span data-stu-id="4a732-169">Delegated - work or school account</span></span>     | <span data-ttu-id="4a732-170">[警报][]、[联系人][]、[对话][]、[driveItem][]、[列表][]、 [事件][]、[组][]、[邮件][]、[用户][]</span><span class="sxs-lookup"><span data-stu-id="4a732-170">[alert][], [contact][], [conversation][], [driveItem][], [list][], [event][], [group][], [message][], [user][]</span></span>|
| <span data-ttu-id="4a732-171">委派 - 个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="4a732-171">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="4a732-172">[联系人][]、[driveItem][]、[列表][]、[事件][]、[邮件][]</span><span class="sxs-lookup"><span data-stu-id="4a732-172">[contact][], [driveItem][], [list][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="4a732-173">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a732-173">Application</span></span>                            | <span data-ttu-id="4a732-174">[alert][]、 [contact][]、 [list][]、 [driveItem][]、 [event][]、 [group][]、 [message][]、 [user][]、 [callRecord][]</span><span class="sxs-lookup"><span data-stu-id="4a732-174">[alert][], [contact][], [list][], [driveItem][], [event][], [group][], [message][], [user][], [callRecord][]</span></span>|


## <a name="see-also"></a><span data-ttu-id="4a732-175">另请参阅</span><span class="sxs-lookup"><span data-stu-id="4a732-175">See also</span></span>

- [<span data-ttu-id="4a732-176">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="4a732-176">Subscription resource type</span></span>](./subscription.md)
- [<span data-ttu-id="4a732-177">列出订阅</span><span class="sxs-lookup"><span data-stu-id="4a732-177">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="4a732-178">获取订阅</span><span class="sxs-lookup"><span data-stu-id="4a732-178">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="4a732-179">创建订阅</span><span class="sxs-lookup"><span data-stu-id="4a732-179">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="4a732-180">更新订阅</span><span class="sxs-lookup"><span data-stu-id="4a732-180">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="4a732-181">删除订阅</span><span class="sxs-lookup"><span data-stu-id="4a732-181">Delete subscription</span></span>](../api/subscription-delete.md)

[联系人]: ./contact.md
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
