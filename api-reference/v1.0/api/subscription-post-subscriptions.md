---
title: 创建订阅
description: 订阅侦听器应用程序，以在 Microsoft Graph 中的数据发生更改时接收通知。
localization_priority: Priority
author: piotrci
ms.openlocfilehash: 7b23968620abcb8f9a20e4a7b3598c21dec72980
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913883"
---
# <a name="create-subscription"></a><span data-ttu-id="d5a23-103">创建订阅</span><span class="sxs-lookup"><span data-stu-id="d5a23-103">Create subscription</span></span>

<span data-ttu-id="d5a23-104">订阅侦听器应用程序，以在 Microsoft Graph 中的数据发生更改时接收通知。</span><span class="sxs-lookup"><span data-stu-id="d5a23-104">Subscribes a listener application to receive notifications when data on the Microsoft Graph changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5a23-105">权限</span><span class="sxs-lookup"><span data-stu-id="d5a23-105">Permissions</span></span>

<span data-ttu-id="d5a23-p101">创建订阅需要读取资源范围。例如，若要获取通知消息，应用需要 `Mail.Read` 权限。下表列出了对各个资源所需权限的建议。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5a23-p101">Creating a subscription requires read scope to the resource. For example, to get notifications messages, your app needs the `Mail.Read` permission. The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d5a23-110">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="d5a23-110">Resource type / Item</span></span>        | <span data-ttu-id="d5a23-111">权限</span><span class="sxs-lookup"><span data-stu-id="d5a23-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="d5a23-112">联系人</span><span class="sxs-lookup"><span data-stu-id="d5a23-112">Contacts</span></span>                    | <span data-ttu-id="d5a23-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d5a23-113">Contacts.Read</span></span>       |
| <span data-ttu-id="d5a23-114">Conversations</span><span class="sxs-lookup"><span data-stu-id="d5a23-114">Conversations</span></span>               | <span data-ttu-id="d5a23-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5a23-115">Group.Read.All</span></span>      |
| <span data-ttu-id="d5a23-116">Events</span><span class="sxs-lookup"><span data-stu-id="d5a23-116">Events</span></span>                      | <span data-ttu-id="d5a23-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d5a23-117">Calendars.Read</span></span>      |
| <span data-ttu-id="d5a23-118">Messages</span><span class="sxs-lookup"><span data-stu-id="d5a23-118">Messages</span></span>                    | <span data-ttu-id="d5a23-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d5a23-119">Mail.Read</span></span>           |
| <span data-ttu-id="d5a23-120">组</span><span class="sxs-lookup"><span data-stu-id="d5a23-120">Groups</span></span>                      | <span data-ttu-id="d5a23-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5a23-121">Group.Read.All</span></span>      |
| <span data-ttu-id="d5a23-122">用户</span><span class="sxs-lookup"><span data-stu-id="d5a23-122">Users</span></span>                       | <span data-ttu-id="d5a23-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5a23-123">User.Read.All</span></span>       |
| <span data-ttu-id="d5a23-124">Drive（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="d5a23-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="d5a23-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d5a23-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="d5a23-126">驱动器 （共享的 SharePoint 内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="d5a23-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="d5a23-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5a23-127">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="d5a23-128">安全警报</span><span class="sxs-lookup"><span data-stu-id="d5a23-128">Security alert</span></span>| <span data-ttu-id="d5a23-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5a23-129">SecurityEvents.ReadWrite.All</span></span> |

 > <span data-ttu-id="d5a23-130">**注意：**/V1.0 终结点允许资源最多的应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="d5a23-130">**Note:** The /v1.0 endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="d5a23-131">应用程序权限不支持对话组和 OneDrive 驱动器根项目。</span><span class="sxs-lookup"><span data-stu-id="d5a23-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="d5a23-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5a23-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="d5a23-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5a23-133">Request headers</span></span>

| <span data-ttu-id="d5a23-134">名称</span><span class="sxs-lookup"><span data-stu-id="d5a23-134">Name</span></span>       | <span data-ttu-id="d5a23-135">类型</span><span class="sxs-lookup"><span data-stu-id="d5a23-135">Type</span></span> | <span data-ttu-id="d5a23-136">说明</span><span class="sxs-lookup"><span data-stu-id="d5a23-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d5a23-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5a23-137">Authorization</span></span>  | <span data-ttu-id="d5a23-138">string</span><span class="sxs-lookup"><span data-stu-id="d5a23-138">string</span></span>  | <span data-ttu-id="d5a23-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d5a23-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d5a23-141">响应</span><span class="sxs-lookup"><span data-stu-id="d5a23-141">Response</span></span>

<span data-ttu-id="d5a23-142">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d5a23-142">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5a23-143">示例</span><span class="sxs-lookup"><span data-stu-id="d5a23-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d5a23-144">请求</span><span class="sxs-lookup"><span data-stu-id="d5a23-144">Request</span></span>

<span data-ttu-id="d5a23-145">下面是在用户收到新邮件时请求发送通知的示例。</span><span class="sxs-lookup"><span data-stu-id="d5a23-145">Here is an example of the request to send a notification when the user receives a new mail.</span></span>
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

<span data-ttu-id="d5a23-146">在请求正文中，提供[订阅](../resources/subscription.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5a23-146">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="d5a23-147">`clientState`字段是可选的。</span><span class="sxs-lookup"><span data-stu-id="d5a23-147">The `clientState` field is optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="d5a23-148">资源示例</span><span class="sxs-lookup"><span data-stu-id="d5a23-148">Resources examples</span></span>

<span data-ttu-id="d5a23-149">订阅资源属性的有效值如下：</span><span class="sxs-lookup"><span data-stu-id="d5a23-149">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="d5a23-150">资源类型</span><span class="sxs-lookup"><span data-stu-id="d5a23-150">Resource type</span></span> | <span data-ttu-id="d5a23-151">示例</span><span class="sxs-lookup"><span data-stu-id="d5a23-151">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="d5a23-152">邮件</span><span class="sxs-lookup"><span data-stu-id="d5a23-152">Mail</span></span>|<span data-ttu-id="d5a23-153">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="d5a23-153">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="d5a23-154">me/messages</span><span class="sxs-lookup"><span data-stu-id="d5a23-154">me/messages</span></span>|
|<span data-ttu-id="d5a23-155">联系人</span><span class="sxs-lookup"><span data-stu-id="d5a23-155">Contacts</span></span>|<span data-ttu-id="d5a23-156">me/contacts</span><span class="sxs-lookup"><span data-stu-id="d5a23-156">me/contacts</span></span>|
|<span data-ttu-id="d5a23-157">日历</span><span class="sxs-lookup"><span data-stu-id="d5a23-157">Calendars</span></span>|<span data-ttu-id="d5a23-158">me/events</span><span class="sxs-lookup"><span data-stu-id="d5a23-158">me/events</span></span>|
|<span data-ttu-id="d5a23-159">用户</span><span class="sxs-lookup"><span data-stu-id="d5a23-159">Users</span></span>|<span data-ttu-id="d5a23-160">users</span><span class="sxs-lookup"><span data-stu-id="d5a23-160">users</span></span>|
|<span data-ttu-id="d5a23-161">组</span><span class="sxs-lookup"><span data-stu-id="d5a23-161">Groups</span></span>|<span data-ttu-id="d5a23-162">组</span><span class="sxs-lookup"><span data-stu-id="d5a23-162">groups</span></span>|
|<span data-ttu-id="d5a23-163">对话</span><span class="sxs-lookup"><span data-stu-id="d5a23-163">Conversations</span></span>|<span data-ttu-id="d5a23-164">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="d5a23-164">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="d5a23-165">驱动器</span><span class="sxs-lookup"><span data-stu-id="d5a23-165">Drives</span></span>|<span data-ttu-id="d5a23-166">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="d5a23-166">me/drive/root</span></span>|
|<span data-ttu-id="d5a23-167">安全警报</span><span class="sxs-lookup"><span data-stu-id="d5a23-167">Security alert</span></span>|<span data-ttu-id="d5a23-168">安全/警告？ $filter = 状态 eq 新建</span><span class="sxs-lookup"><span data-stu-id="d5a23-168">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="d5a23-169">响应</span><span class="sxs-lookup"><span data-stu-id="d5a23-169">Response</span></span>

<span data-ttu-id="d5a23-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d5a23-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="d5a23-173">通知终结点验证</span><span class="sxs-lookup"><span data-stu-id="d5a23-173">Notification endpoint validation</span></span>

<span data-ttu-id="d5a23-174">订阅通知终结点 (中指定`notificationUrl`属性) 必须能够响应验证请求，[设置的用户数据更改的通知](/graph/webhooks#notification-endpoint-validation)中所述。</span><span class="sxs-lookup"><span data-stu-id="d5a23-174">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="d5a23-175">如果验证失败，请求创建订阅，将返回一个 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="d5a23-175">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
