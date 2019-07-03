---
title: 创建订阅
description: 订阅侦听器应用程序，以在 Microsoft Graph 中的数据发生更改时接收通知。
localization_priority: Priority
author: piotrci
ms.openlocfilehash: 1d7b8c65df3aefba65a992d6212d170144f00f2b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450462"
---
# <a name="create-subscription"></a><span data-ttu-id="da173-103">创建订阅</span><span class="sxs-lookup"><span data-stu-id="da173-103">Create subscription</span></span>

<span data-ttu-id="da173-104">订阅侦听器应用程序，以在 Microsoft Graph 中指定资源发生的更改属于请求的更改类型时接收通知。</span><span class="sxs-lookup"><span data-stu-id="da173-104">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="da173-105">权限</span><span class="sxs-lookup"><span data-stu-id="da173-105">Permissions</span></span>

 <span data-ttu-id="da173-106">创建订阅需要读取资源范围。</span><span class="sxs-lookup"><span data-stu-id="da173-106">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="da173-107">例如，若要获取消息通知，应用需要 `Mail.Read` 权限。</span><span class="sxs-lookup"><span data-stu-id="da173-107">For example, to get notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
 <span data-ttu-id="da173-108">根据请求的资源和权限类型（委托或应用程序），下表中指定的权限为调用此 API 所需的最小权限。</span><span class="sxs-lookup"><span data-stu-id="da173-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="da173-109">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da173-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="da173-110">支持的资源</span><span class="sxs-lookup"><span data-stu-id="da173-110">Supported resource</span></span> | <span data-ttu-id="da173-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da173-111">Delegated (work or school account)</span></span> | <span data-ttu-id="da173-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da173-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da173-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="da173-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="da173-114">联系人</span><span class="sxs-lookup"><span data-stu-id="da173-114">contact</span></span>](../resources/contact.md) | <span data-ttu-id="da173-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="da173-115">Contacts.Read</span></span> | <span data-ttu-id="da173-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="da173-116">Contacts.Read</span></span> | <span data-ttu-id="da173-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="da173-117">Contacts.Read</span></span> |
|<span data-ttu-id="da173-118">[driveItem](../resources/driveitem.md)（用户的个人 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="da173-118">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="da173-119">不支持</span><span class="sxs-lookup"><span data-stu-id="da173-119">Not supported</span></span> | <span data-ttu-id="da173-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da173-120">Files.ReadWrite</span></span> | <span data-ttu-id="da173-121">不支持</span><span class="sxs-lookup"><span data-stu-id="da173-121">Not supported</span></span> |
|<span data-ttu-id="da173-122">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="da173-122">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="da173-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da173-123">Files.ReadWrite.All</span></span> | <span data-ttu-id="da173-124">不支持</span><span class="sxs-lookup"><span data-stu-id="da173-124">Not supported</span></span> | <span data-ttu-id="da173-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da173-125">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="da173-126">事件</span><span class="sxs-lookup"><span data-stu-id="da173-126">event</span></span>](../resources/event.md) | <span data-ttu-id="da173-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="da173-127">Calendars.Read</span></span> | <span data-ttu-id="da173-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="da173-128">Calendars.Read</span></span> | <span data-ttu-id="da173-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="da173-129">Calendars.Read</span></span> |
|[<span data-ttu-id="da173-130">组</span><span class="sxs-lookup"><span data-stu-id="da173-130">group</span></span>](../resources/group.md) | <span data-ttu-id="da173-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="da173-131">Group.Read.All</span></span> | <span data-ttu-id="da173-132">不支持</span><span class="sxs-lookup"><span data-stu-id="da173-132">Not supported</span></span> | <span data-ttu-id="da173-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="da173-133">Group.Read.All</span></span> |
|[<span data-ttu-id="da173-134">组对话</span><span class="sxs-lookup"><span data-stu-id="da173-134">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="da173-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="da173-135">Group.Read.All</span></span> | <span data-ttu-id="da173-136">不支持</span><span class="sxs-lookup"><span data-stu-id="da173-136">Not supported</span></span> | <span data-ttu-id="da173-137">不支持</span><span class="sxs-lookup"><span data-stu-id="da173-137">Not supported</span></span> |
|[<span data-ttu-id="da173-138">邮件</span><span class="sxs-lookup"><span data-stu-id="da173-138">message</span></span>](../resources/message.md) | <span data-ttu-id="da173-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="da173-139">Mail.Read</span></span> | <span data-ttu-id="da173-140">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="da173-140">Mail.Read</span></span> | <span data-ttu-id="da173-141">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="da173-141">Mail.Read</span></span> |
|<span data-ttu-id="da173-142">安全[警报](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="da173-142">[security alert](../resources/alert.md)</span></span> | <span data-ttu-id="da173-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da173-143">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="da173-144">不支持</span><span class="sxs-lookup"><span data-stu-id="da173-144">Not supported</span></span> | <span data-ttu-id="da173-145">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da173-145">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="da173-146">用户</span><span class="sxs-lookup"><span data-stu-id="da173-146">user</span></span>](../resources/user.md) | <span data-ttu-id="da173-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="da173-147">User.Read.All</span></span> | <span data-ttu-id="da173-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="da173-148">User.Read.All</span></span> | <span data-ttu-id="da173-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="da173-149">User.Read.All</span></span> |

> <span data-ttu-id="da173-150">**注意：** 订阅 OneDrive 和 Outlook 项还有其他限制。</span><span class="sxs-lookup"><span data-stu-id="da173-150">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="da173-151">这些限制适用于订阅的创建和管理（获取、更新和删除订阅）。</span><span class="sxs-lookup"><span data-stu-id="da173-151">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="da173-152">在个人 OneDrive 上，可订阅根文件夹或该驱动器中的任何子文件夹。</span><span class="sxs-lookup"><span data-stu-id="da173-152">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="da173-153">在 OneDrive for Business 上，只可以订阅根文件夹。</span><span class="sxs-lookup"><span data-stu-id="da173-153">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="da173-154">对订阅的文件夹或者其层次结构中的任何文件、文件夹或其他 **driveItem** 实例所做更改属于请求的更改类型时，发送通知。</span><span class="sxs-lookup"><span data-stu-id="da173-154">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="da173-155">无法订阅不是文件夹的“**驱动器**”或“**driveItem**”实例，例如单个文件。</span><span class="sxs-lookup"><span data-stu-id="da173-155">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="da173-156">在 Outlook 中，委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。</span><span class="sxs-lookup"><span data-stu-id="da173-156">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="da173-157">也就是说，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。</span><span class="sxs-lookup"><span data-stu-id="da173-157">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="da173-158">订阅_共享或委托_文件夹中 Outlook 联系人、事件或邮件的更改通知：</span><span class="sxs-lookup"><span data-stu-id="da173-158">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="da173-159">使用相应的应用程序权限订阅租户内_任何_用户的文件夹或邮箱中项目的更改。</span><span class="sxs-lookup"><span data-stu-id="da173-159">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="da173-160">切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们**不**支持订阅对共享或委托文件夹中的项的更改通知。</span><span class="sxs-lookup"><span data-stu-id="da173-160">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span> 


## <a name="http-request"></a><span data-ttu-id="da173-161">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da173-161">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="da173-162">请求标头</span><span class="sxs-lookup"><span data-stu-id="da173-162">Request headers</span></span>

| <span data-ttu-id="da173-163">名称</span><span class="sxs-lookup"><span data-stu-id="da173-163">Name</span></span>       | <span data-ttu-id="da173-164">类型</span><span class="sxs-lookup"><span data-stu-id="da173-164">Type</span></span> | <span data-ttu-id="da173-165">说明</span><span class="sxs-lookup"><span data-stu-id="da173-165">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="da173-166">Authorization</span><span class="sxs-lookup"><span data-stu-id="da173-166">Authorization</span></span>  | <span data-ttu-id="da173-167">string</span><span class="sxs-lookup"><span data-stu-id="da173-167">string</span></span>  | <span data-ttu-id="da173-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="da173-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="da173-170">响应</span><span class="sxs-lookup"><span data-stu-id="da173-170">Response</span></span>

<span data-ttu-id="da173-171">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="da173-171">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da173-172">示例</span><span class="sxs-lookup"><span data-stu-id="da173-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="da173-173">请求</span><span class="sxs-lookup"><span data-stu-id="da173-173">Request</span></span>

<span data-ttu-id="da173-174">下面是在用户收到新邮件时请求发送通知的示例。</span><span class="sxs-lookup"><span data-stu-id="da173-174">Here is an example of the request to send a notification when the user receives a new mail.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="da173-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="da173-175">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="da173-176">C#</span><span class="sxs-lookup"><span data-stu-id="da173-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="da173-177">Javascript</span><span class="sxs-lookup"><span data-stu-id="da173-177">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="da173-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da173-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="da173-179">在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da173-179">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="da173-180">`clientState` 字段是可选的。</span><span class="sxs-lookup"><span data-stu-id="da173-180">The `clientState` field is optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="da173-181">资源示例</span><span class="sxs-lookup"><span data-stu-id="da173-181">Resources examples</span></span>

<span data-ttu-id="da173-182">订阅资源属性的有效值如下：</span><span class="sxs-lookup"><span data-stu-id="da173-182">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="da173-183">资源类型</span><span class="sxs-lookup"><span data-stu-id="da173-183">Resource type</span></span> | <span data-ttu-id="da173-184">示例</span><span class="sxs-lookup"><span data-stu-id="da173-184">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="da173-185">邮件</span><span class="sxs-lookup"><span data-stu-id="da173-185">Mail</span></span>|<span data-ttu-id="da173-186">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="da173-186">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="da173-187">me/messages</span><span class="sxs-lookup"><span data-stu-id="da173-187">me/messages</span></span>|
|<span data-ttu-id="da173-188">联系人</span><span class="sxs-lookup"><span data-stu-id="da173-188">Contacts</span></span>|<span data-ttu-id="da173-189">me/contacts</span><span class="sxs-lookup"><span data-stu-id="da173-189">me/contacts</span></span>|
|<span data-ttu-id="da173-190">日历</span><span class="sxs-lookup"><span data-stu-id="da173-190">Calendars</span></span>|<span data-ttu-id="da173-191">me/events</span><span class="sxs-lookup"><span data-stu-id="da173-191">me/events</span></span>|
|<span data-ttu-id="da173-192">用户</span><span class="sxs-lookup"><span data-stu-id="da173-192">Users</span></span>|<span data-ttu-id="da173-193">users</span><span class="sxs-lookup"><span data-stu-id="da173-193">users</span></span>|
|<span data-ttu-id="da173-194">组</span><span class="sxs-lookup"><span data-stu-id="da173-194">Groups</span></span>|<span data-ttu-id="da173-195">groups</span><span class="sxs-lookup"><span data-stu-id="da173-195">groups</span></span>|
|<span data-ttu-id="da173-196">对话</span><span class="sxs-lookup"><span data-stu-id="da173-196">Conversations</span></span>|<span data-ttu-id="da173-197">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="da173-197">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="da173-198">驱动器</span><span class="sxs-lookup"><span data-stu-id="da173-198">Drives</span></span>|<span data-ttu-id="da173-199">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="da173-199">me/drive/root</span></span>|
|<span data-ttu-id="da173-200">安全警报</span><span class="sxs-lookup"><span data-stu-id="da173-200">Security alert</span></span>|<span data-ttu-id="da173-201">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="da173-201">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="da173-202">响应</span><span class="sxs-lookup"><span data-stu-id="da173-202">Response</span></span>

<span data-ttu-id="da173-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="da173-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="da173-206">通知终结点验证</span><span class="sxs-lookup"><span data-stu-id="da173-206">Notification endpoint validation</span></span>

<span data-ttu-id="da173-207">通知终结点（于 `notificationUrl` 属性中指定）必须能够响应验证请求，如[设置用户数据更改的通知](/graph/webhooks#notification-endpoint-validation)中所述。</span><span class="sxs-lookup"><span data-stu-id="da173-207">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="da173-208">如果验证失败，创建订阅请求返回错误“400 请求无效”。</span><span class="sxs-lookup"><span data-stu-id="da173-208">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
