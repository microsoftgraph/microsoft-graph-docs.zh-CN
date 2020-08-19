---
title: 获取最近的用户活动
description: " #C1. 该服务将查询最近的 historyItems，然后拉出这些相关的活动。 活动将根据**historyItem**上的最新**lastModified**进行排序。 这意味着不会在响应中包含不含 **historyItems** 的活动。 Useractivity.readwrite.createdbyapp 权限还将对响应应用额外的筛选，以便仅返回应用程序所创建的活动。 如果用户特别是活动的，并且其他应用程序已创建了更新的活动，则此服务器端筛选可能会导致空页面。 若要获取应用程序的活动，请使用 **nextLink** 属性进行分页。"
localization_priority: Normal
ms.prod: project-rome
doc_type: apiPageType
author: ailae
ms.openlocfilehash: 72c9e425a74f10d066b2fd958126623a5f900601
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809962"
---
# <a name="get-recent-user-activities"></a><span data-ttu-id="d9fc6-109">获取最近的用户活动</span><span class="sxs-lookup"><span data-stu-id="d9fc6-109">Get recent user activities</span></span>

<span data-ttu-id="d9fc6-110">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9fc6-110">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9fc6-111">获取给定用户的最近活动。</span><span class="sxs-lookup"><span data-stu-id="d9fc6-111">Get recent activities for a given user.</span></span> <span data-ttu-id="d9fc6-112">此 OData 函数包含一些默认行为，以使其像 "最近使用过的" API 一样运行。</span><span class="sxs-lookup"><span data-stu-id="d9fc6-112">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="d9fc6-113">该服务将查询最近的 [historyItems](../resources/projectrome-historyitem.md)，然后拉出这些相关的活动。</span><span class="sxs-lookup"><span data-stu-id="d9fc6-113">The service will query for the most recent [historyItems](../resources/projectrome-historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="d9fc6-114">活动将根据**historyItem**上的最新**lastModified**进行排序。</span><span class="sxs-lookup"><span data-stu-id="d9fc6-114">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="d9fc6-115">这意味着不会在响应中包含不含 **historyItems** 的活动。</span><span class="sxs-lookup"><span data-stu-id="d9fc6-115">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="d9fc6-116">Useractivity.readwrite.createdbyapp 权限还将对响应应用额外的筛选，以便仅返回应用程序所创建的活动。</span><span class="sxs-lookup"><span data-stu-id="d9fc6-116">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="d9fc6-117">如果用户特别是活动的，并且其他应用程序已创建了更新的活动，则此服务器端筛选可能会导致空页面。</span><span class="sxs-lookup"><span data-stu-id="d9fc6-117">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="d9fc6-118">若要获取应用程序的活动，请使用 **nextLink** 属性进行分页。</span><span class="sxs-lookup"><span data-stu-id="d9fc6-118">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9fc6-119">权限</span><span class="sxs-lookup"><span data-stu-id="d9fc6-119">Permissions</span></span>

<span data-ttu-id="d9fc6-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d9fc6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9fc6-122">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9fc6-122">Permission type</span></span>      | <span data-ttu-id="d9fc6-123">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d9fc6-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9fc6-124">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9fc6-124">Delegated (work or school account)</span></span> | <span data-ttu-id="d9fc6-125">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="d9fc6-125">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="d9fc6-126">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9fc6-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9fc6-127">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="d9fc6-127">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="d9fc6-128">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9fc6-128">Application</span></span> | <span data-ttu-id="d9fc6-129">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9fc6-129">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9fc6-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9fc6-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d9fc6-131">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d9fc6-131">Optional query parameters</span></span>

<span data-ttu-id="d9fc6-132">此方法支持一些 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d9fc6-132">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="d9fc6-133">支持以下查询参数：</span><span class="sxs-lookup"><span data-stu-id="d9fc6-133">The following query parameters are supported:</span></span>

- <span data-ttu-id="d9fc6-134">**historyItems**导航属性的 $expand。</span><span class="sxs-lookup"><span data-stu-id="d9fc6-134">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="d9fc6-135">$top，以限制跨页的最大项目数。</span><span class="sxs-lookup"><span data-stu-id="d9fc6-135">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="d9fc6-136">在**活动**或**historyItems**的**lastModifiedDateTime**属性上 $filter （如果已展开）。</span><span class="sxs-lookup"><span data-stu-id="d9fc6-136">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="d9fc6-137">以下是使用 URL 编码支持的查询的一些示例。</span><span class="sxs-lookup"><span data-stu-id="d9fc6-137">The following are some examples of supported queries with URL encoding.</span></span>

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="d9fc6-138">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9fc6-138">Request headers</span></span>

|<span data-ttu-id="d9fc6-139">名称</span><span class="sxs-lookup"><span data-stu-id="d9fc6-139">Name</span></span> | <span data-ttu-id="d9fc6-140">类型</span><span class="sxs-lookup"><span data-stu-id="d9fc6-140">Type</span></span> | <span data-ttu-id="d9fc6-141">说明</span><span class="sxs-lookup"><span data-stu-id="d9fc6-141">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="d9fc6-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9fc6-142">Authorization</span></span> | <span data-ttu-id="d9fc6-143">string</span><span class="sxs-lookup"><span data-stu-id="d9fc6-143">string</span></span> | <span data-ttu-id="d9fc6-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d9fc6-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9fc6-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9fc6-146">Request body</span></span>

<span data-ttu-id="d9fc6-147">请勿指定请求正文。</span><span class="sxs-lookup"><span data-stu-id="d9fc6-147">Do not specify a request body.</span></span>

## <a name="response"></a><span data-ttu-id="d9fc6-148">响应</span><span class="sxs-lookup"><span data-stu-id="d9fc6-148">Response</span></span>

<span data-ttu-id="d9fc6-149">如果成功，此方法将返回 `200 OK` 应用程序的用户最近活动的响应代码。</span><span class="sxs-lookup"><span data-stu-id="d9fc6-149">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="d9fc6-150">示例</span><span class="sxs-lookup"><span data-stu-id="d9fc6-150">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d9fc6-151">请求</span><span class="sxs-lookup"><span data-stu-id="d9fc6-151">Request</span></span>

<span data-ttu-id="d9fc6-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d9fc6-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities/recent
```

##### <a name="response"></a><span data-ttu-id="d9fc6-153">响应</span><span class="sxs-lookup"><span data-stu-id="d9fc6-153">Response</span></span>

<span data-ttu-id="d9fc6-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d9fc6-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.activity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/activities/recent?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
    "value": [{
        "@odata.type": "#microsoft.graph.activity",
        "activitySourceHost": "https://www.contoso.com",
        "createdDateTime": "2018-02-26T18:34:29.592Z",
        "lastModifiedDateTime": "2018-02-26T18:34:29.607Z",
        "id": "5347642601316252694",
        "appActivityId": "/article?12345",
        "visualElements": {
            "attribution": {
              "iconUrl": "https://www.contoso.com/icon",
              "alternateText": "Contoso, Ltd.",
              "addImageQuery": "false",
              },
            "displayText": "Contoso How-To: How to Tie a Reef Knot",
            "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
            "backgroundColor": "#ff0000",
            "content": {
              "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
              "type": "AdaptiveCard",
              "body":
              [{
                  "type": "TextBlock",
                  "text": "Contoso MainPage"
              }]
            }
        },
        "activationUrl": "https://www.contoso.com/article?id=12345",
        "appDisplayName": "Contoso, Ltd.",
        "userTimezone": "Africa/Casablanca",
        "fallbackUrl": "https://www.contoso.com/article?id=12345",
        "contentUrl": "https://www.contoso.com/article?id=12345",
        "contentInfo": {
            "@context": "https://schema.org",
            "@type": "Article",
            "author": "John Doe",
            "name": "How to Tie a Reef Knot"
        },
        "expirationDateTime": "2018-03-28T18:34:29.607Z",
        "status": "updated"
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get recent activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
