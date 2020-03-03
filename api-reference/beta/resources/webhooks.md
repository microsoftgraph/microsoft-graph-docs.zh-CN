---
title: 使用 Microsoft Graph API 获取更改通知
description: Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。 客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。 客户端应用使用通知在更改时更新其状态。 有关详细信息（包括如何订阅和处理传入通知），请参阅“设置用户数据更改的通知”。
localization_priority: Normal
author: baywet
doc_type: conceptualPageType
ms.prod: ''
ms.openlocfilehash: af08e7a405492a8a7ac02b9889a881190a5689af
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394433"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="feb09-106">使用 Microsoft Graph API 获取更改通知</span><span class="sxs-lookup"><span data-stu-id="feb09-106">Use the Microsoft Graph API to get change notifications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="feb09-107">Microsoft Graph REST API 使用 Webhook 机制将更改通知传递到客户端。</span><span class="sxs-lookup"><span data-stu-id="feb09-107">The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="feb09-108">客户端是一个 Web 服务，用于配置自身的 URL 以接收通知。</span><span class="sxs-lookup"><span data-stu-id="feb09-108">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="feb09-109">客户端应用使用通知在更改时更新其状态。</span><span class="sxs-lookup"><span data-stu-id="feb09-109">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="feb09-110">有关详细信息（包括如何订阅和处理传入通知），请参阅[设置用户数据更改的通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="feb09-110">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="feb09-111">使用 Microsoft Graph API，应用可以订阅以下资源的更改：</span><span class="sxs-lookup"><span data-stu-id="feb09-111">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

| <span data-ttu-id="feb09-112">**资源**</span><span class="sxs-lookup"><span data-stu-id="feb09-112">**Resource**</span></span> | <span data-ttu-id="feb09-113">**支持的资源路径**</span><span class="sxs-lookup"><span data-stu-id="feb09-113">**Supported resource paths**</span></span> | <span data-ttu-id="feb09-114">**可包含在通知中的资源数据**</span><span class="sxs-lookup"><span data-stu-id="feb09-114">**Resource data can be included in notifications**</span></span>                  |
|:----------------|:------------|:-----------------------------------------|
| <span data-ttu-id="feb09-115">Outlook [邮件][]</span><span class="sxs-lookup"><span data-stu-id="feb09-115">Outlook [message][]</span></span> | <span data-ttu-id="feb09-116">对用户邮箱中的所有邮件更改：</span><span class="sxs-lookup"><span data-stu-id="feb09-116">Changes to all messages in a user's mailbox:</span></span> <br>`/users/{id}/messages`<br><span data-ttu-id="feb09-117">对用户收件箱中的所有邮件更改：</span><span class="sxs-lookup"><span data-stu-id="feb09-117">Changes to messages in a user's Inbox:</span></span><br>`/users/{id}/mailFolders('inbox')/messages` | <span data-ttu-id="feb09-118">否</span><span class="sxs-lookup"><span data-stu-id="feb09-118">No</span></span> |
| <span data-ttu-id="feb09-119">Outlook [事件][]</span><span class="sxs-lookup"><span data-stu-id="feb09-119">Outlook [event][]</span></span> | <span data-ttu-id="feb09-120">对用户邮箱中的所有事件更改：</span><span class="sxs-lookup"><span data-stu-id="feb09-120">Changes to all events in a user's mailbox:</span></span><br>`/users/{id}/events` | <span data-ttu-id="feb09-121">否</span><span class="sxs-lookup"><span data-stu-id="feb09-121">No</span></span> |
| <span data-ttu-id="feb09-122">Outlook 个人[联系人][]</span><span class="sxs-lookup"><span data-stu-id="feb09-122">Outlook personal [contact][]</span></span> | <span data-ttu-id="feb09-123">对用户邮箱中的所有个人联系人更改：</span><span class="sxs-lookup"><span data-stu-id="feb09-123">Changes to all personal contacts in a user's mailbox:</span></span><br>`/users/{id}/contacts` | <span data-ttu-id="feb09-124">否</span><span class="sxs-lookup"><span data-stu-id="feb09-124">No</span></span> |
| <span data-ttu-id="feb09-125">[用户][]</span><span class="sxs-lookup"><span data-stu-id="feb09-125">[user][]</span></span> | <span data-ttu-id="feb09-126">对所有用户更改：</span><span class="sxs-lookup"><span data-stu-id="feb09-126">Changes to all users:</span></span><br>`/users` <br><span data-ttu-id="feb09-127">对特定用户更改：</span><span class="sxs-lookup"><span data-stu-id="feb09-127">Changes to a specific user:</span></span><br>`/users/{id}`| <span data-ttu-id="feb09-128">否</span><span class="sxs-lookup"><span data-stu-id="feb09-128">No</span></span> |
| <span data-ttu-id="feb09-129">[组][]</span><span class="sxs-lookup"><span data-stu-id="feb09-129">[group][]</span></span> | <span data-ttu-id="feb09-130">对所有组更改：</span><span class="sxs-lookup"><span data-stu-id="feb09-130">Changes to all groups:</span></span><br>`/groups` <br><span data-ttu-id="feb09-131">对特定组更改：</span><span class="sxs-lookup"><span data-stu-id="feb09-131">Changes to a specific group:</span></span><br>`/groups/{id}` | <span data-ttu-id="feb09-132">否</span><span class="sxs-lookup"><span data-stu-id="feb09-132">No</span></span> |
| <span data-ttu-id="feb09-133">Office 365 组[对话][]</span><span class="sxs-lookup"><span data-stu-id="feb09-133">Office 365 group [conversation][]</span></span> | <span data-ttu-id="feb09-134">查看组的对话：</span><span class="sxs-lookup"><span data-stu-id="feb09-134">Changes to a group's conversations:</span></span><br>`groups/{id}/conversations` | <span data-ttu-id="feb09-135">否</span><span class="sxs-lookup"><span data-stu-id="feb09-135">No</span></span> |
| <span data-ttu-id="feb09-136">OneDrive（个人版）上的 [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="feb09-136">[driveItem][] on OneDrive (personal)</span></span> | <span data-ttu-id="feb09-137">对_任何文件夹_的层次结构内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="feb09-137">Changes to content within the hierarchy of _any folder_:</span></span><br>`/users/{id}/drive/root` | <span data-ttu-id="feb09-138">否</span><span class="sxs-lookup"><span data-stu-id="feb09-138">No</span></span> |
| <span data-ttu-id="feb09-139">OneDrive for Business 上的 [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="feb09-139">[driveItem][] on OneDrive for Business</span></span> | <span data-ttu-id="feb09-140">对_根文件夹_的层次结构内的内容更改：</span><span class="sxs-lookup"><span data-stu-id="feb09-140">Changes to content within the hierarchy of the _root folder_:</span></span><br>`/drives/{id}/root`<br> `/users/{id}/drive/root` | <span data-ttu-id="feb09-141">否</span><span class="sxs-lookup"><span data-stu-id="feb09-141">No</span></span> |
| <span data-ttu-id="feb09-142">SharePoint[网站][]下的[列表][]</span><span class="sxs-lookup"><span data-stu-id="feb09-142">[list][] under a SharePoint [site][]</span></span> | `/sites/{id}/lists/{id}` | <span data-ttu-id="feb09-143">否</span><span class="sxs-lookup"><span data-stu-id="feb09-143">No</span></span> |
| <span data-ttu-id="feb09-144">安全[警报][]</span><span class="sxs-lookup"><span data-stu-id="feb09-144">Security [alert][]</span></span> | <span data-ttu-id="feb09-145">对特定警报更改：</span><span class="sxs-lookup"><span data-stu-id="feb09-145">Changes to a specific alert:</span></span><br>`/security/alerts/{id}` <br><span data-ttu-id="feb09-146">对已筛选的警报更改：</span><span class="sxs-lookup"><span data-stu-id="feb09-146">Changes to filtered alerts:</span></span><br> `/security/alerts/?$filter`| <span data-ttu-id="feb09-147">否</span><span class="sxs-lookup"><span data-stu-id="feb09-147">No</span></span> |
| <span data-ttu-id="feb09-148">团队[callRecord][]</span><span class="sxs-lookup"><span data-stu-id="feb09-148">Teams [callRecord][]</span></span> | <span data-ttu-id="feb09-149">对_所有_呼叫记录的更改：`/communications/callRecords`</span><span class="sxs-lookup"><span data-stu-id="feb09-149">Changes to _all_ call records: `/communications/callRecords`</span></span> | <span data-ttu-id="feb09-150">否</span><span class="sxs-lookup"><span data-stu-id="feb09-150">No</span></span> |
| <span data-ttu-id="feb09-151">Teams [chatmessage](/graph/api/resources/subscription?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="feb09-151">Teams [chatmessage](/graph/api/resources/subscription?view=graph-rest-beta)</span></span> | <span data-ttu-id="feb09-152">对所有团队中所有频道聊天消息更改：</span><span class="sxs-lookup"><span data-stu-id="feb09-152">Changes to chat messages in all channels in all teams:</span></span><br>`/teams/allMessages` <br><span data-ttu-id="feb09-153">对特定频道中的聊天消息更改：</span><span class="sxs-lookup"><span data-stu-id="feb09-153">Changes to chat messages in a specific channel:</span></span><br>`/teams/{id}/channels/{id}/messages`<br><span data-ttu-id="feb09-154">对所有聊天的消息更改：</span><span class="sxs-lookup"><span data-stu-id="feb09-154">Changes to chat messages in all chats:</span></span><br>`/chats/allMessages` <br><span data-ttu-id="feb09-155">对特定聊天中的消息更改：</span><span class="sxs-lookup"><span data-stu-id="feb09-155">Changes to chat messages in a specific chat:</span></span><br>`/chats/{id}/messages` | <span data-ttu-id="feb09-156">是</span><span class="sxs-lookup"><span data-stu-id="feb09-156">Yes</span></span> |

> <span data-ttu-id="feb09-157">**注意**：以 `/users/{id}` 开头的任何资源路径还可接受 `/me` 以引用已登录的用户。</span><span class="sxs-lookup"><span data-stu-id="feb09-157">**Note**: Any resource path that begins with `/users/{id}` can also accept `/me` to reference the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="feb09-158">权限</span><span class="sxs-lookup"><span data-stu-id="feb09-158">Permissions</span></span>

<span data-ttu-id="feb09-159">通常订阅操作需要拥有对资源的读取权限。</span><span class="sxs-lookup"><span data-stu-id="feb09-159">In general, subscription operations require read permission to the resource.</span></span> <span data-ttu-id="feb09-160">例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。</span><span class="sxs-lookup"><span data-stu-id="feb09-160">For example, to get notifications for messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="feb09-161">[创建订阅](../api/subscription-post-subscriptions.md)一文列出了各个资源类型所需的权限。</span><span class="sxs-lookup"><span data-stu-id="feb09-161">The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type.</span></span> <span data-ttu-id="feb09-162">下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。</span><span class="sxs-lookup"><span data-stu-id="feb09-162">The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="feb09-163">权限类型</span><span class="sxs-lookup"><span data-stu-id="feb09-163">Permission type</span></span>                        | <span data-ttu-id="feb09-164">支持的资源类型</span><span class="sxs-lookup"><span data-stu-id="feb09-164">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="feb09-165">委派 - 工作或学校帐户</span><span class="sxs-lookup"><span data-stu-id="feb09-165">Delegated - work or school account</span></span>     | <span data-ttu-id="feb09-166">[警报][]、[联系人][]、[对话][]、 [driveItem][]、 [list][]、 [event][]、 [group][]、 [message][]、 [user][]</span><span class="sxs-lookup"><span data-stu-id="feb09-166">[alert][], [contact][], [conversation][], [driveItem][], [list][], [event][], [group][], [message][], [user][]</span></span>|
| <span data-ttu-id="feb09-167">委派 - 个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="feb09-167">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="feb09-168">[contact][]、 [driveItem][]、 [list][]、 [event][]、 [message][]</span><span class="sxs-lookup"><span data-stu-id="feb09-168">[contact][], [driveItem][], [list][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="feb09-169">应用程序</span><span class="sxs-lookup"><span data-stu-id="feb09-169">Application</span></span>                            | <span data-ttu-id="feb09-170">[alert][]、 [contact][]、 [driveItem][]、 [list][]、 [event][]、 [group][]、 [message][]、 [user][]、 [callRecord][]、[了 chatmessage][]</span><span class="sxs-lookup"><span data-stu-id="feb09-170">[alert][], [contact][], [driveItem][], [list][], [event][], [group][], [message][], [user][], [callRecord][], [chatMessage][]</span></span>|

## <a name="see-also"></a><span data-ttu-id="feb09-171">另请参阅</span><span class="sxs-lookup"><span data-stu-id="feb09-171">See also</span></span>

- [<span data-ttu-id="feb09-172">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="feb09-172">Subscription resource type</span></span>](subscription.md)
- [<span data-ttu-id="feb09-173">列出订阅</span><span class="sxs-lookup"><span data-stu-id="feb09-173">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="feb09-174">获取订阅</span><span class="sxs-lookup"><span data-stu-id="feb09-174">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="feb09-175">创建订阅</span><span class="sxs-lookup"><span data-stu-id="feb09-175">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="feb09-176">更新订阅</span><span class="sxs-lookup"><span data-stu-id="feb09-176">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="feb09-177">删除订阅</span><span class="sxs-lookup"><span data-stu-id="feb09-177">Delete subscription</span></span>](../api/subscription-delete.md)

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
[callRecord]: ./callrecords-callrecord.md
[警报]: ./alert.md
[alert]: ./alert.md
