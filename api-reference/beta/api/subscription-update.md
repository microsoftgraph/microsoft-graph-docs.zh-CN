---
title: 更新订阅
description: 通过延长到期时间续订订阅。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 19355ff8acbcdade689b140abca63e8d9885e3fc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512778"
---
# <a name="update-subscription"></a><span data-ttu-id="1a3cc-103">更新订阅</span><span class="sxs-lookup"><span data-stu-id="1a3cc-103">Update subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a3cc-104">通过延长到期时间续订订阅。</span><span class="sxs-lookup"><span data-stu-id="1a3cc-104">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="1a3cc-105">订阅过期后一个随资源类型的时间长度。</span><span class="sxs-lookup"><span data-stu-id="1a3cc-105">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="1a3cc-106">为了避免丢失通知，应用程序应更新其订阅之前其到期日期。</span><span class="sxs-lookup"><span data-stu-id="1a3cc-106">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="1a3cc-107">请参阅最大长度为每个资源类型订阅的[订阅](../resources/subscription.md)。</span><span class="sxs-lookup"><span data-stu-id="1a3cc-107">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a3cc-108">权限</span><span class="sxs-lookup"><span data-stu-id="1a3cc-108">Permissions</span></span>

<span data-ttu-id="1a3cc-p102">下表列出了对各个资源所需权限的建议。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a3cc-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1a3cc-111">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="1a3cc-111">Resource type / Item</span></span>        | <span data-ttu-id="1a3cc-112">权限</span><span class="sxs-lookup"><span data-stu-id="1a3cc-112">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="1a3cc-113">联系人</span><span class="sxs-lookup"><span data-stu-id="1a3cc-113">Contacts</span></span>                    | <span data-ttu-id="1a3cc-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1a3cc-114">Contacts.Read</span></span>       |
| <span data-ttu-id="1a3cc-115">Conversations</span><span class="sxs-lookup"><span data-stu-id="1a3cc-115">Conversations</span></span>               | <span data-ttu-id="1a3cc-116">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a3cc-116">Group.Read.All</span></span>      |
| <span data-ttu-id="1a3cc-117">Events</span><span class="sxs-lookup"><span data-stu-id="1a3cc-117">Events</span></span>                      | <span data-ttu-id="1a3cc-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1a3cc-118">Calendars.Read</span></span>      |
| <span data-ttu-id="1a3cc-119">Messages</span><span class="sxs-lookup"><span data-stu-id="1a3cc-119">Messages</span></span>                    | <span data-ttu-id="1a3cc-120">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1a3cc-120">Mail.Read</span></span>           |
| <span data-ttu-id="1a3cc-121">组</span><span class="sxs-lookup"><span data-stu-id="1a3cc-121">Groups</span></span>                      | <span data-ttu-id="1a3cc-122">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a3cc-122">Group.Read.All</span></span>      |
| <span data-ttu-id="1a3cc-123">用户</span><span class="sxs-lookup"><span data-stu-id="1a3cc-123">Users</span></span>                       | <span data-ttu-id="1a3cc-124">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a3cc-124">User.Read.All</span></span>       |
| <span data-ttu-id="1a3cc-125">Drive（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="1a3cc-125">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="1a3cc-126">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a3cc-126">Files.ReadWrite</span></span>     |
| <span data-ttu-id="1a3cc-127">驱动器 （共享的 SharePoint 内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="1a3cc-127">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="1a3cc-128">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a3cc-128">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="1a3cc-129">安全警报</span><span class="sxs-lookup"><span data-stu-id="1a3cc-129">Security alert</span></span>               | <span data-ttu-id="1a3cc-130">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a3cc-130">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="1a3cc-131">***注意：***/Beta 终结点允许资源最多的应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="1a3cc-131">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="1a3cc-132">应用程序权限不支持对话组和 OneDrive 驱动器根项目。</span><span class="sxs-lookup"><span data-stu-id="1a3cc-132">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="1a3cc-133">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a3cc-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1a3cc-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a3cc-134">Request headers</span></span>

| <span data-ttu-id="1a3cc-135">名称</span><span class="sxs-lookup"><span data-stu-id="1a3cc-135">Name</span></span>       | <span data-ttu-id="1a3cc-136">类型</span><span class="sxs-lookup"><span data-stu-id="1a3cc-136">Type</span></span> | <span data-ttu-id="1a3cc-137">说明</span><span class="sxs-lookup"><span data-stu-id="1a3cc-137">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1a3cc-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a3cc-138">Authorization</span></span>  | <span data-ttu-id="1a3cc-139">string</span><span class="sxs-lookup"><span data-stu-id="1a3cc-139">string</span></span>  | <span data-ttu-id="1a3cc-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1a3cc-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1a3cc-142">响应</span><span class="sxs-lookup"><span data-stu-id="1a3cc-142">Response</span></span>

<span data-ttu-id="1a3cc-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1a3cc-143">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a3cc-144">示例</span><span class="sxs-lookup"><span data-stu-id="1a3cc-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1a3cc-145">请求</span><span class="sxs-lookup"><span data-stu-id="1a3cc-145">Request</span></span>

<span data-ttu-id="1a3cc-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a3cc-146">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="1a3cc-147">响应</span><span class="sxs-lookup"><span data-stu-id="1a3cc-147">Response</span></span>

<span data-ttu-id="1a3cc-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1a3cc-148">Here is an example of the response.</span></span>
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

<!--
{
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
