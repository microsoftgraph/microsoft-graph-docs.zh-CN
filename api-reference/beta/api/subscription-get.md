---
title: 获取订阅
description: 检索订阅的属性和关系。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 165fd990d7dbec64eb61b9e06d05b51b40bf1212
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934882"
---
# <a name="get-subscription"></a><span data-ttu-id="778c4-103">获取订阅</span><span class="sxs-lookup"><span data-stu-id="778c4-103">Get subscription</span></span>

> <span data-ttu-id="778c4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="778c4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="778c4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="778c4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="778c4-106">检索订阅的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="778c4-106">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="778c4-107">权限</span><span class="sxs-lookup"><span data-stu-id="778c4-107">Permissions</span></span>

<span data-ttu-id="778c4-p102">下表列出了对各个资源所需权限的建议。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="778c4-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="778c4-110">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="778c4-110">Resource type / Item</span></span>        | <span data-ttu-id="778c4-111">权限</span><span class="sxs-lookup"><span data-stu-id="778c4-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="778c4-112">联系人</span><span class="sxs-lookup"><span data-stu-id="778c4-112">Contacts</span></span>                    | <span data-ttu-id="778c4-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="778c4-113">Contacts.Read</span></span>       |
| <span data-ttu-id="778c4-114">Conversations</span><span class="sxs-lookup"><span data-stu-id="778c4-114">Conversations</span></span>               | <span data-ttu-id="778c4-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="778c4-115">Group.Read.All</span></span>      |
| <span data-ttu-id="778c4-116">Events</span><span class="sxs-lookup"><span data-stu-id="778c4-116">Events</span></span>                      | <span data-ttu-id="778c4-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="778c4-117">Calendars.Read</span></span>      |
| <span data-ttu-id="778c4-118">Messages</span><span class="sxs-lookup"><span data-stu-id="778c4-118">Messages</span></span>                    | <span data-ttu-id="778c4-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="778c4-119">Mail.Read</span></span>           |
| <span data-ttu-id="778c4-120">组</span><span class="sxs-lookup"><span data-stu-id="778c4-120">Groups</span></span>                      | <span data-ttu-id="778c4-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="778c4-121">Group.Read.All</span></span>      |
| <span data-ttu-id="778c4-122">用户</span><span class="sxs-lookup"><span data-stu-id="778c4-122">Users</span></span>                       | <span data-ttu-id="778c4-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="778c4-123">User.Read.All</span></span>       |
| <span data-ttu-id="778c4-124">Drive（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="778c4-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="778c4-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="778c4-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="778c4-126">驱动器 （共享的 SharePoint 内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="778c4-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="778c4-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="778c4-127">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="778c4-128">安全警报</span><span class="sxs-lookup"><span data-stu-id="778c4-128">Security alert</span></span>              | <span data-ttu-id="778c4-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="778c4-129">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="778c4-130">***注意：***/Beta 终结点允许资源最多的应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="778c4-130">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="778c4-131">应用程序权限不支持对话组和 OneDrive 驱动器根项目。</span><span class="sxs-lookup"><span data-stu-id="778c4-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="778c4-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="778c4-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="778c4-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="778c4-133">Optional query parameters</span></span>

<span data-ttu-id="778c4-134">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="778c4-134">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="778c4-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="778c4-135">Request headers</span></span>

| <span data-ttu-id="778c4-136">名称</span><span class="sxs-lookup"><span data-stu-id="778c4-136">Name</span></span>       | <span data-ttu-id="778c4-137">类型</span><span class="sxs-lookup"><span data-stu-id="778c4-137">Type</span></span> | <span data-ttu-id="778c4-138">说明</span><span class="sxs-lookup"><span data-stu-id="778c4-138">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="778c4-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="778c4-139">Authorization</span></span>  | <span data-ttu-id="778c4-140">string</span><span class="sxs-lookup"><span data-stu-id="778c4-140">string</span></span>  | <span data-ttu-id="778c4-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="778c4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="778c4-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="778c4-143">Request body</span></span>

<span data-ttu-id="778c4-144">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="778c4-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="778c4-145">响应</span><span class="sxs-lookup"><span data-stu-id="778c4-145">Response</span></span>

<span data-ttu-id="778c4-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="778c4-146">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="778c4-147">示例</span><span class="sxs-lookup"><span data-stu-id="778c4-147">Example</span></span>

##### <a name="request"></a><span data-ttu-id="778c4-148">请求</span><span class="sxs-lookup"><span data-stu-id="778c4-148">Request</span></span>

<span data-ttu-id="778c4-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="778c4-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="778c4-150">响应</span><span class="sxs-lookup"><span data-stu-id="778c4-150">Response</span></span>

<span data-ttu-id="778c4-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="778c4-151">Here is an example of the response.</span></span>
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
