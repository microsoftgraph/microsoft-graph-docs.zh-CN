---
title: 创建订阅
description: 订阅侦听器应用程序, 以在 Microsoft Graph 资源的数据发生更改时接收通知。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: a781d3654a54c8514b243f4a1f15772c5dd63fe8
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638573"
---
# <a name="create-subscription"></a><span data-ttu-id="785be-103">创建订阅</span><span class="sxs-lookup"><span data-stu-id="785be-103">Create subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="785be-104">订阅侦听器应用程序，以在 Microsoft Graph 中指定资源发生的更改属于请求的更改类型时接收通知。</span><span class="sxs-lookup"><span data-stu-id="785be-104">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="785be-105">权限</span><span class="sxs-lookup"><span data-stu-id="785be-105">Permissions</span></span>

<span data-ttu-id="785be-106">创建订阅需要读取资源范围。</span><span class="sxs-lookup"><span data-stu-id="785be-106">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="785be-107">例如，若要获取消息通知，应用需要 `Mail.Read` 权限。</span><span class="sxs-lookup"><span data-stu-id="785be-107">For example, to get notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
 <span data-ttu-id="785be-108">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="785be-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="785be-109">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="785be-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="785be-110">支持的资源</span><span class="sxs-lookup"><span data-stu-id="785be-110">Supported resource</span></span> | <span data-ttu-id="785be-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="785be-111">Delegated (work or school account)</span></span> | <span data-ttu-id="785be-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="785be-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="785be-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="785be-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="785be-114">联系人</span><span class="sxs-lookup"><span data-stu-id="785be-114">contact</span></span>](../resources/contact.md) | <span data-ttu-id="785be-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="785be-115">Contacts.Read</span></span> | <span data-ttu-id="785be-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="785be-116">Contacts.Read</span></span> | <span data-ttu-id="785be-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="785be-117">Contacts.Read</span></span> |
|<span data-ttu-id="785be-118">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="785be-118">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="785be-119">不支持</span><span class="sxs-lookup"><span data-stu-id="785be-119">Not supported</span></span> | <span data-ttu-id="785be-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="785be-120">Files.ReadWrite</span></span> | <span data-ttu-id="785be-121">不支持</span><span class="sxs-lookup"><span data-stu-id="785be-121">Not supported</span></span> |
|<span data-ttu-id="785be-122">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="785be-122">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="785be-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="785be-123">Files.ReadWrite.All</span></span> | <span data-ttu-id="785be-124">不支持</span><span class="sxs-lookup"><span data-stu-id="785be-124">Not supported</span></span> | <span data-ttu-id="785be-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="785be-125">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="785be-126">事件</span><span class="sxs-lookup"><span data-stu-id="785be-126">event</span></span>](../resources/event.md) | <span data-ttu-id="785be-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="785be-127">Calendars.Read</span></span> | <span data-ttu-id="785be-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="785be-128">Calendars.Read</span></span> | <span data-ttu-id="785be-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="785be-129">Calendars.Read</span></span> |
|[<span data-ttu-id="785be-130">组</span><span class="sxs-lookup"><span data-stu-id="785be-130">group</span></span>](../resources/group.md) | <span data-ttu-id="785be-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="785be-131">Group.Read.All</span></span> | <span data-ttu-id="785be-132">不支持</span><span class="sxs-lookup"><span data-stu-id="785be-132">Not supported</span></span> | <span data-ttu-id="785be-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="785be-133">Group.Read.All</span></span> |
|[<span data-ttu-id="785be-134">组对话</span><span class="sxs-lookup"><span data-stu-id="785be-134">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="785be-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="785be-135">Group.Read.All</span></span> | <span data-ttu-id="785be-136">不支持</span><span class="sxs-lookup"><span data-stu-id="785be-136">Not supported</span></span> | <span data-ttu-id="785be-137">不支持</span><span class="sxs-lookup"><span data-stu-id="785be-137">Not supported</span></span> |
|[<span data-ttu-id="785be-138">邮件</span><span class="sxs-lookup"><span data-stu-id="785be-138">message</span></span>](../resources/message.md) | <span data-ttu-id="785be-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="785be-139">Mail.Read</span></span> | <span data-ttu-id="785be-140">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="785be-140">Mail.Read</span></span> | <span data-ttu-id="785be-141">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="785be-141">Mail.Read</span></span> |
|<span data-ttu-id="785be-142">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="785be-142">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="785be-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="785be-143">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="785be-144">不支持</span><span class="sxs-lookup"><span data-stu-id="785be-144">Not supported</span></span> | <span data-ttu-id="785be-145">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="785be-145">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="785be-146">用户</span><span class="sxs-lookup"><span data-stu-id="785be-146">user</span></span>](../resources/user.md) | <span data-ttu-id="785be-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="785be-147">User.Read.All</span></span> | <span data-ttu-id="785be-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="785be-148">User.Read.All</span></span> | <span data-ttu-id="785be-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="785be-149">User.Read.All</span></span> |

> <span data-ttu-id="785be-150">**注意：** 订阅 OneDrive 和 Outlook 项还有其他限制。</span><span class="sxs-lookup"><span data-stu-id="785be-150">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="785be-151">这些限制适用于订阅的创建和管理（获取、更新和删除订阅）。</span><span class="sxs-lookup"><span data-stu-id="785be-151">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="785be-152">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="785be-152">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="785be-153">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="785be-153">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="785be-154">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送通知。</span><span class="sxs-lookup"><span data-stu-id="785be-154">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="785be-155">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="785be-155">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="785be-156">在 Outlook 中，委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="785be-156">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="785be-157">也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="785be-157">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="785be-158">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="785be-158">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="785be-159">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="785be-159">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="785be-160">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="785be-160">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="785be-161">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="785be-161">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="785be-162">请求标头</span><span class="sxs-lookup"><span data-stu-id="785be-162">Request headers</span></span>

| <span data-ttu-id="785be-163">名称</span><span class="sxs-lookup"><span data-stu-id="785be-163">Name</span></span>       | <span data-ttu-id="785be-164">类型</span><span class="sxs-lookup"><span data-stu-id="785be-164">Type</span></span> | <span data-ttu-id="785be-165">说明</span><span class="sxs-lookup"><span data-stu-id="785be-165">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="785be-166">Authorization</span><span class="sxs-lookup"><span data-stu-id="785be-166">Authorization</span></span>  | <span data-ttu-id="785be-167">string</span><span class="sxs-lookup"><span data-stu-id="785be-167">string</span></span>  | <span data-ttu-id="785be-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="785be-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="785be-170">响应</span><span class="sxs-lookup"><span data-stu-id="785be-170">Response</span></span>

<span data-ttu-id="785be-171">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="785be-171">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="785be-172">示例</span><span class="sxs-lookup"><span data-stu-id="785be-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="785be-173">请求</span><span class="sxs-lookup"><span data-stu-id="785be-173">Request</span></span>

<span data-ttu-id="785be-174">在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="785be-174">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="785be-175">`clientState` 字段是可选的。</span><span class="sxs-lookup"><span data-stu-id="785be-175">The `clientState` field is optional.</span></span>

<span data-ttu-id="785be-176">此示例请求创建一个订阅, 用于通知当前登录用户接收到的新邮件。</span><span class="sxs-lookup"><span data-stu-id="785be-176">This sample request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```

<span data-ttu-id="785be-177">以下是 resource 属性的有效值:</span><span class="sxs-lookup"><span data-stu-id="785be-177">The following are valid values for the resource property:</span></span>

| <span data-ttu-id="785be-178">资源类型</span><span class="sxs-lookup"><span data-stu-id="785be-178">Resource type</span></span> | <span data-ttu-id="785be-179">示例</span><span class="sxs-lookup"><span data-stu-id="785be-179">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="785be-180">邮件</span><span class="sxs-lookup"><span data-stu-id="785be-180">Mail</span></span>|<span data-ttu-id="785be-181">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="785be-181">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="785be-182">me/messages</span><span class="sxs-lookup"><span data-stu-id="785be-182">me/messages</span></span>|
|<span data-ttu-id="785be-183">联系人</span><span class="sxs-lookup"><span data-stu-id="785be-183">Contacts</span></span>|<span data-ttu-id="785be-184">me/contacts</span><span class="sxs-lookup"><span data-stu-id="785be-184">me/contacts</span></span>|
|<span data-ttu-id="785be-185">日历</span><span class="sxs-lookup"><span data-stu-id="785be-185">Calendars</span></span>|<span data-ttu-id="785be-186">me/events</span><span class="sxs-lookup"><span data-stu-id="785be-186">me/events</span></span>|
|<span data-ttu-id="785be-187">用户</span><span class="sxs-lookup"><span data-stu-id="785be-187">Users</span></span>|<span data-ttu-id="785be-188">users</span><span class="sxs-lookup"><span data-stu-id="785be-188">users</span></span>|
|<span data-ttu-id="785be-189">组</span><span class="sxs-lookup"><span data-stu-id="785be-189">Groups</span></span>|<span data-ttu-id="785be-190">groups</span><span class="sxs-lookup"><span data-stu-id="785be-190">groups</span></span>|
|<span data-ttu-id="785be-191">对话</span><span class="sxs-lookup"><span data-stu-id="785be-191">Conversations</span></span>|<span data-ttu-id="785be-192">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="785be-192">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="785be-193">驱动器</span><span class="sxs-lookup"><span data-stu-id="785be-193">Drives</span></span>|<span data-ttu-id="785be-194">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="785be-194">me/drive/root</span></span>|
|<span data-ttu-id="785be-195">安全警报</span><span class="sxs-lookup"><span data-stu-id="785be-195">Security alert</span></span>|<span data-ttu-id="785be-196">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="785be-196">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="785be-197">响应</span><span class="sxs-lookup"><span data-stu-id="785be-197">Response</span></span>

<span data-ttu-id="785be-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="785be-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "changeType": "created,updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="785be-201">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="785be-201">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="785be-202">语言</span><span class="sxs-lookup"><span data-stu-id="785be-202">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_subscription_from_subscriptions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="785be-203">Javascript</span><span class="sxs-lookup"><span data-stu-id="785be-203">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_subscription_from_subscriptions-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="notification-endpoint-validation"></a><span data-ttu-id="785be-204">通知终结点验证</span><span class="sxs-lookup"><span data-stu-id="785be-204">Notification endpoint validation</span></span>

<span data-ttu-id="785be-205">通知终结点（于 `notificationUrl` 属性中指定）必须能够响应验证请求，如[设置用户数据更改的通知](/graph/webhooks#notification-endpoint-validation)中所述。</span><span class="sxs-lookup"><span data-stu-id="785be-205">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="785be-206">如果验证失败，创建订阅请求返回错误“400 请求无效”。</span><span class="sxs-lookup"><span data-stu-id="785be-206">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
    "Error: /api-reference/beta/api/subscription-post-subscriptions.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/subscription-post-subscriptions.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
