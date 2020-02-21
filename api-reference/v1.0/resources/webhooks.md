---
title: 使用 Microsoft Graph API 获取更改通知
description: Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。 客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。 客户端应用使用通知在更改时更新其状态。 有关详细信息（包括如何订阅和处理传入通知），请参阅“设置用户数据更改的通知”。
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: aadd1cb451a5da1c8d546ce140bd8129ca9c2bf8
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162510"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="5b359-106">使用 Microsoft Graph API 获取更改通知</span><span class="sxs-lookup"><span data-stu-id="5b359-106">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="5b359-107">Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。</span><span class="sxs-lookup"><span data-stu-id="5b359-107">The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="5b359-108">客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。</span><span class="sxs-lookup"><span data-stu-id="5b359-108">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="5b359-109">客户端应用使用通知在更改时更新其状态。</span><span class="sxs-lookup"><span data-stu-id="5b359-109">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="5b359-110">有关详细信息（包括如何订阅和处理传入通知），请参阅[设置用户数据更改的通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="5b359-110">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="5b359-111">使用 Microsoft Graph API，应用可以订阅以下资源的更改：</span><span class="sxs-lookup"><span data-stu-id="5b359-111">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

| <span data-ttu-id="5b359-112">**资源**</span><span class="sxs-lookup"><span data-stu-id="5b359-112">**Resource**</span></span> | <span data-ttu-id="5b359-113">**支持的资源路径**</span><span class="sxs-lookup"><span data-stu-id="5b359-113">**Supported resource paths**</span></span> | <span data-ttu-id="5b359-114">**可包含在通知中的资源数据**</span><span class="sxs-lookup"><span data-stu-id="5b359-114">**Resource data can be included in notifications**</span></span>                  |
|:----------------|:------------|:-----------------------------------------|
| <span data-ttu-id="5b359-115">Outlook [邮件][]</span><span class="sxs-lookup"><span data-stu-id="5b359-115">Outlook [message][]</span></span> | `/users/{id}/messages`<br>`/users/{id}/mailFolders('inbox')/messages` | <span data-ttu-id="5b359-116">否</span><span class="sxs-lookup"><span data-stu-id="5b359-116">No</span></span> |
| <span data-ttu-id="5b359-117">Outlook [事件][]</span><span class="sxs-lookup"><span data-stu-id="5b359-117">Outlook [event][]</span></span> | `/users/{id}/events` | <span data-ttu-id="5b359-118">否</span><span class="sxs-lookup"><span data-stu-id="5b359-118">No</span></span> |
| <span data-ttu-id="5b359-119">Outlook 个人[联系人][]</span><span class="sxs-lookup"><span data-stu-id="5b359-119">Outlook personal [contact][]</span></span> | `/users/{id}/contacts` | <span data-ttu-id="5b359-120">否</span><span class="sxs-lookup"><span data-stu-id="5b359-120">No</span></span> |
| <span data-ttu-id="5b359-121">[用户][]</span><span class="sxs-lookup"><span data-stu-id="5b359-121">[user][]</span></span> | <span data-ttu-id="5b359-122">`/users`（对所有用户更改）</span><span class="sxs-lookup"><span data-stu-id="5b359-122">`/users` (changes to all users)</span></span><br><span data-ttu-id="5b359-123">`/users/{id}`（对特定用户更改）</span><span class="sxs-lookup"><span data-stu-id="5b359-123">`/users/{id}` (changes to a specific user)</span></span> | <span data-ttu-id="5b359-124">否</span><span class="sxs-lookup"><span data-stu-id="5b359-124">No</span></span> |
| <span data-ttu-id="5b359-125">[组][]</span><span class="sxs-lookup"><span data-stu-id="5b359-125">[group][]</span></span> | <span data-ttu-id="5b359-126">`/groups`（对所有组更改）</span><span class="sxs-lookup"><span data-stu-id="5b359-126">`/groups` (changes to all groups)</span></span><br><span data-ttu-id="5b359-127">`/groups/{id}`（对特定组更改）</span><span class="sxs-lookup"><span data-stu-id="5b359-127">`/groups/{id}` (changes to a specific group)</span></span> | <span data-ttu-id="5b359-128">否</span><span class="sxs-lookup"><span data-stu-id="5b359-128">No</span></span> |
| <span data-ttu-id="5b359-129">Office 365 组[对话][]</span><span class="sxs-lookup"><span data-stu-id="5b359-129">Office 365 group [conversation][]</span></span> | `groups/{id}/conversations` | <span data-ttu-id="5b359-130">否</span><span class="sxs-lookup"><span data-stu-id="5b359-130">No</span></span> |
| <span data-ttu-id="5b359-131">用户个人 OneDrive 上_任何_ [driveItem][] 文件夹层次结构内的内容</span><span class="sxs-lookup"><span data-stu-id="5b359-131">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span> | `/me/drive/root` | <span data-ttu-id="5b359-132">否</span><span class="sxs-lookup"><span data-stu-id="5b359-132">No</span></span> |
| <span data-ttu-id="5b359-133">OneDrive for Business 上 [driveItem][] _根文件夹_层次结构内的内容</span><span class="sxs-lookup"><span data-stu-id="5b359-133">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span> | `/drives/{id}/root`<br> `/me/drive/root` | <span data-ttu-id="5b359-134">否</span><span class="sxs-lookup"><span data-stu-id="5b359-134">No</span></span> |
| <span data-ttu-id="5b359-135">安全[警报][]</span><span class="sxs-lookup"><span data-stu-id="5b359-135">Security [alert][]</span></span> | <span data-ttu-id="5b359-136">`/security/alerts/{id}`（对特定警报更改）</span><span class="sxs-lookup"><span data-stu-id="5b359-136">`/security/alerts/{id}` (changes to a specific alert)</span></span> <br> <span data-ttu-id="5b359-137">`/security/alerts/?$filter`（对已筛选的警报更改）</span><span class="sxs-lookup"><span data-stu-id="5b359-137">`/security/alerts/?$filter` (changes to filtered alerts)</span></span> | <span data-ttu-id="5b359-138">否</span><span class="sxs-lookup"><span data-stu-id="5b359-138">No</span></span> |
| <span data-ttu-id="5b359-139">Teams [chatmessage](/graph/api/resources/subscription?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="5b359-139">Teams [chatmessage](/graph/api/resources/subscription?view=graph-rest-beta)</span></span> | <span data-ttu-id="5b359-140">`/teams/allMessages`（所有团队中所有渠道中的消息）</span><span class="sxs-lookup"><span data-stu-id="5b359-140">`/teams/allMessages` (messages in all channels in all teams)</span></span><br><span data-ttu-id="5b359-141">`/teams/{id}/channels/{id}/messages`（特定频道中的消息）</span><span class="sxs-lookup"><span data-stu-id="5b359-141">`/teams/{id}/channels/{id}/messages` (messages in a specific channel)</span></span><br><span data-ttu-id="5b359-142">`/chats/allMessages`（所有聊天中的消息）</span><span class="sxs-lookup"><span data-stu-id="5b359-142">`/chats/allMessages` (messages in all chats)</span></span><br><span data-ttu-id="5b359-143">`/chats/{id}/messages`（特定聊天中的消息）</span><span class="sxs-lookup"><span data-stu-id="5b359-143">`/chats/{id}/messages` (messages in a specific chat)</span></span> | <span data-ttu-id="5b359-144">是</span><span class="sxs-lookup"><span data-stu-id="5b359-144">Yes</span></span> |

> <span data-ttu-id="5b359-145">**注意**：以 `/users/{id}` 开头的任何资源路径还可接受 `/me` 以引用已登录的用户。</span><span class="sxs-lookup"><span data-stu-id="5b359-145">**Note**: Any resource path that begins with `/users/{id}` can also accept `/me` to reference the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b359-146">权限</span><span class="sxs-lookup"><span data-stu-id="5b359-146">Permissions</span></span>

<span data-ttu-id="5b359-147">通常订阅操作需要拥有对资源的读取权限。</span><span class="sxs-lookup"><span data-stu-id="5b359-147">In general, subscription operations require read permission to the resource.</span></span> <span data-ttu-id="5b359-148">例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。</span><span class="sxs-lookup"><span data-stu-id="5b359-148">For example, to get notifications for messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="5b359-149">[创建订阅](../api/subscription-post-subscriptions.md)一文列出了各个资源类型所需的权限。</span><span class="sxs-lookup"><span data-stu-id="5b359-149">The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type.</span></span> <span data-ttu-id="5b359-150">下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。</span><span class="sxs-lookup"><span data-stu-id="5b359-150">The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="5b359-151">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b359-151">Permission type</span></span>                        | <span data-ttu-id="5b359-152">支持的资源类型</span><span class="sxs-lookup"><span data-stu-id="5b359-152">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="5b359-153">委派 - 工作或学校帐户</span><span class="sxs-lookup"><span data-stu-id="5b359-153">Delegated - work or school account</span></span>     | <span data-ttu-id="5b359-154">[警报][]、[联系人][]、[对话][]、[driveItem][]、[事件][]、[组][]、[邮件][]、[用户][]</span><span class="sxs-lookup"><span data-stu-id="5b359-154">[alert][], [contact][], [conversation][], [driveItem][], [event][], [group][], [message][], [user][]</span></span>|
| <span data-ttu-id="5b359-155">委派 - 个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="5b359-155">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="5b359-156">[联系人][]、[driveItem][]、[事件][]、[邮件][]</span><span class="sxs-lookup"><span data-stu-id="5b359-156">[contact][], [driveItem][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="5b359-157">应用程序</span><span class="sxs-lookup"><span data-stu-id="5b359-157">Application</span></span>                            | <span data-ttu-id="5b359-158">[警报][]、[联系人][]、[driveItem][]、[事件][]、[组][]、[邮件][]、[用户][]</span><span class="sxs-lookup"><span data-stu-id="5b359-158">[alert][], [contact][], [driveItem][], [event][], [group][], [message][], [user][]</span></span>|


## <a name="see-also"></a><span data-ttu-id="5b359-159">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5b359-159">See also</span></span>

- [<span data-ttu-id="5b359-160">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="5b359-160">Subscription resource type</span></span>](./subscription.md)
- [<span data-ttu-id="5b359-161">列出订阅</span><span class="sxs-lookup"><span data-stu-id="5b359-161">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="5b359-162">获取订阅</span><span class="sxs-lookup"><span data-stu-id="5b359-162">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="5b359-163">创建订阅</span><span class="sxs-lookup"><span data-stu-id="5b359-163">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="5b359-164">更新订阅</span><span class="sxs-lookup"><span data-stu-id="5b359-164">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="5b359-165">删除订阅</span><span class="sxs-lookup"><span data-stu-id="5b359-165">Delete subscription</span></span>](../api/subscription-delete.md)

[联系人]: ./contact.md
[contact]: ./contact.md
[对话]: ./conversation.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[事件]: ./event.md
[event]: ./event.md
[组]: ./group.md
[group]: ./group.md
[邮件]: ./message.md
[message]: ./message.md
[用户]: ./user.md
[user]: ./user.md
[警报]: ./alert.md
[alert]: ./alert.md
