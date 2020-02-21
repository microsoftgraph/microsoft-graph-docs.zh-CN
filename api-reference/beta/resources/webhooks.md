---
title: 使用 Microsoft Graph API 获取更改通知
description: Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。 客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。 客户端应用使用通知在更改时更新其状态。 有关详细信息（包括如何订阅和处理传入通知），请参阅“设置用户数据更改的通知”。
localization_priority: Normal
author: baywet
doc_type: conceptualPageType
ms.prod: ''
ms.openlocfilehash: e14227ad1e64aaea6bf2cfb15f9ba76d0ffeb12b
ms.sourcegitcommit: 31a9b4cb3d0f905f123475a4c1a86f5b1e59b935
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2020
ms.locfileid: "42219648"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="fd429-106">使用 Microsoft Graph API 获取更改通知</span><span class="sxs-lookup"><span data-stu-id="fd429-106">Use the Microsoft Graph API to get change notifications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd429-107">Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。</span><span class="sxs-lookup"><span data-stu-id="fd429-107">The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="fd429-108">客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。</span><span class="sxs-lookup"><span data-stu-id="fd429-108">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="fd429-109">客户端应用使用通知在更改时更新其状态。</span><span class="sxs-lookup"><span data-stu-id="fd429-109">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="fd429-110">有关详细信息（包括如何订阅和处理传入通知），请参阅[设置用户数据更改的通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="fd429-110">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="fd429-111">使用 Microsoft Graph API，应用可以订阅以下资源的更改：</span><span class="sxs-lookup"><span data-stu-id="fd429-111">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

| <span data-ttu-id="fd429-112">**资源**</span><span class="sxs-lookup"><span data-stu-id="fd429-112">**Resource**</span></span> | <span data-ttu-id="fd429-113">**支持的资源路径**</span><span class="sxs-lookup"><span data-stu-id="fd429-113">**Supported resource paths**</span></span> | <span data-ttu-id="fd429-114">**资源数据可以包含在通知中**</span><span class="sxs-lookup"><span data-stu-id="fd429-114">**Resource data can be included in notifications**</span></span>                  |
|:----------------|:------------|:-----------------------------------------|
| <span data-ttu-id="fd429-115">Outlook [邮件][]</span><span class="sxs-lookup"><span data-stu-id="fd429-115">Outlook [message][]</span></span> | <span data-ttu-id="fd429-116">对用户邮箱中的所有邮件所做的更改：</span><span class="sxs-lookup"><span data-stu-id="fd429-116">Changes to all messages in a user's mailbox:</span></span> <br>`/users/{id}/messages`<br><span data-ttu-id="fd429-117">对用户收件箱中的邮件所做的更改：</span><span class="sxs-lookup"><span data-stu-id="fd429-117">Changes to messages in a user's Inbox:</span></span><br>`/users/{id}/mailFolders('inbox')/messages` | <span data-ttu-id="fd429-118">否</span><span class="sxs-lookup"><span data-stu-id="fd429-118">No</span></span> |
| <span data-ttu-id="fd429-119">Outlook [事件][]</span><span class="sxs-lookup"><span data-stu-id="fd429-119">Outlook [event][]</span></span> | <span data-ttu-id="fd429-120">对用户邮箱中的所有事件所做的更改：</span><span class="sxs-lookup"><span data-stu-id="fd429-120">Changes to all events in a user's mailbox:</span></span><br>`/users/{id}/events` | <span data-ttu-id="fd429-121">否</span><span class="sxs-lookup"><span data-stu-id="fd429-121">No</span></span> |
| <span data-ttu-id="fd429-122">Outlook 个人[联系人][]</span><span class="sxs-lookup"><span data-stu-id="fd429-122">Outlook personal [contact][]</span></span> | <span data-ttu-id="fd429-123">对用户邮箱中的所有个人联系人所做的更改：</span><span class="sxs-lookup"><span data-stu-id="fd429-123">Changes to all personal contacts in a user's mailbox:</span></span><br>`/users/{id}/contacts` | <span data-ttu-id="fd429-124">否</span><span class="sxs-lookup"><span data-stu-id="fd429-124">No</span></span> |
| <span data-ttu-id="fd429-125">[用户][]</span><span class="sxs-lookup"><span data-stu-id="fd429-125">[user][]</span></span> | <span data-ttu-id="fd429-126">对所有用户所做的更改：</span><span class="sxs-lookup"><span data-stu-id="fd429-126">Changes to all users:</span></span><br>`/users` <br><span data-ttu-id="fd429-127">对特定用户的更改：</span><span class="sxs-lookup"><span data-stu-id="fd429-127">Changes to a specific user:</span></span><br>`/users/{id}`| <span data-ttu-id="fd429-128">否</span><span class="sxs-lookup"><span data-stu-id="fd429-128">No</span></span> |
| <span data-ttu-id="fd429-129">[组][]</span><span class="sxs-lookup"><span data-stu-id="fd429-129">[group][]</span></span> | <span data-ttu-id="fd429-130">对所有组所做的更改：</span><span class="sxs-lookup"><span data-stu-id="fd429-130">Changes to all groups:</span></span><br>`/groups` <br><span data-ttu-id="fd429-131">对特定组的更改：</span><span class="sxs-lookup"><span data-stu-id="fd429-131">Changes to a specific group:</span></span><br>`/groups/{id}` | <span data-ttu-id="fd429-132">否</span><span class="sxs-lookup"><span data-stu-id="fd429-132">No</span></span> |
| <span data-ttu-id="fd429-133">Office 365 组[对话][]</span><span class="sxs-lookup"><span data-stu-id="fd429-133">Office 365 group [conversation][]</span></span> | <span data-ttu-id="fd429-134">对组的对话所做的更改：</span><span class="sxs-lookup"><span data-stu-id="fd429-134">Changes to a group's conversations:</span></span><br>`groups/{id}/conversations` | <span data-ttu-id="fd429-135">否</span><span class="sxs-lookup"><span data-stu-id="fd429-135">No</span></span> |
| <span data-ttu-id="fd429-136">OneDrive （个人版）上的[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="fd429-136">[driveItem][] on OneDrive (personal)</span></span> | <span data-ttu-id="fd429-137">对_任意文件夹_层次结构中的内容所做的更改：</span><span class="sxs-lookup"><span data-stu-id="fd429-137">Changes to content within the hierarchy of _any folder_:</span></span><br>`/users/{id}/drive/root` | <span data-ttu-id="fd429-138">否</span><span class="sxs-lookup"><span data-stu-id="fd429-138">No</span></span> |
| <span data-ttu-id="fd429-139">OneDrive for Business 上的[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="fd429-139">[driveItem][] on OneDrive for Business</span></span> | <span data-ttu-id="fd429-140">对_根文件夹_层次结构中的内容所做的更改：</span><span class="sxs-lookup"><span data-stu-id="fd429-140">Changes to content within the hierarchy of the _root folder_:</span></span><br>`/drives/{id}/root`<br> `/users/{id}/drive/root` | <span data-ttu-id="fd429-141">否</span><span class="sxs-lookup"><span data-stu-id="fd429-141">No</span></span> |
| <span data-ttu-id="fd429-142">安全[警报][]</span><span class="sxs-lookup"><span data-stu-id="fd429-142">Security [alert][]</span></span> | <span data-ttu-id="fd429-143">对特定警报的更改：</span><span class="sxs-lookup"><span data-stu-id="fd429-143">Changes to a specific alert:</span></span><br>`/security/alerts/{id}` <br><span data-ttu-id="fd429-144">对已筛选警报的更改：</span><span class="sxs-lookup"><span data-stu-id="fd429-144">Changes to filtered alerts:</span></span><br> `/security/alerts/?$filter`| <span data-ttu-id="fd429-145">否</span><span class="sxs-lookup"><span data-stu-id="fd429-145">No</span></span> |
| <span data-ttu-id="fd429-146">团队[了 chatmessage](/graph/api/resources/subscription?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="fd429-146">Teams [chatmessage](/graph/api/resources/subscription?view=graph-rest-beta)</span></span> | <span data-ttu-id="fd429-147">对所有团队中的所有频道中的聊天消息的更改：</span><span class="sxs-lookup"><span data-stu-id="fd429-147">Changes to chat messages in all channels in all teams:</span></span><br>`/teams/allMessages` <br><span data-ttu-id="fd429-148">对特定频道中聊天邮件的更改：</span><span class="sxs-lookup"><span data-stu-id="fd429-148">Changes to chat messages in a specific channel:</span></span><br>`/teams/{id}/channels/{id}/messages`<br><span data-ttu-id="fd429-149">在所有聊天中对聊天消息进行的更改：</span><span class="sxs-lookup"><span data-stu-id="fd429-149">Changes to chat messages in all chats:</span></span><br>`/chats/allMessages` <br><span data-ttu-id="fd429-150">在特定聊天中对聊天消息进行的更改：</span><span class="sxs-lookup"><span data-stu-id="fd429-150">Changes to chat messages in a specific chat:</span></span><br>`/chats/{id}/messages` | <span data-ttu-id="fd429-151">是</span><span class="sxs-lookup"><span data-stu-id="fd429-151">Yes</span></span> |

> <span data-ttu-id="fd429-152">**注意**：开头的`/users/{id}`任何资源路径也都可以接受`/me`引用已登录用户。</span><span class="sxs-lookup"><span data-stu-id="fd429-152">**Note**: Any resource path that begins with `/users/{id}` can also accept `/me` to reference the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd429-153">权限</span><span class="sxs-lookup"><span data-stu-id="fd429-153">Permissions</span></span>

<span data-ttu-id="fd429-154">通常订阅操作需要拥有对资源的读取权限。</span><span class="sxs-lookup"><span data-stu-id="fd429-154">In general, subscription operations require read permission to the resource.</span></span> <span data-ttu-id="fd429-155">例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。</span><span class="sxs-lookup"><span data-stu-id="fd429-155">For example, to get notifications for messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="fd429-156">[创建订阅](../api/subscription-post-subscriptions.md)一文列出了各个资源类型所需的权限。</span><span class="sxs-lookup"><span data-stu-id="fd429-156">The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type.</span></span> <span data-ttu-id="fd429-157">下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。</span><span class="sxs-lookup"><span data-stu-id="fd429-157">The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="fd429-158">权限类型</span><span class="sxs-lookup"><span data-stu-id="fd429-158">Permission type</span></span>                        | <span data-ttu-id="fd429-159">支持的资源类型</span><span class="sxs-lookup"><span data-stu-id="fd429-159">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="fd429-160">委派 - 工作或学校帐户</span><span class="sxs-lookup"><span data-stu-id="fd429-160">Delegated - work or school account</span></span>     | <span data-ttu-id="fd429-161">[警报][]、[联系人][]、[对话][]、[driveItem][]、[事件][]、[组][]、[邮件][]、[用户][]</span><span class="sxs-lookup"><span data-stu-id="fd429-161">[alert][], [contact][], [conversation][], [driveItem][], [event][], [group][], [message][], [user][]</span></span>|
| <span data-ttu-id="fd429-162">委派 - 个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="fd429-162">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="fd429-163">[联系人][]、[driveItem][]、[事件][]、[邮件][]</span><span class="sxs-lookup"><span data-stu-id="fd429-163">[contact][], [driveItem][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="fd429-164">应用程序</span><span class="sxs-lookup"><span data-stu-id="fd429-164">Application</span></span>                            | <span data-ttu-id="fd429-165">[alert][]、 [contact][]、 [driveItem][]、 [event][]、 [group][]、 [message][]、 [user][]、[了 chatmessage][]</span><span class="sxs-lookup"><span data-stu-id="fd429-165">[alert][], [contact][], [driveItem][], [event][], [group][], [message][], [user][], [chatMessage][]</span></span>|

## <a name="see-also"></a><span data-ttu-id="fd429-166">另请参阅</span><span class="sxs-lookup"><span data-stu-id="fd429-166">See also</span></span>

- [<span data-ttu-id="fd429-167">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="fd429-167">Subscription resource type</span></span>](subscription.md)
- [<span data-ttu-id="fd429-168">列出订阅</span><span class="sxs-lookup"><span data-stu-id="fd429-168">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="fd429-169">获取订阅</span><span class="sxs-lookup"><span data-stu-id="fd429-169">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="fd429-170">创建订阅</span><span class="sxs-lookup"><span data-stu-id="fd429-170">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="fd429-171">更新订阅</span><span class="sxs-lookup"><span data-stu-id="fd429-171">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="fd429-172">删除订阅</span><span class="sxs-lookup"><span data-stu-id="fd429-172">Delete subscription</span></span>](../api/subscription-delete.md)

[chatMessage]: ./chatmessage.md
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
