---
title: 创建订阅
description: 订阅侦听器应用程序上的 Microsoft Graph 资源的数据更改时收到通知。
localization_priority: Normal
ms.openlocfilehash: 5b7f465e556d1fb752bcb2d3c962fd6444d462c5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805052"
---
# <a name="create-subscription"></a><span data-ttu-id="641a7-103">创建订阅</span><span class="sxs-lookup"><span data-stu-id="641a7-103">Create subscription</span></span>

> <span data-ttu-id="641a7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="641a7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="641a7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="641a7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="641a7-106">订阅侦听器应用程序上的 Microsoft Graph 资源的数据更改时收到通知。</span><span class="sxs-lookup"><span data-stu-id="641a7-106">Subscribes a listener application to receive notifications when data on a Microsoft Graph resource changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="641a7-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="641a7-107">Permissions</span></span>

<span data-ttu-id="641a7-108">创建订阅需要应用程序将为其接收通知的资源的读取的权限。</span><span class="sxs-lookup"><span data-stu-id="641a7-108">Creating a subscription requires read permission to the resource for which the app will receive notifications.</span></span> <span data-ttu-id="641a7-109">例如，若要获取有关邮件的通知，您的应用程序需要`Mail.Read`权限。</span><span class="sxs-lookup"><span data-stu-id="641a7-109">For example, to get notifications about Messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="641a7-110">下表列出了对各个资源所需权限的建议。</span><span class="sxs-lookup"><span data-stu-id="641a7-110">The following table lists the suggested permission needed for each resource.</span></span> <span data-ttu-id="641a7-111">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="641a7-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="641a7-112">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="641a7-112">Resource type / Item</span></span>        | <span data-ttu-id="641a7-113">权限</span><span class="sxs-lookup"><span data-stu-id="641a7-113">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="641a7-114">联系人</span><span class="sxs-lookup"><span data-stu-id="641a7-114">Contacts</span></span>                    | <span data-ttu-id="641a7-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="641a7-115">Contacts.Read</span></span>       |
| <span data-ttu-id="641a7-116">Conversations</span><span class="sxs-lookup"><span data-stu-id="641a7-116">Conversations</span></span>               | <span data-ttu-id="641a7-117">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="641a7-117">Group.Read.All</span></span>      |
| <span data-ttu-id="641a7-118">Events</span><span class="sxs-lookup"><span data-stu-id="641a7-118">Events</span></span>                      | <span data-ttu-id="641a7-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="641a7-119">Calendars.Read</span></span>      |
| <span data-ttu-id="641a7-120">Messages</span><span class="sxs-lookup"><span data-stu-id="641a7-120">Messages</span></span>                    | <span data-ttu-id="641a7-121">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="641a7-121">Mail.Read</span></span>           |
| <span data-ttu-id="641a7-122">组</span><span class="sxs-lookup"><span data-stu-id="641a7-122">Groups</span></span>                      | <span data-ttu-id="641a7-123">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="641a7-123">Group.Read.All</span></span>      |
| <span data-ttu-id="641a7-124">用户</span><span class="sxs-lookup"><span data-stu-id="641a7-124">Users</span></span>                       | <span data-ttu-id="641a7-125">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="641a7-125">User.Read.All</span></span>       |
| <span data-ttu-id="641a7-126">Drive（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="641a7-126">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="641a7-127">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="641a7-127">Files.ReadWrite</span></span>     |
| <span data-ttu-id="641a7-128">驱动器 （共享的 SharePoint 内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="641a7-128">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="641a7-129">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="641a7-129">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="641a7-130">安全警报</span><span class="sxs-lookup"><span data-stu-id="641a7-130">Security alert</span></span>              | <span data-ttu-id="641a7-131">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="641a7-131">SecurityEvents.ReadWrite.All</span></span> |

> <span data-ttu-id="641a7-132">**注意：**/Beta 终结点允许资源最多的应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="641a7-132">**Note:** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="641a7-133">应用程序权限不支持对话组和 OneDrive 驱动器根项目。</span><span class="sxs-lookup"><span data-stu-id="641a7-133">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="641a7-134">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="641a7-134">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="641a7-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="641a7-135">Request headers</span></span>

| <span data-ttu-id="641a7-136">名称</span><span class="sxs-lookup"><span data-stu-id="641a7-136">Name</span></span>       | <span data-ttu-id="641a7-137">类型</span><span class="sxs-lookup"><span data-stu-id="641a7-137">Type</span></span> | <span data-ttu-id="641a7-138">说明</span><span class="sxs-lookup"><span data-stu-id="641a7-138">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="641a7-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="641a7-139">Authorization</span></span>  | <span data-ttu-id="641a7-140">string</span><span class="sxs-lookup"><span data-stu-id="641a7-140">string</span></span>  | <span data-ttu-id="641a7-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="641a7-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="641a7-143">响应</span><span class="sxs-lookup"><span data-stu-id="641a7-143">Response</span></span>

<span data-ttu-id="641a7-144">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="641a7-144">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="641a7-145">示例</span><span class="sxs-lookup"><span data-stu-id="641a7-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="641a7-146">请求</span><span class="sxs-lookup"><span data-stu-id="641a7-146">Request</span></span>

<span data-ttu-id="641a7-147">在请求正文中，提供[订阅](../resources/subscription.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="641a7-147">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="641a7-148">`clientState`字段是可选的。</span><span class="sxs-lookup"><span data-stu-id="641a7-148">The `clientState` field is optional.</span></span>

<span data-ttu-id="641a7-149">此示例请求创建有关当前登录用户接收的新邮件通知的订阅。</span><span class="sxs-lookup"><span data-stu-id="641a7-149">This sample request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>
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

<span data-ttu-id="641a7-150">资源属性的有效值如下：</span><span class="sxs-lookup"><span data-stu-id="641a7-150">The following are valid values for the resource property:</span></span>

| <span data-ttu-id="641a7-151">资源类型</span><span class="sxs-lookup"><span data-stu-id="641a7-151">Resource type</span></span> | <span data-ttu-id="641a7-152">示例</span><span class="sxs-lookup"><span data-stu-id="641a7-152">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="641a7-153">邮件</span><span class="sxs-lookup"><span data-stu-id="641a7-153">Mail</span></span>|<span data-ttu-id="641a7-154">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="641a7-154">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="641a7-155">me/messages</span><span class="sxs-lookup"><span data-stu-id="641a7-155">me/messages</span></span>|
|<span data-ttu-id="641a7-156">联系人</span><span class="sxs-lookup"><span data-stu-id="641a7-156">Contacts</span></span>|<span data-ttu-id="641a7-157">me/contacts</span><span class="sxs-lookup"><span data-stu-id="641a7-157">me/contacts</span></span>|
|<span data-ttu-id="641a7-158">日历</span><span class="sxs-lookup"><span data-stu-id="641a7-158">Calendars</span></span>|<span data-ttu-id="641a7-159">me/events</span><span class="sxs-lookup"><span data-stu-id="641a7-159">me/events</span></span>|
|<span data-ttu-id="641a7-160">用户</span><span class="sxs-lookup"><span data-stu-id="641a7-160">Users</span></span>|<span data-ttu-id="641a7-161">users</span><span class="sxs-lookup"><span data-stu-id="641a7-161">users</span></span>|
|<span data-ttu-id="641a7-162">组</span><span class="sxs-lookup"><span data-stu-id="641a7-162">Groups</span></span>|<span data-ttu-id="641a7-163">组</span><span class="sxs-lookup"><span data-stu-id="641a7-163">groups</span></span>|
|<span data-ttu-id="641a7-164">对话</span><span class="sxs-lookup"><span data-stu-id="641a7-164">Conversations</span></span>|<span data-ttu-id="641a7-165">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="641a7-165">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="641a7-166">驱动器</span><span class="sxs-lookup"><span data-stu-id="641a7-166">Drives</span></span>|<span data-ttu-id="641a7-167">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="641a7-167">me/drive/root</span></span>|
|<span data-ttu-id="641a7-168">安全警报</span><span class="sxs-lookup"><span data-stu-id="641a7-168">Security alert</span></span>|<span data-ttu-id="641a7-169">安全/警告？ $filter = 状态 eq 新建</span><span class="sxs-lookup"><span data-stu-id="641a7-169">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="641a7-170">响应</span><span class="sxs-lookup"><span data-stu-id="641a7-170">Response</span></span>

<span data-ttu-id="641a7-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="641a7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="641a7-174">通知终结点验证</span><span class="sxs-lookup"><span data-stu-id="641a7-174">Notification endpoint validation</span></span>

<span data-ttu-id="641a7-175">订阅通知终结点 (中指定`notificationUrl`属性) 必须能够响应验证请求，[设置的用户数据更改的通知](/graph/webhooks#notification-endpoint-validation)中所述。</span><span class="sxs-lookup"><span data-stu-id="641a7-175">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="641a7-176">如果验证失败，请求创建订阅，将返回一个 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="641a7-176">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
