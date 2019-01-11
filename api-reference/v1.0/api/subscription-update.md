---
title: 更新订阅
description: 通过延长到期时间续订订阅。
localization_priority: Normal
ms.openlocfilehash: f0804421c2e178d176975317ba82bb0aac0ae212
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809714"
---
# <a name="update-subscription"></a><span data-ttu-id="70a04-103">更新订阅</span><span class="sxs-lookup"><span data-stu-id="70a04-103">Update subscription</span></span>

<span data-ttu-id="70a04-104">通过延长到期时间续订订阅。</span><span class="sxs-lookup"><span data-stu-id="70a04-104">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="70a04-105">订阅过期后一个随资源类型的时间长度。</span><span class="sxs-lookup"><span data-stu-id="70a04-105">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="70a04-106">为了避免丢失通知，应用程序应更新其订阅之前其到期日期。</span><span class="sxs-lookup"><span data-stu-id="70a04-106">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="70a04-107">请参阅最大长度为每个资源类型订阅的[订阅](../resources/subscription.md)。</span><span class="sxs-lookup"><span data-stu-id="70a04-107">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="70a04-108">权限</span><span class="sxs-lookup"><span data-stu-id="70a04-108">Permissions</span></span>

<span data-ttu-id="70a04-p102">下表列出了对各个资源所需权限的建议。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70a04-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="70a04-111">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="70a04-111">Resource type / Item</span></span>        | <span data-ttu-id="70a04-112">权限</span><span class="sxs-lookup"><span data-stu-id="70a04-112">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="70a04-113">联系人</span><span class="sxs-lookup"><span data-stu-id="70a04-113">Contacts</span></span>                    | <span data-ttu-id="70a04-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="70a04-114">Contacts.Read</span></span>       |
| <span data-ttu-id="70a04-115">Conversations</span><span class="sxs-lookup"><span data-stu-id="70a04-115">Conversations</span></span>               | <span data-ttu-id="70a04-116">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="70a04-116">Group.Read.All</span></span>      |
| <span data-ttu-id="70a04-117">Events</span><span class="sxs-lookup"><span data-stu-id="70a04-117">Events</span></span>                      | <span data-ttu-id="70a04-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="70a04-118">Calendars.Read</span></span>      |
| <span data-ttu-id="70a04-119">Messages</span><span class="sxs-lookup"><span data-stu-id="70a04-119">Messages</span></span>                    | <span data-ttu-id="70a04-120">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="70a04-120">Mail.Read</span></span>           |
| <span data-ttu-id="70a04-121">组</span><span class="sxs-lookup"><span data-stu-id="70a04-121">Groups</span></span>                      | <span data-ttu-id="70a04-122">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="70a04-122">Group.Read.All</span></span>      |
| <span data-ttu-id="70a04-123">用户</span><span class="sxs-lookup"><span data-stu-id="70a04-123">Users</span></span>                       | <span data-ttu-id="70a04-124">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="70a04-124">User.Read.All</span></span>       |
| <span data-ttu-id="70a04-125">Drive（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="70a04-125">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="70a04-126">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70a04-126">Files.ReadWrite</span></span>     |
| <span data-ttu-id="70a04-127">驱动器 （共享的 SharePoint 内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="70a04-127">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="70a04-128">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70a04-128">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="70a04-129">安全警报</span><span class="sxs-lookup"><span data-stu-id="70a04-129">Security alert</span></span>| <span data-ttu-id="70a04-130">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70a04-130">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70a04-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70a04-131">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="70a04-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="70a04-132">Request headers</span></span>

| <span data-ttu-id="70a04-133">名称</span><span class="sxs-lookup"><span data-stu-id="70a04-133">Name</span></span>       | <span data-ttu-id="70a04-134">类型</span><span class="sxs-lookup"><span data-stu-id="70a04-134">Type</span></span> | <span data-ttu-id="70a04-135">说明</span><span class="sxs-lookup"><span data-stu-id="70a04-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="70a04-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="70a04-136">Authorization</span></span>  | <span data-ttu-id="70a04-137">string</span><span class="sxs-lookup"><span data-stu-id="70a04-137">string</span></span>  | <span data-ttu-id="70a04-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="70a04-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="70a04-140">响应</span><span class="sxs-lookup"><span data-stu-id="70a04-140">Response</span></span>

<span data-ttu-id="70a04-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="70a04-141">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70a04-142">示例</span><span class="sxs-lookup"><span data-stu-id="70a04-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="70a04-143">请求</span><span class="sxs-lookup"><span data-stu-id="70a04-143">Request</span></span>

<span data-ttu-id="70a04-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="70a04-144">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="70a04-145">响应</span><span class="sxs-lookup"><span data-stu-id="70a04-145">Response</span></span>

<span data-ttu-id="70a04-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="70a04-146">Here is an example of the response.</span></span>
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
