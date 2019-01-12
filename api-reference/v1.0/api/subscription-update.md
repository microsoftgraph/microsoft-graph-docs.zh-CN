---
title: 更新订阅
description: 通过延长到期时间续订订阅。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: a980d1fdc50a3295a309ccb1d58c0ebf5b5b6133
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976630"
---
# <a name="update-subscription"></a><span data-ttu-id="0e6e9-103">更新订阅</span><span class="sxs-lookup"><span data-stu-id="0e6e9-103">Update subscription</span></span>

<span data-ttu-id="0e6e9-104">通过延长到期时间续订订阅。</span><span class="sxs-lookup"><span data-stu-id="0e6e9-104">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="0e6e9-105">订阅过期后一个随资源类型的时间长度。</span><span class="sxs-lookup"><span data-stu-id="0e6e9-105">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="0e6e9-106">为了避免丢失通知，应用程序应更新其订阅之前其到期日期。</span><span class="sxs-lookup"><span data-stu-id="0e6e9-106">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="0e6e9-107">请参阅最大长度为每个资源类型订阅的[订阅](../resources/subscription.md)。</span><span class="sxs-lookup"><span data-stu-id="0e6e9-107">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e6e9-108">权限</span><span class="sxs-lookup"><span data-stu-id="0e6e9-108">Permissions</span></span>

<span data-ttu-id="0e6e9-p102">下表列出了对各个资源所需权限的建议。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e6e9-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0e6e9-111">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="0e6e9-111">Resource type / Item</span></span>        | <span data-ttu-id="0e6e9-112">权限</span><span class="sxs-lookup"><span data-stu-id="0e6e9-112">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="0e6e9-113">联系人</span><span class="sxs-lookup"><span data-stu-id="0e6e9-113">Contacts</span></span>                    | <span data-ttu-id="0e6e9-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="0e6e9-114">Contacts.Read</span></span>       |
| <span data-ttu-id="0e6e9-115">Conversations</span><span class="sxs-lookup"><span data-stu-id="0e6e9-115">Conversations</span></span>               | <span data-ttu-id="0e6e9-116">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e6e9-116">Group.Read.All</span></span>      |
| <span data-ttu-id="0e6e9-117">Events</span><span class="sxs-lookup"><span data-stu-id="0e6e9-117">Events</span></span>                      | <span data-ttu-id="0e6e9-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0e6e9-118">Calendars.Read</span></span>      |
| <span data-ttu-id="0e6e9-119">Messages</span><span class="sxs-lookup"><span data-stu-id="0e6e9-119">Messages</span></span>                    | <span data-ttu-id="0e6e9-120">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0e6e9-120">Mail.Read</span></span>           |
| <span data-ttu-id="0e6e9-121">组</span><span class="sxs-lookup"><span data-stu-id="0e6e9-121">Groups</span></span>                      | <span data-ttu-id="0e6e9-122">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e6e9-122">Group.Read.All</span></span>      |
| <span data-ttu-id="0e6e9-123">用户</span><span class="sxs-lookup"><span data-stu-id="0e6e9-123">Users</span></span>                       | <span data-ttu-id="0e6e9-124">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e6e9-124">User.Read.All</span></span>       |
| <span data-ttu-id="0e6e9-125">Drive（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="0e6e9-125">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="0e6e9-126">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e6e9-126">Files.ReadWrite</span></span>     |
| <span data-ttu-id="0e6e9-127">驱动器 （共享的 SharePoint 内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="0e6e9-127">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="0e6e9-128">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e6e9-128">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="0e6e9-129">安全警报</span><span class="sxs-lookup"><span data-stu-id="0e6e9-129">Security alert</span></span>| <span data-ttu-id="0e6e9-130">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e6e9-130">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e6e9-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e6e9-131">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0e6e9-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e6e9-132">Request headers</span></span>

| <span data-ttu-id="0e6e9-133">名称</span><span class="sxs-lookup"><span data-stu-id="0e6e9-133">Name</span></span>       | <span data-ttu-id="0e6e9-134">类型</span><span class="sxs-lookup"><span data-stu-id="0e6e9-134">Type</span></span> | <span data-ttu-id="0e6e9-135">说明</span><span class="sxs-lookup"><span data-stu-id="0e6e9-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0e6e9-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e6e9-136">Authorization</span></span>  | <span data-ttu-id="0e6e9-137">string</span><span class="sxs-lookup"><span data-stu-id="0e6e9-137">string</span></span>  | <span data-ttu-id="0e6e9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0e6e9-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0e6e9-140">响应</span><span class="sxs-lookup"><span data-stu-id="0e6e9-140">Response</span></span>

<span data-ttu-id="0e6e9-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0e6e9-141">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e6e9-142">示例</span><span class="sxs-lookup"><span data-stu-id="0e6e9-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0e6e9-143">请求</span><span class="sxs-lookup"><span data-stu-id="0e6e9-143">Request</span></span>

<span data-ttu-id="0e6e9-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0e6e9-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a><span data-ttu-id="0e6e9-145">响应</span><span class="sxs-lookup"><span data-stu-id="0e6e9-145">Response</span></span>

<span data-ttu-id="0e6e9-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0e6e9-146">Here is an example of the response.</span></span>
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
  "clientState":"subscription-identifier",
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
