---
title: 创建订阅
description: 订阅侦听器应用程序，以在 Microsoft Graph 资源的数据发生更改时接收通知。
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: fff6dd2d707ba75db352837e77089f97e58cb325
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774385"
---
# <a name="create-subscription"></a><span data-ttu-id="20ae4-103">创建订阅</span><span class="sxs-lookup"><span data-stu-id="20ae4-103">Create subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20ae4-104">订阅侦听器应用程序，以在 Microsoft Graph 中指定资源发生的更改属于请求的更改类型时接收通知。</span><span class="sxs-lookup"><span data-stu-id="20ae4-104">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="20ae4-105">权限</span><span class="sxs-lookup"><span data-stu-id="20ae4-105">Permissions</span></span>

<span data-ttu-id="20ae4-106">创建订阅需要对资源具有读取权限。</span><span class="sxs-lookup"><span data-stu-id="20ae4-106">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="20ae4-107">例如，若要获取有关邮件的通知，您的应用程序需要具有邮件读取权限。</span><span class="sxs-lookup"><span data-stu-id="20ae4-107">For example, to get notifications on messages, your app needs the Mail.Read permission.</span></span> 
 
 <span data-ttu-id="20ae4-108">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="20ae4-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="20ae4-109">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="20ae4-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="20ae4-110">支持的资源</span><span class="sxs-lookup"><span data-stu-id="20ae4-110">Supported resource</span></span> | <span data-ttu-id="20ae4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20ae4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="20ae4-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20ae4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20ae4-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="20ae4-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="20ae4-114">[了 chatmessage](../resources/chatmessage.md) （/teams/{id}/channels/{id}/messages）</span><span class="sxs-lookup"><span data-stu-id="20ae4-114">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="20ae4-115">不支持</span><span class="sxs-lookup"><span data-stu-id="20ae4-115">Not supported</span></span> | <span data-ttu-id="20ae4-116">不支持</span><span class="sxs-lookup"><span data-stu-id="20ae4-116">Not supported</span></span> | <span data-ttu-id="20ae4-117">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="20ae4-117">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="20ae4-118">[了 chatmessage](../resources/chatmessage.md) （/chats/{id}/messages）</span><span class="sxs-lookup"><span data-stu-id="20ae4-118">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="20ae4-119">不支持</span><span class="sxs-lookup"><span data-stu-id="20ae4-119">Not supported</span></span> | <span data-ttu-id="20ae4-120">不支持</span><span class="sxs-lookup"><span data-stu-id="20ae4-120">Not supported</span></span> | <span data-ttu-id="20ae4-121">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="20ae4-121">Chat.Read.All</span></span>  |
|[<span data-ttu-id="20ae4-122">联系人</span><span class="sxs-lookup"><span data-stu-id="20ae4-122">contact</span></span>](../resources/contact.md) | <span data-ttu-id="20ae4-123">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="20ae4-123">Contacts.Read</span></span> | <span data-ttu-id="20ae4-124">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="20ae4-124">Contacts.Read</span></span> | <span data-ttu-id="20ae4-125">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="20ae4-125">Contacts.Read</span></span> |
|<span data-ttu-id="20ae4-126">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="20ae4-126">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="20ae4-127">不支持</span><span class="sxs-lookup"><span data-stu-id="20ae4-127">Not supported</span></span> | <span data-ttu-id="20ae4-128">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20ae4-128">Files.ReadWrite</span></span> | <span data-ttu-id="20ae4-129">不支持</span><span class="sxs-lookup"><span data-stu-id="20ae4-129">Not supported</span></span> |
|<span data-ttu-id="20ae4-130">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="20ae4-130">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="20ae4-131">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20ae4-131">Files.ReadWrite.All</span></span> | <span data-ttu-id="20ae4-132">不支持</span><span class="sxs-lookup"><span data-stu-id="20ae4-132">Not supported</span></span> | <span data-ttu-id="20ae4-133">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20ae4-133">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="20ae4-134">事件</span><span class="sxs-lookup"><span data-stu-id="20ae4-134">event</span></span>](../resources/event.md) | <span data-ttu-id="20ae4-135">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="20ae4-135">Calendars.Read</span></span> | <span data-ttu-id="20ae4-136">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="20ae4-136">Calendars.Read</span></span> | <span data-ttu-id="20ae4-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="20ae4-137">Calendars.Read</span></span> |
|[<span data-ttu-id="20ae4-138">组</span><span class="sxs-lookup"><span data-stu-id="20ae4-138">group</span></span>](../resources/group.md) | <span data-ttu-id="20ae4-139">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="20ae4-139">Group.Read.All</span></span> | <span data-ttu-id="20ae4-140">不支持</span><span class="sxs-lookup"><span data-stu-id="20ae4-140">Not supported</span></span> | <span data-ttu-id="20ae4-141">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="20ae4-141">Group.Read.All</span></span> |
|[<span data-ttu-id="20ae4-142">组对话</span><span class="sxs-lookup"><span data-stu-id="20ae4-142">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="20ae4-143">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="20ae4-143">Group.Read.All</span></span> | <span data-ttu-id="20ae4-144">不支持</span><span class="sxs-lookup"><span data-stu-id="20ae4-144">Not supported</span></span> | <span data-ttu-id="20ae4-145">不支持</span><span class="sxs-lookup"><span data-stu-id="20ae4-145">Not supported</span></span> |
|[<span data-ttu-id="20ae4-146">邮件</span><span class="sxs-lookup"><span data-stu-id="20ae4-146">message</span></span>](../resources/message.md) | <span data-ttu-id="20ae4-147">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="20ae4-147">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="20ae4-148">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="20ae4-148">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="20ae4-149">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="20ae4-149">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="20ae4-150">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="20ae4-150">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="20ae4-151">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20ae4-151">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="20ae4-152">不支持</span><span class="sxs-lookup"><span data-stu-id="20ae4-152">Not supported</span></span> | <span data-ttu-id="20ae4-153">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20ae4-153">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="20ae4-154">用户</span><span class="sxs-lookup"><span data-stu-id="20ae4-154">user</span></span>](../resources/user.md) | <span data-ttu-id="20ae4-155">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="20ae4-155">User.Read.All</span></span> | <span data-ttu-id="20ae4-156">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="20ae4-156">User.Read.All</span></span> | <span data-ttu-id="20ae4-157">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="20ae4-157">User.Read.All</span></span> |

> <span data-ttu-id="20ae4-158">**注意：** 了 chatmessage 订阅需要[加密](/graph/webhooks-with-resource-data)。</span><span class="sxs-lookup"><span data-stu-id="20ae4-158">**Note:** chatMessage subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="20ae4-159">如果未指定[encryptionCertificate](../resources/subscription.md) ，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="20ae4-159">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

> <span data-ttu-id="20ae4-160">**注意：** 对 OneDrive 和 Outlook 项目的订阅适用其他限制。</span><span class="sxs-lookup"><span data-stu-id="20ae4-160">**Note:** Additional limitations apply for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="20ae4-161">这些限制适用于创建和管理（获取、更新和删除）订阅。</span><span class="sxs-lookup"><span data-stu-id="20ae4-161">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="20ae4-162">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="20ae4-162">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="20ae4-163">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="20ae4-163">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="20ae4-164">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送通知。</span><span class="sxs-lookup"><span data-stu-id="20ae4-164">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="20ae4-165">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="20ae4-165">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="20ae4-166">在 Outlook 中，委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="20ae4-166">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="20ae4-167">也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="20ae4-167">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="20ae4-168">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="20ae4-168">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="20ae4-169">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="20ae4-169">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="20ae4-170">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="20ae4-170">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="20ae4-171">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20ae4-171">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="20ae4-172">请求标头</span><span class="sxs-lookup"><span data-stu-id="20ae4-172">Request headers</span></span>

| <span data-ttu-id="20ae4-173">名称</span><span class="sxs-lookup"><span data-stu-id="20ae4-173">Name</span></span>       | <span data-ttu-id="20ae4-174">类型</span><span class="sxs-lookup"><span data-stu-id="20ae4-174">Type</span></span> | <span data-ttu-id="20ae4-175">说明</span><span class="sxs-lookup"><span data-stu-id="20ae4-175">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="20ae4-176">Authorization</span><span class="sxs-lookup"><span data-stu-id="20ae4-176">Authorization</span></span>  | <span data-ttu-id="20ae4-177">string</span><span class="sxs-lookup"><span data-stu-id="20ae4-177">string</span></span>  | <span data-ttu-id="20ae4-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="20ae4-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="20ae4-180">响应</span><span class="sxs-lookup"><span data-stu-id="20ae4-180">Response</span></span>

<span data-ttu-id="20ae4-181">如果成功，此方法在响应`201 Created`正文中返回响应代码和[订阅](../resources/subscription.md)对象。</span><span class="sxs-lookup"><span data-stu-id="20ae4-181">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20ae4-182">示例</span><span class="sxs-lookup"><span data-stu-id="20ae4-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="20ae4-183">请求</span><span class="sxs-lookup"><span data-stu-id="20ae4-183">Request</span></span>

<span data-ttu-id="20ae4-184">在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20ae4-184">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="20ae4-185">" `clientState` " `latestSupportedTlsVersion`和 "" 字段是可选的。</span><span class="sxs-lookup"><span data-stu-id="20ae4-185">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="20ae4-186">此请求创建一个订阅，用于通知当前登录用户接收到的新邮件。</span><span class="sxs-lookup"><span data-stu-id="20ae4-186">This request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="20ae4-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="20ae4-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue",
   "latestSupportedTlsVersion": "v1_2"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="20ae4-188">C#</span><span class="sxs-lookup"><span data-stu-id="20ae4-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="20ae4-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20ae4-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="20ae4-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20ae4-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="20ae4-191">以下是 resource 属性的有效值。</span><span class="sxs-lookup"><span data-stu-id="20ae4-191">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="20ae4-192">资源类型</span><span class="sxs-lookup"><span data-stu-id="20ae4-192">Resource type</span></span> | <span data-ttu-id="20ae4-193">示例</span><span class="sxs-lookup"><span data-stu-id="20ae4-193">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="20ae4-194">邮件</span><span class="sxs-lookup"><span data-stu-id="20ae4-194">Mail</span></span>|<span data-ttu-id="20ae4-195">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="20ae4-195">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="20ae4-196">me/messages</span><span class="sxs-lookup"><span data-stu-id="20ae4-196">me/messages</span></span>|
|<span data-ttu-id="20ae4-197">联系人</span><span class="sxs-lookup"><span data-stu-id="20ae4-197">Contacts</span></span>|<span data-ttu-id="20ae4-198">me/contacts</span><span class="sxs-lookup"><span data-stu-id="20ae4-198">me/contacts</span></span>|
|<span data-ttu-id="20ae4-199">日历</span><span class="sxs-lookup"><span data-stu-id="20ae4-199">Calendars</span></span>|<span data-ttu-id="20ae4-200">me/events</span><span class="sxs-lookup"><span data-stu-id="20ae4-200">me/events</span></span>|
|<span data-ttu-id="20ae4-201">用户</span><span class="sxs-lookup"><span data-stu-id="20ae4-201">Users</span></span>|<span data-ttu-id="20ae4-202">users</span><span class="sxs-lookup"><span data-stu-id="20ae4-202">users</span></span>|
|<span data-ttu-id="20ae4-203">组</span><span class="sxs-lookup"><span data-stu-id="20ae4-203">Groups</span></span>|<span data-ttu-id="20ae4-204">groups</span><span class="sxs-lookup"><span data-stu-id="20ae4-204">groups</span></span>|
|<span data-ttu-id="20ae4-205">对话</span><span class="sxs-lookup"><span data-stu-id="20ae4-205">Conversations</span></span>|<span data-ttu-id="20ae4-206">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="20ae4-206">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="20ae4-207">驱动器</span><span class="sxs-lookup"><span data-stu-id="20ae4-207">Drives</span></span>|<span data-ttu-id="20ae4-208">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="20ae4-208">me/drive/root</span></span>|
|<span data-ttu-id="20ae4-209">安全警报</span><span class="sxs-lookup"><span data-stu-id="20ae4-209">Security alert</span></span>|<span data-ttu-id="20ae4-210">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="20ae4-210">security/alerts?$filter=status eq ‘New’</span></span>|

### <a name="response"></a><span data-ttu-id="20ae4-211">响应</span><span class="sxs-lookup"><span data-stu-id="20ae4-211">Response</span></span>

<span data-ttu-id="20ae4-212">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="20ae4-212">The following example shows the response.</span></span> 

><span data-ttu-id="20ae4-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="20ae4-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 252

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="20ae4-215">通知终结点验证</span><span class="sxs-lookup"><span data-stu-id="20ae4-215">Notification endpoint validation</span></span>

<span data-ttu-id="20ae4-216">订阅通知终结点（在**notificationUrl**属性中指定）必须能够响应验证请求，如[设置用户数据中的更改通知](/graph/webhooks#notification-endpoint-validation)中所述。</span><span class="sxs-lookup"><span data-stu-id="20ae4-216">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="20ae4-217">如果验证失败，创建订阅请求返回错误“400 请求无效”。</span><span class="sxs-lookup"><span data-stu-id="20ae4-217">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
