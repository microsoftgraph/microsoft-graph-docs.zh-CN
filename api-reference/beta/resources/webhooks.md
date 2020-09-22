---
title: 使用 Microsoft Graph API 获取更改通知
description: Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。 客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。 客户端应用使用通知在更改时更新其状态。 有关详细信息（包括如何订阅和处理传入通知），请参阅“设置用户数据更改的通知”。
localization_priority: Normal
author: davidmu1
doc_type: conceptualPageType
ms.prod: ''
ms.openlocfilehash: 1c664d25be4e7106ca7d2024de4b8fb4dc52cc54
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192175"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="9c9d6-106">使用 Microsoft Graph API 获取更改通知</span><span class="sxs-lookup"><span data-stu-id="9c9d6-106">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="9c9d6-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c9d6-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c9d6-108">Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。</span><span class="sxs-lookup"><span data-stu-id="9c9d6-108">The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="9c9d6-109">客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。</span><span class="sxs-lookup"><span data-stu-id="9c9d6-109">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="9c9d6-110">客户端应用使用通知在更改时更新其状态。</span><span class="sxs-lookup"><span data-stu-id="9c9d6-110">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="9c9d6-111">有关详细信息（包括如何订阅和处理传入通知），请参阅[设置用户数据更改的通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="9c9d6-111">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="9c9d6-112">使用 Microsoft Graph API，应用可以订阅以下资源的更改：</span><span class="sxs-lookup"><span data-stu-id="9c9d6-112">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

| <span data-ttu-id="9c9d6-113">**资源**</span><span class="sxs-lookup"><span data-stu-id="9c9d6-113">**Resource**</span></span> | <span data-ttu-id="9c9d6-114">**支持的资源路径**</span><span class="sxs-lookup"><span data-stu-id="9c9d6-114">**Supported resource paths**</span></span> | <span data-ttu-id="9c9d6-115">**可包含在通知中的资源数据**</span><span class="sxs-lookup"><span data-stu-id="9c9d6-115">**Resource data can be included in notifications**</span></span>                  |
|:----------------|:------------|:-----------------------------------------|
| <span data-ttu-id="9c9d6-116">Outlook [邮件][]</span><span class="sxs-lookup"><span data-stu-id="9c9d6-116">Outlook [message][]</span></span> | <span data-ttu-id="9c9d6-117">对用户邮箱中的所有邮件更改：</span><span class="sxs-lookup"><span data-stu-id="9c9d6-117">Changes to all messages in a user's mailbox:</span></span> <br>`/users/{id}/messages`<br><span data-ttu-id="9c9d6-118">对用户收件箱中的所有邮件更改：</span><span class="sxs-lookup"><span data-stu-id="9c9d6-118">Changes to messages in a user's Inbox:</span></span><br>`/users/{id}/mailFolders('inbox')/messages` | <span data-ttu-id="9c9d6-119">否</span><span class="sxs-lookup"><span data-stu-id="9c9d6-119">No</span></span> |
| <span data-ttu-id="9c9d6-120">Outlook [事件][]</span><span class="sxs-lookup"><span data-stu-id="9c9d6-120">Outlook [event][]</span></span> | <span data-ttu-id="9c9d6-121">对用户邮箱中的所有事件更改：</span><span class="sxs-lookup"><span data-stu-id="9c9d6-121">Changes to all events in a user's mailbox:</span></span><br>`/users/{id}/events` | <span data-ttu-id="9c9d6-122">否</span><span class="sxs-lookup"><span data-stu-id="9c9d6-122">No</span></span> |
| <span data-ttu-id="9c9d6-123">Outlook 个人[联系人][]</span><span class="sxs-lookup"><span data-stu-id="9c9d6-123">Outlook personal [contact][]</span></span> | <span data-ttu-id="9c9d6-124">对用户邮箱中的所有个人联系人更改：</span><span class="sxs-lookup"><span data-stu-id="9c9d6-124">Changes to all personal contacts in a user's mailbox:</span></span><br>`/users/{id}/contacts` | <span data-ttu-id="9c9d6-125">否</span><span class="sxs-lookup"><span data-stu-id="9c9d6-125">No</span></span> |
| <span data-ttu-id="9c9d6-126">[用户][]</span><span class="sxs-lookup"><span data-stu-id="9c9d6-126">[user][]</span></span> | <span data-ttu-id="9c9d6-127">对所有用户更改：</span><span class="sxs-lookup"><span data-stu-id="9c9d6-127">Changes to all users:</span></span><br>`/users` <br><span data-ttu-id="9c9d6-128">对特定用户更改：</span><span class="sxs-lookup"><span data-stu-id="9c9d6-128">Changes to a specific user:</span></span><br>`/users/{id}`| <span data-ttu-id="9c9d6-129">否</span><span class="sxs-lookup"><span data-stu-id="9c9d6-129">No</span></span> |
| <span data-ttu-id="9c9d6-130">[组][]</span><span class="sxs-lookup"><span data-stu-id="9c9d6-130">[group][]</span></span> | <span data-ttu-id="9c9d6-131">对所有组更改：</span><span class="sxs-lookup"><span data-stu-id="9c9d6-131">Changes to all groups:</span></span><br>`/groups` <br><span data-ttu-id="9c9d6-132">对特定组更改：</span><span class="sxs-lookup"><span data-stu-id="9c9d6-132">Changes to a specific group:</span></span><br>`/groups/{id}`<br><span data-ttu-id="9c9d6-133">对特定组的所有者所做的更改：</span><span class="sxs-lookup"><span data-stu-id="9c9d6-133">Changes to owners of a specific group:</span></span><br>`/groups/{id}/owners`<br><span data-ttu-id="9c9d6-134">对特定组成员所做的更改：</span><span class="sxs-lookup"><span data-stu-id="9c9d6-134">Changes to members of a specific group:</span></span><br>`/groups/{id}/members` | <span data-ttu-id="9c9d6-135">否</span><span class="sxs-lookup"><span data-stu-id="9c9d6-135">No</span></span> |
| <span data-ttu-id="9c9d6-136">Microsoft 365 组[对话][]</span><span class="sxs-lookup"><span data-stu-id="9c9d6-136">Microsoft 365 group [conversation][]</span></span> | <span data-ttu-id="9c9d6-137">查看组的对话：</span><span class="sxs-lookup"><span data-stu-id="9c9d6-137">Changes to a group's conversations:</span></span><br>`groups/{id}/conversations` | <span data-ttu-id="9c9d6-138">否</span><span class="sxs-lookup"><span data-stu-id="9c9d6-138">No</span></span> |
| <span data-ttu-id="9c9d6-139">OneDrive（个人版）上的 [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="9c9d6-139">[driveItem][] on OneDrive (personal)</span></span> | <span data-ttu-id="9c9d6-140">对_任何文件夹_的层次结构内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="9c9d6-140">Changes to content within the hierarchy of _any folder_:</span></span><br>`/users/{id}/drive/root` | <span data-ttu-id="9c9d6-141">否</span><span class="sxs-lookup"><span data-stu-id="9c9d6-141">No</span></span> |
| <span data-ttu-id="9c9d6-142">OneDrive for Business 上的 [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="9c9d6-142">[driveItem][] on OneDrive for Business</span></span> | <span data-ttu-id="9c9d6-143">对_根文件夹_的层次结构内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="9c9d6-143">Changes to content within the hierarchy of the _root folder_:</span></span><br>`/drives/{id}/root`<br> `/users/{id}/drive/root` | <span data-ttu-id="9c9d6-144">否</span><span class="sxs-lookup"><span data-stu-id="9c9d6-144">No</span></span> |
| <span data-ttu-id="9c9d6-145">SharePoint [网站][]下的[列表][]</span><span class="sxs-lookup"><span data-stu-id="9c9d6-145">[list][] under a SharePoint [site][]</span></span> | `/sites/{id}/lists/{id}` | <span data-ttu-id="9c9d6-146">否</span><span class="sxs-lookup"><span data-stu-id="9c9d6-146">No</span></span> |
| <span data-ttu-id="9c9d6-147">安全[警报][]</span><span class="sxs-lookup"><span data-stu-id="9c9d6-147">Security [alert][]</span></span> | <span data-ttu-id="9c9d6-148">对特定警报更改：</span><span class="sxs-lookup"><span data-stu-id="9c9d6-148">Changes to a specific alert:</span></span><br>`/security/alerts/{id}` <br><span data-ttu-id="9c9d6-149">对已筛选的警报更改：</span><span class="sxs-lookup"><span data-stu-id="9c9d6-149">Changes to filtered alerts:</span></span><br> `/security/alerts/?$filter`| <span data-ttu-id="9c9d6-150">否</span><span class="sxs-lookup"><span data-stu-id="9c9d6-150">No</span></span> |
| <span data-ttu-id="9c9d6-151">Teams [callRecord][]</span><span class="sxs-lookup"><span data-stu-id="9c9d6-151">Teams [callRecord][]</span></span> | <span data-ttu-id="9c9d6-152">更改 _所有_ 呼叫记录： `/communications/callRecords`</span><span class="sxs-lookup"><span data-stu-id="9c9d6-152">Changes to _all_ call records: `/communications/callRecords`</span></span> | <span data-ttu-id="9c9d6-153">否</span><span class="sxs-lookup"><span data-stu-id="9c9d6-153">No</span></span> |
| <span data-ttu-id="9c9d6-154">Teams [chatmessage][]</span><span class="sxs-lookup"><span data-stu-id="9c9d6-154">Teams [chatmessage][]</span></span> | <span data-ttu-id="9c9d6-155">对所有团队中所有频道聊天消息更改：</span><span class="sxs-lookup"><span data-stu-id="9c9d6-155">Changes to chat messages in all channels in all teams:</span></span><br>`/teams/getAllMessages` <br><span data-ttu-id="9c9d6-156">对特定频道中的聊天消息更改：</span><span class="sxs-lookup"><span data-stu-id="9c9d6-156">Changes to chat messages in a specific channel:</span></span><br>`/teams/{id}/channels/{id}/messages`<br><span data-ttu-id="9c9d6-157">对所有聊天的消息更改：</span><span class="sxs-lookup"><span data-stu-id="9c9d6-157">Changes to chat messages in all chats:</span></span><br>`/chats/getAllMessages` <br><span data-ttu-id="9c9d6-158">对特定聊天中的消息更改：</span><span class="sxs-lookup"><span data-stu-id="9c9d6-158">Changes to chat messages in a specific chat:</span></span><br>`/chats/{id}/messages` | <span data-ttu-id="9c9d6-159">是</span><span class="sxs-lookup"><span data-stu-id="9c9d6-159">Yes</span></span> |
| <span data-ttu-id="9c9d6-160">团队 [状态][]</span><span class="sxs-lookup"><span data-stu-id="9c9d6-160">Teams [presence][]</span></span> | <span data-ttu-id="9c9d6-161">对单个用户的状态的更改： `/communications/presences/{id}`</span><span class="sxs-lookup"><span data-stu-id="9c9d6-161">Changes to a single user's presence: `/communications/presences/{id}`</span></span> <br> <span data-ttu-id="9c9d6-162">对多个用户状态的更改：</span><span class="sxs-lookup"><span data-stu-id="9c9d6-162">Changes to multiple user presences:</span></span><br> `/communications/presences?$filter=id in ({id},{id}...)` | <span data-ttu-id="9c9d6-163">是</span><span class="sxs-lookup"><span data-stu-id="9c9d6-163">Yes</span></span> |

> <span data-ttu-id="9c9d6-164">**注意**：以 `/users/{id}` 开头的任何资源路径还可接受 `/me` 以引用已登录的用户。</span><span class="sxs-lookup"><span data-stu-id="9c9d6-164">**Note**: Any resource path that begins with `/users/{id}` can also accept `/me` to reference the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c9d6-165">权限</span><span class="sxs-lookup"><span data-stu-id="9c9d6-165">Permissions</span></span>

<span data-ttu-id="9c9d6-166">通常订阅操作需要拥有对资源的读取权限。</span><span class="sxs-lookup"><span data-stu-id="9c9d6-166">In general, subscription operations require read permission to the resource.</span></span> <span data-ttu-id="9c9d6-167">例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。</span><span class="sxs-lookup"><span data-stu-id="9c9d6-167">For example, to get notifications for messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="9c9d6-168">[创建订阅](../api/subscription-post-subscriptions.md)一文列出了各个资源类型所需的权限。</span><span class="sxs-lookup"><span data-stu-id="9c9d6-168">The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type.</span></span> <span data-ttu-id="9c9d6-169">下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。</span><span class="sxs-lookup"><span data-stu-id="9c9d6-169">The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="9c9d6-170">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c9d6-170">Permission type</span></span>                        | <span data-ttu-id="9c9d6-171">支持的资源类型</span><span class="sxs-lookup"><span data-stu-id="9c9d6-171">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="9c9d6-172">委派 - 工作或学校帐户</span><span class="sxs-lookup"><span data-stu-id="9c9d6-172">Delegated - work or school account</span></span>     | <span data-ttu-id="9c9d6-173">[警报][]、 [联系人][]、 [对话][]、 [driveItem][]、 [list][]、 [event][]、 [group][]、 [message][]、 [user][]、 [出席][]、 [了 chatmessage][] (preview) </span><span class="sxs-lookup"><span data-stu-id="9c9d6-173">[alert][], [contact][], [conversation][], [driveItem][], [list][], [event][], [group][], [message][], [user][], [presence][], [chatMessage][] (preview)</span></span> |
| <span data-ttu-id="9c9d6-174">委派 - 个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="9c9d6-174">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="9c9d6-175">[联系人][]、[driveItem][]、[列表][]、[事件][]、[邮件][]</span><span class="sxs-lookup"><span data-stu-id="9c9d6-175">[contact][], [driveItem][], [list][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="9c9d6-176">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c9d6-176">Application</span></span>                            | <span data-ttu-id="9c9d6-177">[alert][]、 [contact][]、 [driveItem][]、 [list][]、 [event][]、 [group][]、 [message][]、 [user][]、 [callRecord][]、 [了 chatmessage][]</span><span class="sxs-lookup"><span data-stu-id="9c9d6-177">[alert][], [contact][], [driveItem][], [list][], [event][], [group][], [message][], [user][], [callRecord][], [chatMessage][]</span></span>|

## <a name="see-also"></a><span data-ttu-id="9c9d6-178">另请参阅</span><span class="sxs-lookup"><span data-stu-id="9c9d6-178">See also</span></span>

- [<span data-ttu-id="9c9d6-179">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="9c9d6-179">Subscription resource type</span></span>](subscription.md)
- [<span data-ttu-id="9c9d6-180">列出订阅</span><span class="sxs-lookup"><span data-stu-id="9c9d6-180">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="9c9d6-181">获取订阅</span><span class="sxs-lookup"><span data-stu-id="9c9d6-181">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="9c9d6-182">创建订阅</span><span class="sxs-lookup"><span data-stu-id="9c9d6-182">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="9c9d6-183">更新订阅</span><span class="sxs-lookup"><span data-stu-id="9c9d6-183">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="9c9d6-184">删除订阅</span><span class="sxs-lookup"><span data-stu-id="9c9d6-184">Delete subscription</span></span>](../api/subscription-delete.md)

[chatMessage]: ./chatmessage.md
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
[状态]: ./presence.md
[presence]: ./presence.md


