---
title: 使用 Microsoft Graph API 获取更改通知
description: Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。 客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。 客户端应用使用通知在更改时更新其状态。 有关详细信息（包括如何订阅和处理传入通知），请参阅“设置用户数据更改的通知”。
localization_priority: Normal
author: baywet
doc_type: conceptualPageType
ms.prod: ''
ms.openlocfilehash: 739f5821df7eded3757a437fb2909595c4df7692
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331330"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="89d86-106">使用 Microsoft Graph API 获取更改通知</span><span class="sxs-lookup"><span data-stu-id="89d86-106">Use the Microsoft Graph API to get change notifications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89d86-107">Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。</span><span class="sxs-lookup"><span data-stu-id="89d86-107">The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="89d86-108">客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。</span><span class="sxs-lookup"><span data-stu-id="89d86-108">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="89d86-109">客户端应用使用通知在更改时更新其状态。</span><span class="sxs-lookup"><span data-stu-id="89d86-109">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="89d86-110">有关详细信息（包括如何订阅和处理传入通知），请参阅[设置用户数据更改的通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="89d86-110">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="89d86-111">使用 Microsoft Graph API，应用可以订阅以下资源的更改：</span><span class="sxs-lookup"><span data-stu-id="89d86-111">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

| <span data-ttu-id="89d86-112">**资源**</span><span class="sxs-lookup"><span data-stu-id="89d86-112">**Resource**</span></span> | <span data-ttu-id="89d86-113">**支持的资源路径**</span><span class="sxs-lookup"><span data-stu-id="89d86-113">**Supported resource paths**</span></span> | <span data-ttu-id="89d86-114">**可包含在通知中的资源数据**</span><span class="sxs-lookup"><span data-stu-id="89d86-114">**Resource data can be included in notifications**</span></span>                  |
|:----------------|:------------|:-----------------------------------------|
| <span data-ttu-id="89d86-115">Outlook [邮件][]</span><span class="sxs-lookup"><span data-stu-id="89d86-115">Outlook [message][]</span></span> | <span data-ttu-id="89d86-116">对用户邮箱中的所有邮件更改：</span><span class="sxs-lookup"><span data-stu-id="89d86-116">Changes to all messages in a user's mailbox:</span></span> <br>`/users/{id}/messages`<br><span data-ttu-id="89d86-117">对用户收件箱中的所有邮件更改：</span><span class="sxs-lookup"><span data-stu-id="89d86-117">Changes to messages in a user's Inbox:</span></span><br>`/users/{id}/mailFolders('inbox')/messages` | <span data-ttu-id="89d86-118">否</span><span class="sxs-lookup"><span data-stu-id="89d86-118">No</span></span> |
| <span data-ttu-id="89d86-119">Outlook [事件][]</span><span class="sxs-lookup"><span data-stu-id="89d86-119">Outlook [event][]</span></span> | <span data-ttu-id="89d86-120">对用户邮箱中的所有事件更改：</span><span class="sxs-lookup"><span data-stu-id="89d86-120">Changes to all events in a user's mailbox:</span></span><br>`/users/{id}/events` | <span data-ttu-id="89d86-121">否</span><span class="sxs-lookup"><span data-stu-id="89d86-121">No</span></span> |
| <span data-ttu-id="89d86-122">Outlook 个人[联系人][]</span><span class="sxs-lookup"><span data-stu-id="89d86-122">Outlook personal [contact][]</span></span> | <span data-ttu-id="89d86-123">对用户邮箱中的所有个人联系人更改：</span><span class="sxs-lookup"><span data-stu-id="89d86-123">Changes to all personal contacts in a user's mailbox:</span></span><br>`/users/{id}/contacts` | <span data-ttu-id="89d86-124">否</span><span class="sxs-lookup"><span data-stu-id="89d86-124">No</span></span> |
| <span data-ttu-id="89d86-125">[用户][]</span><span class="sxs-lookup"><span data-stu-id="89d86-125">[user][]</span></span> | <span data-ttu-id="89d86-126">对所有用户更改：</span><span class="sxs-lookup"><span data-stu-id="89d86-126">Changes to all users:</span></span><br>`/users` <br><span data-ttu-id="89d86-127">对特定用户更改：</span><span class="sxs-lookup"><span data-stu-id="89d86-127">Changes to a specific user:</span></span><br>`/users/{id}`| <span data-ttu-id="89d86-128">否</span><span class="sxs-lookup"><span data-stu-id="89d86-128">No</span></span> |
| <span data-ttu-id="89d86-129">[组][]</span><span class="sxs-lookup"><span data-stu-id="89d86-129">[group][]</span></span> | <span data-ttu-id="89d86-130">对所有组更改：</span><span class="sxs-lookup"><span data-stu-id="89d86-130">Changes to all groups:</span></span><br>`/groups` <br><span data-ttu-id="89d86-131">对特定组更改：</span><span class="sxs-lookup"><span data-stu-id="89d86-131">Changes to a specific group:</span></span><br>`/groups/{id}` | <span data-ttu-id="89d86-132">否</span><span class="sxs-lookup"><span data-stu-id="89d86-132">No</span></span> |
| <span data-ttu-id="89d86-133">Office 365 组[对话][]</span><span class="sxs-lookup"><span data-stu-id="89d86-133">Office 365 group [conversation][]</span></span> | <span data-ttu-id="89d86-134">查看组的对话：</span><span class="sxs-lookup"><span data-stu-id="89d86-134">Changes to a group's conversations:</span></span><br>`groups/{id}/conversations` | <span data-ttu-id="89d86-135">否</span><span class="sxs-lookup"><span data-stu-id="89d86-135">No</span></span> |
| <span data-ttu-id="89d86-136">OneDrive（个人版）上的 [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="89d86-136">[driveItem][] on OneDrive (personal)</span></span> | <span data-ttu-id="89d86-137">对_任何文件夹_的层次结构内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="89d86-137">Changes to content within the hierarchy of _any folder_:</span></span><br>`/users/{id}/drive/root` | <span data-ttu-id="89d86-138">否</span><span class="sxs-lookup"><span data-stu-id="89d86-138">No</span></span> |
| <span data-ttu-id="89d86-139">OneDrive for Business 上的 [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="89d86-139">[driveItem][] on OneDrive for Business</span></span> | <span data-ttu-id="89d86-140">对_根文件夹_的层次结构内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="89d86-140">Changes to content within the hierarchy of the _root folder_:</span></span><br>`/drives/{id}/root`<br> `/users/{id}/drive/root` | <span data-ttu-id="89d86-141">否</span><span class="sxs-lookup"><span data-stu-id="89d86-141">No</span></span> |
| <span data-ttu-id="89d86-142">SharePoint[网站][]下的[列表][]</span><span class="sxs-lookup"><span data-stu-id="89d86-142">[list][] under a SharePoint [site][]</span></span> | `/sites/{id}/lists/{id}` | <span data-ttu-id="89d86-143">否</span><span class="sxs-lookup"><span data-stu-id="89d86-143">No</span></span> |
| <span data-ttu-id="89d86-144">安全[警报][]</span><span class="sxs-lookup"><span data-stu-id="89d86-144">Security [alert][]</span></span> | <span data-ttu-id="89d86-145">对特定警报更改：</span><span class="sxs-lookup"><span data-stu-id="89d86-145">Changes to a specific alert:</span></span><br>`/security/alerts/{id}` <br><span data-ttu-id="89d86-146">对已筛选的警报更改：</span><span class="sxs-lookup"><span data-stu-id="89d86-146">Changes to filtered alerts:</span></span><br> `/security/alerts/?$filter`| <span data-ttu-id="89d86-147">否</span><span class="sxs-lookup"><span data-stu-id="89d86-147">No</span></span> |
| <span data-ttu-id="89d86-148">Teams [chatmessage](/graph/api/resources/subscription?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="89d86-148">Teams [chatmessage](/graph/api/resources/subscription?view=graph-rest-beta)</span></span> | <span data-ttu-id="89d86-149">对所有团队中所有频道聊天消息更改：</span><span class="sxs-lookup"><span data-stu-id="89d86-149">Changes to chat messages in all channels in all teams:</span></span><br>`/teams/allMessages` <br><span data-ttu-id="89d86-150">对特定频道中的聊天消息更改：</span><span class="sxs-lookup"><span data-stu-id="89d86-150">Changes to chat messages in a specific channel:</span></span><br>`/teams/{id}/channels/{id}/messages`<br><span data-ttu-id="89d86-151">对所有聊天的消息更改：</span><span class="sxs-lookup"><span data-stu-id="89d86-151">Changes to chat messages in all chats:</span></span><br>`/chats/allMessages` <br><span data-ttu-id="89d86-152">对特定聊天中的消息更改：</span><span class="sxs-lookup"><span data-stu-id="89d86-152">Changes to chat messages in a specific chat:</span></span><br>`/chats/{id}/messages` | <span data-ttu-id="89d86-153">是</span><span class="sxs-lookup"><span data-stu-id="89d86-153">Yes</span></span> |

> <span data-ttu-id="89d86-154">**注意**：以 `/users/{id}` 开头的任何资源路径还可接受 `/me` 以引用已登录的用户。</span><span class="sxs-lookup"><span data-stu-id="89d86-154">**Note**: Any resource path that begins with `/users/{id}` can also accept `/me` to reference the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="89d86-155">权限</span><span class="sxs-lookup"><span data-stu-id="89d86-155">Permissions</span></span>

<span data-ttu-id="89d86-156">通常订阅操作需要拥有对资源的读取权限。</span><span class="sxs-lookup"><span data-stu-id="89d86-156">In general, subscription operations require read permission to the resource.</span></span> <span data-ttu-id="89d86-157">例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。</span><span class="sxs-lookup"><span data-stu-id="89d86-157">For example, to get notifications for messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="89d86-158">[创建订阅](../api/subscription-post-subscriptions.md)一文列出了各个资源类型所需的权限。</span><span class="sxs-lookup"><span data-stu-id="89d86-158">The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type.</span></span> <span data-ttu-id="89d86-159">下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。</span><span class="sxs-lookup"><span data-stu-id="89d86-159">The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="89d86-160">权限类型</span><span class="sxs-lookup"><span data-stu-id="89d86-160">Permission type</span></span>                        | <span data-ttu-id="89d86-161">支持的资源类型</span><span class="sxs-lookup"><span data-stu-id="89d86-161">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="89d86-162">委派 - 工作或学校帐户</span><span class="sxs-lookup"><span data-stu-id="89d86-162">Delegated - work or school account</span></span>     | <span data-ttu-id="89d86-163">[警报][]、[联系人][]、[对话][]、 [driveItem][]、 [list][]、 [event][]、 [group][]、 [message][]、 [user][]</span><span class="sxs-lookup"><span data-stu-id="89d86-163">[alert][], [contact][], [conversation][], [driveItem][], [list][], [event][], [group][], [message][], [user][]</span></span>|
| <span data-ttu-id="89d86-164">委派 - 个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="89d86-164">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="89d86-165">[contact][]、 [driveItem][]、 [list][]、 [event][]、 [message][]</span><span class="sxs-lookup"><span data-stu-id="89d86-165">[contact][], [driveItem][], [list][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="89d86-166">应用程序</span><span class="sxs-lookup"><span data-stu-id="89d86-166">Application</span></span>                            | <span data-ttu-id="89d86-167">[alert][]、 [contact][]、 [driveItem][]、 [list][]、 [event][]、 [group][]、 [message][]、 [user][]、[了 chatmessage][]</span><span class="sxs-lookup"><span data-stu-id="89d86-167">[alert][], [contact][], [driveItem][], [list][], [event][], [group][], [message][], [user][], [chatMessage][]</span></span>|

## <a name="see-also"></a><span data-ttu-id="89d86-168">另请参阅</span><span class="sxs-lookup"><span data-stu-id="89d86-168">See also</span></span>

- [<span data-ttu-id="89d86-169">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="89d86-169">Subscription resource type</span></span>](subscription.md)
- [<span data-ttu-id="89d86-170">列出订阅</span><span class="sxs-lookup"><span data-stu-id="89d86-170">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="89d86-171">获取订阅</span><span class="sxs-lookup"><span data-stu-id="89d86-171">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="89d86-172">创建订阅</span><span class="sxs-lookup"><span data-stu-id="89d86-172">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="89d86-173">更新订阅</span><span class="sxs-lookup"><span data-stu-id="89d86-173">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="89d86-174">删除订阅</span><span class="sxs-lookup"><span data-stu-id="89d86-174">Delete subscription</span></span>](../api/subscription-delete.md)

[chatMessage]: ./chatmessage.md
[联系人]: ./contact.md
[contact]: ./contact.md
[对话]: ./conversation.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[list]: ./list.md
[网站]: ./site.md
[site]: ./site.md
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
