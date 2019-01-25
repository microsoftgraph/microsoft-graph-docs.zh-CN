---
title: 获取订阅
description: 检索订阅的属性和关系。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: c7dd20810cd9fdacec697345d42690f85bc3b8b1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522362"
---
# <a name="get-subscription"></a><span data-ttu-id="8b233-103">获取订阅</span><span class="sxs-lookup"><span data-stu-id="8b233-103">Get subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b233-104">检索订阅的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8b233-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b233-105">权限</span><span class="sxs-lookup"><span data-stu-id="8b233-105">Permissions</span></span>

<span data-ttu-id="8b233-p101">下表列出了对各个资源所需权限的建议。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8b233-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b233-108">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="8b233-108">Resource type / Item</span></span>        | <span data-ttu-id="8b233-109">权限</span><span class="sxs-lookup"><span data-stu-id="8b233-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="8b233-110">联系人</span><span class="sxs-lookup"><span data-stu-id="8b233-110">Contacts</span></span>                    | <span data-ttu-id="8b233-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8b233-111">Contacts.Read</span></span>       |
| <span data-ttu-id="8b233-112">Conversations</span><span class="sxs-lookup"><span data-stu-id="8b233-112">Conversations</span></span>               | <span data-ttu-id="8b233-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b233-113">Group.Read.All</span></span>      |
| <span data-ttu-id="8b233-114">Events</span><span class="sxs-lookup"><span data-stu-id="8b233-114">Events</span></span>                      | <span data-ttu-id="8b233-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8b233-115">Calendars.Read</span></span>      |
| <span data-ttu-id="8b233-116">Messages</span><span class="sxs-lookup"><span data-stu-id="8b233-116">Messages</span></span>                    | <span data-ttu-id="8b233-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8b233-117">Mail.Read</span></span>           |
| <span data-ttu-id="8b233-118">组</span><span class="sxs-lookup"><span data-stu-id="8b233-118">Groups</span></span>                      | <span data-ttu-id="8b233-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b233-119">Group.Read.All</span></span>      |
| <span data-ttu-id="8b233-120">用户</span><span class="sxs-lookup"><span data-stu-id="8b233-120">Users</span></span>                       | <span data-ttu-id="8b233-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b233-121">User.Read.All</span></span>       |
| <span data-ttu-id="8b233-122">Drive（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="8b233-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="8b233-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b233-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="8b233-124">驱动器 （共享的 SharePoint 内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="8b233-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="8b233-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b233-125">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="8b233-126">安全警报</span><span class="sxs-lookup"><span data-stu-id="8b233-126">Security alert</span></span>              | <span data-ttu-id="8b233-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b233-127">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="8b233-128">***注意：***/Beta 终结点允许资源最多的应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="8b233-128">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="8b233-129">应用程序权限不支持对话组和 OneDrive 驱动器根项目。</span><span class="sxs-lookup"><span data-stu-id="8b233-129">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="8b233-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8b233-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8b233-131">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8b233-131">Optional query parameters</span></span>

<span data-ttu-id="8b233-132">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8b233-132">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b233-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="8b233-133">Request headers</span></span>

| <span data-ttu-id="8b233-134">名称</span><span class="sxs-lookup"><span data-stu-id="8b233-134">Name</span></span>       | <span data-ttu-id="8b233-135">类型</span><span class="sxs-lookup"><span data-stu-id="8b233-135">Type</span></span> | <span data-ttu-id="8b233-136">说明</span><span class="sxs-lookup"><span data-stu-id="8b233-136">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="8b233-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b233-137">Authorization</span></span>  | <span data-ttu-id="8b233-138">string</span><span class="sxs-lookup"><span data-stu-id="8b233-138">string</span></span>  | <span data-ttu-id="8b233-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8b233-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b233-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="8b233-141">Request body</span></span>

<span data-ttu-id="8b233-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8b233-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b233-143">响应</span><span class="sxs-lookup"><span data-stu-id="8b233-143">Response</span></span>

<span data-ttu-id="8b233-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8b233-144">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b233-145">示例</span><span class="sxs-lookup"><span data-stu-id="8b233-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8b233-146">请求</span><span class="sxs-lookup"><span data-stu-id="8b233-146">Request</span></span>

<span data-ttu-id="8b233-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8b233-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="8b233-148">响应</span><span class="sxs-lookup"><span data-stu-id="8b233-148">Response</span></span>

<span data-ttu-id="8b233-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8b233-149">Here is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
