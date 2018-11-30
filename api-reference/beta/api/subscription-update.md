---
title: 更新订阅
description: 通过延长到期时间续订订阅。
ms.openlocfilehash: e2021e22d84ad9e05429db7980d37cbd1574843c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043404"
---
# <a name="update-subscription"></a><span data-ttu-id="bf33c-103">更新订阅</span><span class="sxs-lookup"><span data-stu-id="bf33c-103">Update subscription</span></span>

> <span data-ttu-id="bf33c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bf33c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf33c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bf33c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bf33c-106">通过延长到期时间续订订阅。</span><span class="sxs-lookup"><span data-stu-id="bf33c-106">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="bf33c-107">订阅过期后一个随资源类型的时间长度。</span><span class="sxs-lookup"><span data-stu-id="bf33c-107">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="bf33c-108">为了避免丢失通知，应用程序应更新其订阅之前其到期日期。</span><span class="sxs-lookup"><span data-stu-id="bf33c-108">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="bf33c-109">请参阅最大长度为每个资源类型订阅的[订阅](../resources/subscription.md)。</span><span class="sxs-lookup"><span data-stu-id="bf33c-109">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf33c-110">权限</span><span class="sxs-lookup"><span data-stu-id="bf33c-110">Permissions</span></span>

<span data-ttu-id="bf33c-p103">下表列出了对各个资源所需权限的建议。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bf33c-p103">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bf33c-113">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="bf33c-113">Resource type / Item</span></span>        | <span data-ttu-id="bf33c-114">权限</span><span class="sxs-lookup"><span data-stu-id="bf33c-114">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="bf33c-115">联系人</span><span class="sxs-lookup"><span data-stu-id="bf33c-115">Contacts</span></span>                    | <span data-ttu-id="bf33c-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="bf33c-116">Contacts.Read</span></span>       |
| <span data-ttu-id="bf33c-117">Conversations</span><span class="sxs-lookup"><span data-stu-id="bf33c-117">Conversations</span></span>               | <span data-ttu-id="bf33c-118">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf33c-118">Group.Read.All</span></span>      |
| <span data-ttu-id="bf33c-119">Events</span><span class="sxs-lookup"><span data-stu-id="bf33c-119">Events</span></span>                      | <span data-ttu-id="bf33c-120">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bf33c-120">Calendars.Read</span></span>      |
| <span data-ttu-id="bf33c-121">Messages</span><span class="sxs-lookup"><span data-stu-id="bf33c-121">Messages</span></span>                    | <span data-ttu-id="bf33c-122">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bf33c-122">Mail.Read</span></span>           |
| <span data-ttu-id="bf33c-123">Groups</span><span class="sxs-lookup"><span data-stu-id="bf33c-123">Groups</span></span>                      | <span data-ttu-id="bf33c-124">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf33c-124">Group.Read.All</span></span>      |
| <span data-ttu-id="bf33c-125">Users</span><span class="sxs-lookup"><span data-stu-id="bf33c-125">Users</span></span>                       | <span data-ttu-id="bf33c-126">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf33c-126">User.Read.All</span></span>       |
| <span data-ttu-id="bf33c-127">Drive（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="bf33c-127">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="bf33c-128">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf33c-128">Files.ReadWrite</span></span>     |
| <span data-ttu-id="bf33c-129">驱动器 （共享的 SharePoint 内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="bf33c-129">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="bf33c-130">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf33c-130">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="bf33c-131">安全警报</span><span class="sxs-lookup"><span data-stu-id="bf33c-131">Security alert</span></span>               | <span data-ttu-id="bf33c-132">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf33c-132">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="bf33c-133">***注意：***/Beta 终结点允许资源最多的应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="bf33c-133">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="bf33c-134">应用程序权限不支持对话组和 OneDrive 驱动器根项目。</span><span class="sxs-lookup"><span data-stu-id="bf33c-134">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="bf33c-135">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf33c-135">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bf33c-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="bf33c-136">Request headers</span></span>

| <span data-ttu-id="bf33c-137">名称</span><span class="sxs-lookup"><span data-stu-id="bf33c-137">Name</span></span>       | <span data-ttu-id="bf33c-138">类型</span><span class="sxs-lookup"><span data-stu-id="bf33c-138">Type</span></span> | <span data-ttu-id="bf33c-139">说明</span><span class="sxs-lookup"><span data-stu-id="bf33c-139">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bf33c-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf33c-140">Authorization</span></span>  | <span data-ttu-id="bf33c-141">string</span><span class="sxs-lookup"><span data-stu-id="bf33c-141">string</span></span>  | <span data-ttu-id="bf33c-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bf33c-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="bf33c-144">响应</span><span class="sxs-lookup"><span data-stu-id="bf33c-144">Response</span></span>

<span data-ttu-id="bf33c-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bf33c-145">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf33c-146">示例</span><span class="sxs-lookup"><span data-stu-id="bf33c-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bf33c-147">请求</span><span class="sxs-lookup"><span data-stu-id="bf33c-147">Request</span></span>

<span data-ttu-id="bf33c-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bf33c-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/beta/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a><span data-ttu-id="bf33c-149">响应</span><span class="sxs-lookup"><span data-stu-id="bf33c-149">Response</span></span>

<span data-ttu-id="bf33c-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="bf33c-150">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
