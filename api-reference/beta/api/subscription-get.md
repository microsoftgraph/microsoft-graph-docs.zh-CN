---
title: 获取订阅
description: 检索订阅的属性和关系。
ms.openlocfilehash: 5694015fe7e8cbf87b5d62f7ae4af35d1773532b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044662"
---
# <a name="get-subscription"></a><span data-ttu-id="d8e56-103">获取订阅</span><span class="sxs-lookup"><span data-stu-id="d8e56-103">Get subscription</span></span>

> <span data-ttu-id="d8e56-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d8e56-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8e56-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d8e56-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d8e56-106">检索订阅的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d8e56-106">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8e56-107">权限</span><span class="sxs-lookup"><span data-stu-id="d8e56-107">Permissions</span></span>

<span data-ttu-id="d8e56-p102">下表列出了对各个资源所需权限的建议。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d8e56-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d8e56-110">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="d8e56-110">Resource type / Item</span></span>        | <span data-ttu-id="d8e56-111">权限</span><span class="sxs-lookup"><span data-stu-id="d8e56-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="d8e56-112">联系人</span><span class="sxs-lookup"><span data-stu-id="d8e56-112">Contacts</span></span>                    | <span data-ttu-id="d8e56-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d8e56-113">Contacts.Read</span></span>       |
| <span data-ttu-id="d8e56-114">Conversations</span><span class="sxs-lookup"><span data-stu-id="d8e56-114">Conversations</span></span>               | <span data-ttu-id="d8e56-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8e56-115">Group.Read.All</span></span>      |
| <span data-ttu-id="d8e56-116">Events</span><span class="sxs-lookup"><span data-stu-id="d8e56-116">Events</span></span>                      | <span data-ttu-id="d8e56-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d8e56-117">Calendars.Read</span></span>      |
| <span data-ttu-id="d8e56-118">Messages</span><span class="sxs-lookup"><span data-stu-id="d8e56-118">Messages</span></span>                    | <span data-ttu-id="d8e56-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d8e56-119">Mail.Read</span></span>           |
| <span data-ttu-id="d8e56-120">Groups</span><span class="sxs-lookup"><span data-stu-id="d8e56-120">Groups</span></span>                      | <span data-ttu-id="d8e56-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8e56-121">Group.Read.All</span></span>      |
| <span data-ttu-id="d8e56-122">Users</span><span class="sxs-lookup"><span data-stu-id="d8e56-122">Users</span></span>                       | <span data-ttu-id="d8e56-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8e56-123">User.Read.All</span></span>       |
| <span data-ttu-id="d8e56-124">Drive（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="d8e56-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="d8e56-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8e56-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="d8e56-126">驱动器 （共享的 SharePoint 内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="d8e56-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="d8e56-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8e56-127">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="d8e56-128">安全警报</span><span class="sxs-lookup"><span data-stu-id="d8e56-128">Security alert</span></span>              | <span data-ttu-id="d8e56-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8e56-129">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="d8e56-130">***注意：***/Beta 终结点允许资源最多的应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="d8e56-130">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="d8e56-131">应用程序权限不支持对话组和 OneDrive 驱动器根项目。</span><span class="sxs-lookup"><span data-stu-id="d8e56-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="d8e56-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8e56-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d8e56-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d8e56-133">Optional query parameters</span></span>

<span data-ttu-id="d8e56-134">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d8e56-134">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d8e56-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8e56-135">Request headers</span></span>

| <span data-ttu-id="d8e56-136">名称</span><span class="sxs-lookup"><span data-stu-id="d8e56-136">Name</span></span>       | <span data-ttu-id="d8e56-137">类型</span><span class="sxs-lookup"><span data-stu-id="d8e56-137">Type</span></span> | <span data-ttu-id="d8e56-138">说明</span><span class="sxs-lookup"><span data-stu-id="d8e56-138">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="d8e56-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8e56-139">Authorization</span></span>  | <span data-ttu-id="d8e56-140">string</span><span class="sxs-lookup"><span data-stu-id="d8e56-140">string</span></span>  | <span data-ttu-id="d8e56-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d8e56-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8e56-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8e56-143">Request body</span></span>

<span data-ttu-id="d8e56-144">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d8e56-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8e56-145">响应</span><span class="sxs-lookup"><span data-stu-id="d8e56-145">Response</span></span>

<span data-ttu-id="d8e56-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d8e56-146">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8e56-147">示例</span><span class="sxs-lookup"><span data-stu-id="d8e56-147">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d8e56-148">请求</span><span class="sxs-lookup"><span data-stu-id="d8e56-148">Request</span></span>

<span data-ttu-id="d8e56-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d8e56-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="d8e56-150">响应</span><span class="sxs-lookup"><span data-stu-id="d8e56-150">Response</span></span>

<span data-ttu-id="d8e56-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d8e56-151">Here is an example of the response.</span></span>
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
