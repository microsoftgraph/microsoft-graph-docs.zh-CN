---
title: 使用 Microsoft Graph API 获取更改通知
description: Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。 客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。 客户端应用使用通知在更改时更新其状态。 有关详细信息（包括如何订阅和处理传入通知），请参阅“设置用户数据更改的通知”。
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: b825101cc3b32ea3ab562bd317c7dc511cc00079
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533401"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="1b00a-106">使用 Microsoft Graph API 获取更改通知</span><span class="sxs-lookup"><span data-stu-id="1b00a-106">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="1b00a-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b00a-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1b00a-108">Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。</span><span class="sxs-lookup"><span data-stu-id="1b00a-108">The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="1b00a-109">客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。</span><span class="sxs-lookup"><span data-stu-id="1b00a-109">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="1b00a-110">客户端应用使用通知在更改时更新其状态。</span><span class="sxs-lookup"><span data-stu-id="1b00a-110">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="1b00a-111">有关详细信息（包括如何订阅和处理传入通知），请参阅[设置用户数据更改的通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="1b00a-111">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="1b00a-112">使用 Microsoft Graph API，应用可以订阅以下资源的更改：</span><span class="sxs-lookup"><span data-stu-id="1b00a-112">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

| <span data-ttu-id="1b00a-113">**资源**</span><span class="sxs-lookup"><span data-stu-id="1b00a-113">**Resource**</span></span> | <span data-ttu-id="1b00a-114">**支持的资源路径**</span><span class="sxs-lookup"><span data-stu-id="1b00a-114">**Supported resource paths**</span></span> | <span data-ttu-id="1b00a-115">**可包含在通知中的资源数据**</span><span class="sxs-lookup"><span data-stu-id="1b00a-115">**Resource data can be included in notifications**</span></span>                  |
|:----------------|:------------|:-----------------------------------------|
| <span data-ttu-id="1b00a-116">Outlook [邮件][]</span><span class="sxs-lookup"><span data-stu-id="1b00a-116">Outlook [message][]</span></span> | <span data-ttu-id="1b00a-117">对用户邮箱中的所有邮件更改：</span><span class="sxs-lookup"><span data-stu-id="1b00a-117">Changes to all messages in a user's mailbox:</span></span> <br>`/users/{id}/messages`<br><span data-ttu-id="1b00a-118">对用户收件箱中的所有邮件更改：</span><span class="sxs-lookup"><span data-stu-id="1b00a-118">Changes to messages in a user's Inbox:</span></span><br>`/users/{id}/mailFolders('inbox')/messages` | <span data-ttu-id="1b00a-119">否</span><span class="sxs-lookup"><span data-stu-id="1b00a-119">No</span></span> |
| <span data-ttu-id="1b00a-120">Outlook [事件][]</span><span class="sxs-lookup"><span data-stu-id="1b00a-120">Outlook [event][]</span></span> | <span data-ttu-id="1b00a-121">对用户邮箱中的所有事件更改：</span><span class="sxs-lookup"><span data-stu-id="1b00a-121">Changes to all events in a user's mailbox:</span></span><br>`/users/{id}/events` | <span data-ttu-id="1b00a-122">否</span><span class="sxs-lookup"><span data-stu-id="1b00a-122">No</span></span> |
| <span data-ttu-id="1b00a-123">Outlook 个人[联系人][]</span><span class="sxs-lookup"><span data-stu-id="1b00a-123">Outlook personal [contact][]</span></span> | <span data-ttu-id="1b00a-124">对用户邮箱中的所有个人联系人更改：</span><span class="sxs-lookup"><span data-stu-id="1b00a-124">Changes to all personal contacts in a user's mailbox:</span></span><br>`/users/{id}/contacts` | <span data-ttu-id="1b00a-125">否</span><span class="sxs-lookup"><span data-stu-id="1b00a-125">No</span></span> |
| <span data-ttu-id="1b00a-126">[用户][]</span><span class="sxs-lookup"><span data-stu-id="1b00a-126">[user][]</span></span> | <span data-ttu-id="1b00a-127">对所有用户更改：</span><span class="sxs-lookup"><span data-stu-id="1b00a-127">Changes to all users:</span></span><br>`/users` <br><span data-ttu-id="1b00a-128">对特定用户更改：</span><span class="sxs-lookup"><span data-stu-id="1b00a-128">Changes to a specific user:</span></span><br>`/users/{id}`| <span data-ttu-id="1b00a-129">否</span><span class="sxs-lookup"><span data-stu-id="1b00a-129">No</span></span> |
| <span data-ttu-id="1b00a-130">[组][]</span><span class="sxs-lookup"><span data-stu-id="1b00a-130">[group][]</span></span> | <span data-ttu-id="1b00a-131">对所有组更改：</span><span class="sxs-lookup"><span data-stu-id="1b00a-131">Changes to all groups:</span></span><br>`/groups` <br><span data-ttu-id="1b00a-132">对特定组更改：</span><span class="sxs-lookup"><span data-stu-id="1b00a-132">Changes to a specific group:</span></span><br>`/groups/{id}` | <span data-ttu-id="1b00a-133">否</span><span class="sxs-lookup"><span data-stu-id="1b00a-133">No</span></span> |
| <span data-ttu-id="1b00a-134">Office 365 组[对话][]</span><span class="sxs-lookup"><span data-stu-id="1b00a-134">Office 365 group [conversation][]</span></span> | <span data-ttu-id="1b00a-135">查看组的对话：</span><span class="sxs-lookup"><span data-stu-id="1b00a-135">Changes to a group's conversations:</span></span><br>`groups/{id}/conversations` | <span data-ttu-id="1b00a-136">否</span><span class="sxs-lookup"><span data-stu-id="1b00a-136">No</span></span> |
| <span data-ttu-id="1b00a-137">OneDrive（个人版）上的 [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="1b00a-137">[driveItem][] on OneDrive (personal)</span></span> | <span data-ttu-id="1b00a-138">对_任何文件夹_的层次结构内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="1b00a-138">Changes to content within the hierarchy of _any folder_:</span></span><br>`/users/{id}/drive/root` | <span data-ttu-id="1b00a-139">否</span><span class="sxs-lookup"><span data-stu-id="1b00a-139">No</span></span> |
| <span data-ttu-id="1b00a-140">OneDrive for Business 上的 [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="1b00a-140">[driveItem][] on OneDrive for Business</span></span> | <span data-ttu-id="1b00a-141">对_根文件夹_的层次结构内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="1b00a-141">Changes to content within the hierarchy of the _root folder_:</span></span><br>`/drives/{id}/root`<br> `/users/{id}/drive/root` | <span data-ttu-id="1b00a-142">否</span><span class="sxs-lookup"><span data-stu-id="1b00a-142">No</span></span> |
| <span data-ttu-id="1b00a-143">安全[警报][]</span><span class="sxs-lookup"><span data-stu-id="1b00a-143">Security [alert][]</span></span> | <span data-ttu-id="1b00a-144">对特定警报更改：</span><span class="sxs-lookup"><span data-stu-id="1b00a-144">Changes to a specific alert:</span></span><br>`/security/alerts/{id}` <br><span data-ttu-id="1b00a-145">对已筛选的警报更改：</span><span class="sxs-lookup"><span data-stu-id="1b00a-145">Changes to filtered alerts:</span></span><br> `/security/alerts/?$filter`| <span data-ttu-id="1b00a-146">否</span><span class="sxs-lookup"><span data-stu-id="1b00a-146">No</span></span> |
| <span data-ttu-id="1b00a-147">Teams [chatmessage](/graph/api/resources/subscription?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="1b00a-147">Teams [chatmessage](/graph/api/resources/subscription?view=graph-rest-beta)</span></span> | <span data-ttu-id="1b00a-148">对所有团队中所有频道聊天消息更改：</span><span class="sxs-lookup"><span data-stu-id="1b00a-148">Changes to chat messages in all channels in all teams:</span></span><br>`/teams/allMessages` <br><span data-ttu-id="1b00a-149">对特定频道中的聊天消息更改：</span><span class="sxs-lookup"><span data-stu-id="1b00a-149">Changes to chat messages in a specific channel:</span></span><br>`/teams/{id}/channels/{id}/messages`<br><span data-ttu-id="1b00a-150">对所有聊天的消息更改：</span><span class="sxs-lookup"><span data-stu-id="1b00a-150">Changes to chat messages in all chats:</span></span><br>`/chats/allMessages` <br><span data-ttu-id="1b00a-151">对特定聊天中的消息更改：</span><span class="sxs-lookup"><span data-stu-id="1b00a-151">Changes to chat messages in a specific chat:</span></span><br>`/chats/{id}/messages` | <span data-ttu-id="1b00a-152">是</span><span class="sxs-lookup"><span data-stu-id="1b00a-152">Yes</span></span> |

> <span data-ttu-id="1b00a-153">**注意**：以 `/users/{id}` 开头的任何资源路径还可接受 `/me` 以引用已登录的用户。</span><span class="sxs-lookup"><span data-stu-id="1b00a-153">**Note**: Any resource path that begins with `/users/{id}` can also accept `/me` to reference the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b00a-154">权限</span><span class="sxs-lookup"><span data-stu-id="1b00a-154">Permissions</span></span>

<span data-ttu-id="1b00a-155">通常订阅操作需要拥有对资源的读取权限。</span><span class="sxs-lookup"><span data-stu-id="1b00a-155">In general, subscription operations require read permission to the resource.</span></span> <span data-ttu-id="1b00a-156">例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。</span><span class="sxs-lookup"><span data-stu-id="1b00a-156">For example, to get notifications for messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="1b00a-157">[创建订阅](../api/subscription-post-subscriptions.md)一文列出了各个资源类型所需的权限。</span><span class="sxs-lookup"><span data-stu-id="1b00a-157">The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type.</span></span> <span data-ttu-id="1b00a-158">下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。</span><span class="sxs-lookup"><span data-stu-id="1b00a-158">The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="1b00a-159">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b00a-159">Permission type</span></span>                        | <span data-ttu-id="1b00a-160">支持的资源类型</span><span class="sxs-lookup"><span data-stu-id="1b00a-160">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="1b00a-161">委派 - 工作或学校帐户</span><span class="sxs-lookup"><span data-stu-id="1b00a-161">Delegated - work or school account</span></span>     | <span data-ttu-id="1b00a-162">[警报][]、[联系人][]、[对话][]、[driveItem][]、[事件][]、[组][]、[邮件][]、[用户][]</span><span class="sxs-lookup"><span data-stu-id="1b00a-162">[alert][], [contact][], [conversation][], [driveItem][], [event][], [group][], [message][], [user][]</span></span>|
| <span data-ttu-id="1b00a-163">委派 - 个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="1b00a-163">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="1b00a-164">[联系人][]、[driveItem][]、[事件][]、[邮件][]</span><span class="sxs-lookup"><span data-stu-id="1b00a-164">[contact][], [driveItem][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="1b00a-165">应用程序</span><span class="sxs-lookup"><span data-stu-id="1b00a-165">Application</span></span>                            | <span data-ttu-id="1b00a-166">[警报][]、[联系人][]、[driveItem][]、[事件][]、[组][]、[邮件][]、[用户][]</span><span class="sxs-lookup"><span data-stu-id="1b00a-166">[alert][], [contact][], [driveItem][], [event][], [group][], [message][], [user][]</span></span>|


## <a name="see-also"></a><span data-ttu-id="1b00a-167">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1b00a-167">See also</span></span>

- [<span data-ttu-id="1b00a-168">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="1b00a-168">Subscription resource type</span></span>](./subscription.md)
- [<span data-ttu-id="1b00a-169">列出订阅</span><span class="sxs-lookup"><span data-stu-id="1b00a-169">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="1b00a-170">获取订阅</span><span class="sxs-lookup"><span data-stu-id="1b00a-170">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="1b00a-171">创建订阅</span><span class="sxs-lookup"><span data-stu-id="1b00a-171">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="1b00a-172">更新订阅</span><span class="sxs-lookup"><span data-stu-id="1b00a-172">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="1b00a-173">删除订阅</span><span class="sxs-lookup"><span data-stu-id="1b00a-173">Delete subscription</span></span>](../api/subscription-delete.md)

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
