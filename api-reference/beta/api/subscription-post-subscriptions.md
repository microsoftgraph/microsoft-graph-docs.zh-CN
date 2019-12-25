---
title: 创建订阅
description: 订阅侦听器应用程序，以在 Microsoft Graph 资源的数据发生更改时接收通知。
localization_priority: Normal
author: piotrci
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 487be3c7a50dcd5b09ece599f69b74248965eacf
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870824"
---
# <a name="create-subscription"></a><span data-ttu-id="c0f23-103">创建订阅</span><span class="sxs-lookup"><span data-stu-id="c0f23-103">Create subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0f23-104">订阅侦听器应用程序，以在 Microsoft Graph 中指定资源发生的更改属于请求的更改类型时接收通知。</span><span class="sxs-lookup"><span data-stu-id="c0f23-104">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0f23-105">权限</span><span class="sxs-lookup"><span data-stu-id="c0f23-105">Permissions</span></span>

<span data-ttu-id="c0f23-106">创建订阅需要对资源具有读取权限。</span><span class="sxs-lookup"><span data-stu-id="c0f23-106">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="c0f23-107">例如，若要获取有关邮件的通知，您的应用程序需要具有邮件读取权限。</span><span class="sxs-lookup"><span data-stu-id="c0f23-107">For example, to get notifications on messages, your app needs the Mail.Read permission.</span></span> 
 
 <span data-ttu-id="c0f23-108">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="c0f23-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="c0f23-109">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0f23-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c0f23-110">支持的资源</span><span class="sxs-lookup"><span data-stu-id="c0f23-110">Supported resource</span></span> | <span data-ttu-id="c0f23-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0f23-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c0f23-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0f23-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0f23-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0f23-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="c0f23-114">[了 chatmessage](../resources/chatmessage.md) （/teams/{id}/channels/{id}/messages）</span><span class="sxs-lookup"><span data-stu-id="c0f23-114">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="c0f23-115">不支持</span><span class="sxs-lookup"><span data-stu-id="c0f23-115">Not supported</span></span> | <span data-ttu-id="c0f23-116">不支持</span><span class="sxs-lookup"><span data-stu-id="c0f23-116">Not supported</span></span> | <span data-ttu-id="c0f23-117">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0f23-117">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="c0f23-118">[了 chatmessage](../resources/chatmessage.md) （/chats/{id}/messages）</span><span class="sxs-lookup"><span data-stu-id="c0f23-118">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="c0f23-119">不支持</span><span class="sxs-lookup"><span data-stu-id="c0f23-119">Not supported</span></span> | <span data-ttu-id="c0f23-120">不支持</span><span class="sxs-lookup"><span data-stu-id="c0f23-120">Not supported</span></span> | <span data-ttu-id="c0f23-121">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0f23-121">Chat.Read.All</span></span>  |
|[<span data-ttu-id="c0f23-122">联系人</span><span class="sxs-lookup"><span data-stu-id="c0f23-122">contact</span></span>](../resources/contact.md) | <span data-ttu-id="c0f23-123">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c0f23-123">Contacts.Read</span></span> | <span data-ttu-id="c0f23-124">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c0f23-124">Contacts.Read</span></span> | <span data-ttu-id="c0f23-125">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c0f23-125">Contacts.Read</span></span> |
|<span data-ttu-id="c0f23-126">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="c0f23-126">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="c0f23-127">不支持</span><span class="sxs-lookup"><span data-stu-id="c0f23-127">Not supported</span></span> | <span data-ttu-id="c0f23-128">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0f23-128">Files.ReadWrite</span></span> | <span data-ttu-id="c0f23-129">不支持</span><span class="sxs-lookup"><span data-stu-id="c0f23-129">Not supported</span></span> |
|<span data-ttu-id="c0f23-130">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="c0f23-130">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="c0f23-131">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0f23-131">Files.ReadWrite.All</span></span> | <span data-ttu-id="c0f23-132">不支持</span><span class="sxs-lookup"><span data-stu-id="c0f23-132">Not supported</span></span> | <span data-ttu-id="c0f23-133">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0f23-133">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="c0f23-134">事件</span><span class="sxs-lookup"><span data-stu-id="c0f23-134">event</span></span>](../resources/event.md) | <span data-ttu-id="c0f23-135">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c0f23-135">Calendars.Read</span></span> | <span data-ttu-id="c0f23-136">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c0f23-136">Calendars.Read</span></span> | <span data-ttu-id="c0f23-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c0f23-137">Calendars.Read</span></span> |
|[<span data-ttu-id="c0f23-138">组</span><span class="sxs-lookup"><span data-stu-id="c0f23-138">group</span></span>](../resources/group.md) | <span data-ttu-id="c0f23-139">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0f23-139">Group.Read.All</span></span> | <span data-ttu-id="c0f23-140">不支持</span><span class="sxs-lookup"><span data-stu-id="c0f23-140">Not supported</span></span> | <span data-ttu-id="c0f23-141">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0f23-141">Group.Read.All</span></span> |
|[<span data-ttu-id="c0f23-142">组对话</span><span class="sxs-lookup"><span data-stu-id="c0f23-142">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="c0f23-143">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0f23-143">Group.Read.All</span></span> | <span data-ttu-id="c0f23-144">不支持</span><span class="sxs-lookup"><span data-stu-id="c0f23-144">Not supported</span></span> | <span data-ttu-id="c0f23-145">不支持</span><span class="sxs-lookup"><span data-stu-id="c0f23-145">Not supported</span></span> |
|[<span data-ttu-id="c0f23-146">邮件</span><span class="sxs-lookup"><span data-stu-id="c0f23-146">message</span></span>](../resources/message.md) | <span data-ttu-id="c0f23-147">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c0f23-147">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="c0f23-148">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c0f23-148">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="c0f23-149">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c0f23-149">Mail.ReadBasic, Mail.Read</span></span> |
|<span data-ttu-id="c0f23-150">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="c0f23-150">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="c0f23-151">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0f23-151">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="c0f23-152">不支持</span><span class="sxs-lookup"><span data-stu-id="c0f23-152">Not supported</span></span> | <span data-ttu-id="c0f23-153">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0f23-153">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="c0f23-154">用户</span><span class="sxs-lookup"><span data-stu-id="c0f23-154">user</span></span>](../resources/user.md) | <span data-ttu-id="c0f23-155">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0f23-155">User.Read.All</span></span> | <span data-ttu-id="c0f23-156">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0f23-156">User.Read.All</span></span> | <span data-ttu-id="c0f23-157">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0f23-157">User.Read.All</span></span> |

> <span data-ttu-id="c0f23-158">**注意：** 在2020年1月，了 chatmessage 订阅将需要[加密](/graph/webhooks-with-resource-data)，如果未指定[encryptionCertificate](../resources/subscription.md) ，则订阅创建将失败。</span><span class="sxs-lookup"><span data-stu-id="c0f23-158">**Note:** In January 2020, chatMessage subscriptions will require [encryption](/graph/webhooks-with-resource-data), and subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

> <span data-ttu-id="c0f23-159">**注意：** 对 OneDrive 和 Outlook 项目的订阅适用其他限制。</span><span class="sxs-lookup"><span data-stu-id="c0f23-159">**Note:** Additional limitations apply for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="c0f23-160">这些限制适用于创建和管理（获取、更新和删除）订阅。</span><span class="sxs-lookup"><span data-stu-id="c0f23-160">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="c0f23-161">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="c0f23-161">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="c0f23-162">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="c0f23-162">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="c0f23-163">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送通知。</span><span class="sxs-lookup"><span data-stu-id="c0f23-163">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="c0f23-164">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="c0f23-164">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="c0f23-165">在 Outlook 中，委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="c0f23-165">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="c0f23-166">也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="c0f23-166">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="c0f23-167">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="c0f23-167">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="c0f23-168">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="c0f23-168">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="c0f23-169">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="c0f23-169">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="c0f23-170">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0f23-170">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="c0f23-171">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0f23-171">Request headers</span></span>

| <span data-ttu-id="c0f23-172">名称</span><span class="sxs-lookup"><span data-stu-id="c0f23-172">Name</span></span>       | <span data-ttu-id="c0f23-173">类型</span><span class="sxs-lookup"><span data-stu-id="c0f23-173">Type</span></span> | <span data-ttu-id="c0f23-174">说明</span><span class="sxs-lookup"><span data-stu-id="c0f23-174">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c0f23-175">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0f23-175">Authorization</span></span>  | <span data-ttu-id="c0f23-176">string</span><span class="sxs-lookup"><span data-stu-id="c0f23-176">string</span></span>  | <span data-ttu-id="c0f23-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c0f23-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c0f23-179">响应</span><span class="sxs-lookup"><span data-stu-id="c0f23-179">Response</span></span>

<span data-ttu-id="c0f23-180">如果成功，此方法在响应`201 Created`正文中返回响应代码和[订阅](../resources/subscription.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c0f23-180">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0f23-181">示例</span><span class="sxs-lookup"><span data-stu-id="c0f23-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0f23-182">请求</span><span class="sxs-lookup"><span data-stu-id="c0f23-182">Request</span></span>

<span data-ttu-id="c0f23-183">在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0f23-183">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="c0f23-184">`clientState` 字段是可选的。</span><span class="sxs-lookup"><span data-stu-id="c0f23-184">The `clientState` field is optional.</span></span>

<span data-ttu-id="c0f23-185">此请求创建一个订阅，用于通知当前登录用户接收到的新邮件。</span><span class="sxs-lookup"><span data-stu-id="c0f23-185">This request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c0f23-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0f23-186">HTTP</span></span>](#tab/http)
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
   "clientState": "secretClientValue"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c0f23-187">C#</span><span class="sxs-lookup"><span data-stu-id="c0f23-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c0f23-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0f23-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c0f23-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0f23-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="c0f23-190">以下是 resource 属性的有效值。</span><span class="sxs-lookup"><span data-stu-id="c0f23-190">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="c0f23-191">资源类型</span><span class="sxs-lookup"><span data-stu-id="c0f23-191">Resource type</span></span> | <span data-ttu-id="c0f23-192">示例</span><span class="sxs-lookup"><span data-stu-id="c0f23-192">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="c0f23-193">邮件</span><span class="sxs-lookup"><span data-stu-id="c0f23-193">Mail</span></span>|<span data-ttu-id="c0f23-194">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="c0f23-194">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="c0f23-195">me/messages</span><span class="sxs-lookup"><span data-stu-id="c0f23-195">me/messages</span></span>|
|<span data-ttu-id="c0f23-196">联系人</span><span class="sxs-lookup"><span data-stu-id="c0f23-196">Contacts</span></span>|<span data-ttu-id="c0f23-197">me/contacts</span><span class="sxs-lookup"><span data-stu-id="c0f23-197">me/contacts</span></span>|
|<span data-ttu-id="c0f23-198">日历</span><span class="sxs-lookup"><span data-stu-id="c0f23-198">Calendars</span></span>|<span data-ttu-id="c0f23-199">me/events</span><span class="sxs-lookup"><span data-stu-id="c0f23-199">me/events</span></span>|
|<span data-ttu-id="c0f23-200">用户</span><span class="sxs-lookup"><span data-stu-id="c0f23-200">Users</span></span>|<span data-ttu-id="c0f23-201">users</span><span class="sxs-lookup"><span data-stu-id="c0f23-201">users</span></span>|
|<span data-ttu-id="c0f23-202">组</span><span class="sxs-lookup"><span data-stu-id="c0f23-202">Groups</span></span>|<span data-ttu-id="c0f23-203">groups</span><span class="sxs-lookup"><span data-stu-id="c0f23-203">groups</span></span>|
|<span data-ttu-id="c0f23-204">对话</span><span class="sxs-lookup"><span data-stu-id="c0f23-204">Conversations</span></span>|<span data-ttu-id="c0f23-205">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="c0f23-205">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="c0f23-206">驱动器</span><span class="sxs-lookup"><span data-stu-id="c0f23-206">Drives</span></span>|<span data-ttu-id="c0f23-207">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="c0f23-207">me/drive/root</span></span>|
|<span data-ttu-id="c0f23-208">安全警报</span><span class="sxs-lookup"><span data-stu-id="c0f23-208">Security alert</span></span>|<span data-ttu-id="c0f23-209">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="c0f23-209">security/alerts?$filter=status eq ‘New’</span></span>|

### <a name="response"></a><span data-ttu-id="c0f23-210">响应</span><span class="sxs-lookup"><span data-stu-id="c0f23-210">Response</span></span>

<span data-ttu-id="c0f23-211">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="c0f23-211">The following example shows the response.</span></span> 

><span data-ttu-id="c0f23-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c0f23-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="c0f23-214">通知终结点验证</span><span class="sxs-lookup"><span data-stu-id="c0f23-214">Notification endpoint validation</span></span>

<span data-ttu-id="c0f23-215">订阅通知终结点（在**notificationUrl**属性中指定）必须能够响应验证请求，如[设置用户数据中的更改通知](/graph/webhooks#notification-endpoint-validation)中所述。</span><span class="sxs-lookup"><span data-stu-id="c0f23-215">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="c0f23-216">如果验证失败，创建订阅请求返回错误“400 请求无效”。</span><span class="sxs-lookup"><span data-stu-id="c0f23-216">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
