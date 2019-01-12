---
title: 获取订阅
description: 检索订阅的属性和关系。
localization_priority: Priority
author: piotrci
ms.openlocfilehash: 4c55c81fdb26bb706ad270e5d53ded712ea69b22
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956974"
---
# <a name="get-subscription"></a><span data-ttu-id="4122d-103">获取订阅</span><span class="sxs-lookup"><span data-stu-id="4122d-103">Get subscription</span></span>

<span data-ttu-id="4122d-104">检索订阅的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4122d-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="4122d-105">权限</span><span class="sxs-lookup"><span data-stu-id="4122d-105">Permissions</span></span>

<span data-ttu-id="4122d-p101">下表列出了对各个资源所需权限的建议。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4122d-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4122d-108">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="4122d-108">Resource type / Item</span></span>        | <span data-ttu-id="4122d-109">权限</span><span class="sxs-lookup"><span data-stu-id="4122d-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="4122d-110">联系人</span><span class="sxs-lookup"><span data-stu-id="4122d-110">Contacts</span></span>                    | <span data-ttu-id="4122d-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4122d-111">Contacts.Read</span></span>       |
| <span data-ttu-id="4122d-112">Conversations</span><span class="sxs-lookup"><span data-stu-id="4122d-112">Conversations</span></span>               | <span data-ttu-id="4122d-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4122d-113">Group.Read.All</span></span>      |
| <span data-ttu-id="4122d-114">Events</span><span class="sxs-lookup"><span data-stu-id="4122d-114">Events</span></span>                      | <span data-ttu-id="4122d-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4122d-115">Calendars.Read</span></span>      |
| <span data-ttu-id="4122d-116">Messages</span><span class="sxs-lookup"><span data-stu-id="4122d-116">Messages</span></span>                    | <span data-ttu-id="4122d-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4122d-117">Mail.Read</span></span>           |
| <span data-ttu-id="4122d-118">组</span><span class="sxs-lookup"><span data-stu-id="4122d-118">Groups</span></span>                      | <span data-ttu-id="4122d-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4122d-119">Group.Read.All</span></span>      |
| <span data-ttu-id="4122d-120">用户</span><span class="sxs-lookup"><span data-stu-id="4122d-120">Users</span></span>                       | <span data-ttu-id="4122d-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4122d-121">User.Read.All</span></span>       |
| <span data-ttu-id="4122d-122">Drive（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="4122d-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="4122d-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4122d-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="4122d-124">驱动器 （共享的 SharePoint 内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="4122d-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="4122d-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4122d-125">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="4122d-126">安全警报</span><span class="sxs-lookup"><span data-stu-id="4122d-126">Security alert</span></span>| <span data-ttu-id="4122d-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4122d-127">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4122d-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4122d-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4122d-129">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4122d-129">Optional query parameters</span></span>

<span data-ttu-id="4122d-130">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4122d-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4122d-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="4122d-131">Request headers</span></span>

| <span data-ttu-id="4122d-132">名称</span><span class="sxs-lookup"><span data-stu-id="4122d-132">Name</span></span>       | <span data-ttu-id="4122d-133">类型</span><span class="sxs-lookup"><span data-stu-id="4122d-133">Type</span></span> | <span data-ttu-id="4122d-134">说明</span><span class="sxs-lookup"><span data-stu-id="4122d-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4122d-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="4122d-135">Authorization</span></span>  | <span data-ttu-id="4122d-136">string</span><span class="sxs-lookup"><span data-stu-id="4122d-136">string</span></span>  | <span data-ttu-id="4122d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4122d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4122d-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="4122d-139">Request body</span></span>

<span data-ttu-id="4122d-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4122d-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4122d-141">响应</span><span class="sxs-lookup"><span data-stu-id="4122d-141">Response</span></span>

<span data-ttu-id="4122d-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4122d-142">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4122d-143">示例</span><span class="sxs-lookup"><span data-stu-id="4122d-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4122d-144">请求</span><span class="sxs-lookup"><span data-stu-id="4122d-144">Request</span></span>

<span data-ttu-id="4122d-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4122d-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="4122d-146">响应</span><span class="sxs-lookup"><span data-stu-id="4122d-146">Response</span></span>

<span data-ttu-id="4122d-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4122d-147">Here is an example of the response.</span></span>
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
  "applicationId" : "string",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
