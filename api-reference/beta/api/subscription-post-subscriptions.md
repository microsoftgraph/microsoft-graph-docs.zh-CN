---
title: 创建订阅
description: 订阅侦听器应用程序上的 Microsoft Graph 资源的数据更改时收到通知。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 002dd88c7db2650be2303e7df6f86ce9a5fbdaa9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527575"
---
# <a name="create-subscription"></a><span data-ttu-id="14a06-103">创建订阅</span><span class="sxs-lookup"><span data-stu-id="14a06-103">Create subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14a06-104">订阅侦听器应用程序上的 Microsoft Graph 资源的数据更改时收到通知。</span><span class="sxs-lookup"><span data-stu-id="14a06-104">Subscribes a listener application to receive notifications when data on a Microsoft Graph resource changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="14a06-105">权限</span><span class="sxs-lookup"><span data-stu-id="14a06-105">Permissions</span></span>

<span data-ttu-id="14a06-106">创建订阅需要应用程序将为其接收通知的资源的读取的权限。</span><span class="sxs-lookup"><span data-stu-id="14a06-106">Creating a subscription requires read permission to the resource for which the app will receive notifications.</span></span> <span data-ttu-id="14a06-107">例如，若要获取有关邮件的通知，您的应用程序需要`Mail.Read`权限。</span><span class="sxs-lookup"><span data-stu-id="14a06-107">For example, to get notifications about Messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="14a06-108">下表列出了对各个资源所需权限的建议。</span><span class="sxs-lookup"><span data-stu-id="14a06-108">The following table lists the suggested permission needed for each resource.</span></span> <span data-ttu-id="14a06-109">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14a06-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="14a06-110">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="14a06-110">Resource type / Item</span></span>        | <span data-ttu-id="14a06-111">权限</span><span class="sxs-lookup"><span data-stu-id="14a06-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="14a06-112">联系人</span><span class="sxs-lookup"><span data-stu-id="14a06-112">Contacts</span></span>                    | <span data-ttu-id="14a06-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="14a06-113">Contacts.Read</span></span>       |
| <span data-ttu-id="14a06-114">Conversations</span><span class="sxs-lookup"><span data-stu-id="14a06-114">Conversations</span></span>               | <span data-ttu-id="14a06-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="14a06-115">Group.Read.All</span></span>      |
| <span data-ttu-id="14a06-116">Events</span><span class="sxs-lookup"><span data-stu-id="14a06-116">Events</span></span>                      | <span data-ttu-id="14a06-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="14a06-117">Calendars.Read</span></span>      |
| <span data-ttu-id="14a06-118">Messages</span><span class="sxs-lookup"><span data-stu-id="14a06-118">Messages</span></span>                    | <span data-ttu-id="14a06-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="14a06-119">Mail.Read</span></span>           |
| <span data-ttu-id="14a06-120">组</span><span class="sxs-lookup"><span data-stu-id="14a06-120">Groups</span></span>                      | <span data-ttu-id="14a06-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="14a06-121">Group.Read.All</span></span>      |
| <span data-ttu-id="14a06-122">用户</span><span class="sxs-lookup"><span data-stu-id="14a06-122">Users</span></span>                       | <span data-ttu-id="14a06-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="14a06-123">User.Read.All</span></span>       |
| <span data-ttu-id="14a06-124">Drive（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="14a06-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="14a06-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14a06-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="14a06-126">驱动器 （共享的 SharePoint 内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="14a06-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="14a06-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a06-127">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="14a06-128">安全警报</span><span class="sxs-lookup"><span data-stu-id="14a06-128">Security alert</span></span>              | <span data-ttu-id="14a06-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a06-129">SecurityEvents.ReadWrite.All</span></span> |

> <span data-ttu-id="14a06-130">**注意：**/Beta 终结点允许资源最多的应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="14a06-130">**Note:** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="14a06-131">应用程序权限不支持对话组和 OneDrive 驱动器根项目。</span><span class="sxs-lookup"><span data-stu-id="14a06-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="14a06-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14a06-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="14a06-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="14a06-133">Request headers</span></span>

| <span data-ttu-id="14a06-134">名称</span><span class="sxs-lookup"><span data-stu-id="14a06-134">Name</span></span>       | <span data-ttu-id="14a06-135">类型</span><span class="sxs-lookup"><span data-stu-id="14a06-135">Type</span></span> | <span data-ttu-id="14a06-136">说明</span><span class="sxs-lookup"><span data-stu-id="14a06-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="14a06-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="14a06-137">Authorization</span></span>  | <span data-ttu-id="14a06-138">string</span><span class="sxs-lookup"><span data-stu-id="14a06-138">string</span></span>  | <span data-ttu-id="14a06-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="14a06-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="14a06-141">响应</span><span class="sxs-lookup"><span data-stu-id="14a06-141">Response</span></span>

<span data-ttu-id="14a06-142">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="14a06-142">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14a06-143">示例</span><span class="sxs-lookup"><span data-stu-id="14a06-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="14a06-144">请求</span><span class="sxs-lookup"><span data-stu-id="14a06-144">Request</span></span>

<span data-ttu-id="14a06-145">在请求正文中，提供[订阅](../resources/subscription.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14a06-145">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="14a06-146">`clientState`字段是可选的。</span><span class="sxs-lookup"><span data-stu-id="14a06-146">The `clientState` field is optional.</span></span>

<span data-ttu-id="14a06-147">此示例请求创建有关当前登录用户接收的新邮件通知的订阅。</span><span class="sxs-lookup"><span data-stu-id="14a06-147">This sample request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>
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

<span data-ttu-id="14a06-148">资源属性的有效值如下：</span><span class="sxs-lookup"><span data-stu-id="14a06-148">The following are valid values for the resource property:</span></span>

| <span data-ttu-id="14a06-149">资源类型</span><span class="sxs-lookup"><span data-stu-id="14a06-149">Resource type</span></span> | <span data-ttu-id="14a06-150">示例</span><span class="sxs-lookup"><span data-stu-id="14a06-150">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="14a06-151">邮件</span><span class="sxs-lookup"><span data-stu-id="14a06-151">Mail</span></span>|<span data-ttu-id="14a06-152">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="14a06-152">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="14a06-153">me/messages</span><span class="sxs-lookup"><span data-stu-id="14a06-153">me/messages</span></span>|
|<span data-ttu-id="14a06-154">联系人</span><span class="sxs-lookup"><span data-stu-id="14a06-154">Contacts</span></span>|<span data-ttu-id="14a06-155">me/contacts</span><span class="sxs-lookup"><span data-stu-id="14a06-155">me/contacts</span></span>|
|<span data-ttu-id="14a06-156">日历</span><span class="sxs-lookup"><span data-stu-id="14a06-156">Calendars</span></span>|<span data-ttu-id="14a06-157">me/events</span><span class="sxs-lookup"><span data-stu-id="14a06-157">me/events</span></span>|
|<span data-ttu-id="14a06-158">用户</span><span class="sxs-lookup"><span data-stu-id="14a06-158">Users</span></span>|<span data-ttu-id="14a06-159">users</span><span class="sxs-lookup"><span data-stu-id="14a06-159">users</span></span>|
|<span data-ttu-id="14a06-160">组</span><span class="sxs-lookup"><span data-stu-id="14a06-160">Groups</span></span>|<span data-ttu-id="14a06-161">组</span><span class="sxs-lookup"><span data-stu-id="14a06-161">groups</span></span>|
|<span data-ttu-id="14a06-162">对话</span><span class="sxs-lookup"><span data-stu-id="14a06-162">Conversations</span></span>|<span data-ttu-id="14a06-163">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="14a06-163">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="14a06-164">驱动器</span><span class="sxs-lookup"><span data-stu-id="14a06-164">Drives</span></span>|<span data-ttu-id="14a06-165">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="14a06-165">me/drive/root</span></span>|
|<span data-ttu-id="14a06-166">安全警报</span><span class="sxs-lookup"><span data-stu-id="14a06-166">Security alert</span></span>|<span data-ttu-id="14a06-167">安全/警告？ $filter = 状态 eq 新建</span><span class="sxs-lookup"><span data-stu-id="14a06-167">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="14a06-168">响应</span><span class="sxs-lookup"><span data-stu-id="14a06-168">Response</span></span>

<span data-ttu-id="14a06-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="14a06-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="14a06-172">通知终结点验证</span><span class="sxs-lookup"><span data-stu-id="14a06-172">Notification endpoint validation</span></span>

<span data-ttu-id="14a06-173">订阅通知终结点 (中指定`notificationUrl`属性) 必须能够响应验证请求，[设置的用户数据更改的通知](/graph/webhooks#notification-endpoint-validation)中所述。</span><span class="sxs-lookup"><span data-stu-id="14a06-173">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="14a06-174">如果验证失败，请求创建订阅，将返回一个 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="14a06-174">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
    "Error: /api-reference/beta/api/subscription-post-subscriptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
