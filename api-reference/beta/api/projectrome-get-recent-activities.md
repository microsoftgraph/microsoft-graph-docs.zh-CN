---
title: 获取最近的用户活动
description: " #c1. 该服务将查询最近的 historyItems, 然后拉出这些相关的活动。 活动将根据**historyItem**上的最新**lastModified**进行排序。 这意味着不会在响应中包含不含**historyItems**的活动。 useractivity.readwrite.createdbyapp 权限还将对响应应用额外的筛选, 以便仅返回应用程序所创建的活动。 如果用户特别是活动的, 并且其他应用程序已创建了更新的活动, 则此服务器端筛选可能会导致空页面。 若要获取应用程序的活动, 请使用**nextLink**属性进行分页。"
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 464d57e5257b1e9c85796e72e4b8cbda732d4946
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337189"
---
# <a name="get-recent-user-activities"></a><span data-ttu-id="b755f-109">获取最近的用户活动</span><span class="sxs-lookup"><span data-stu-id="b755f-109">Get recent user activities</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b755f-110">获取给定用户的最近活动。</span><span class="sxs-lookup"><span data-stu-id="b755f-110">Get recent activities for a given user.</span></span> <span data-ttu-id="b755f-111">此 OData 函数包含一些默认行为, 以使其像 "最近使用过的" API 一样运行。</span><span class="sxs-lookup"><span data-stu-id="b755f-111">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="b755f-112">该服务将查询最近的[historyItems](../resources/projectrome-historyitem.md), 然后拉出这些相关的活动。</span><span class="sxs-lookup"><span data-stu-id="b755f-112">The service will query for the most recent [historyItems](../resources/projectrome-historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="b755f-113">活动将根据**historyItem**上的最新**lastModified**进行排序。</span><span class="sxs-lookup"><span data-stu-id="b755f-113">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="b755f-114">这意味着不会在响应中包含不含**historyItems**的活动。</span><span class="sxs-lookup"><span data-stu-id="b755f-114">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="b755f-115">useractivity.readwrite.createdbyapp 权限还将对响应应用额外的筛选, 以便仅返回应用程序所创建的活动。</span><span class="sxs-lookup"><span data-stu-id="b755f-115">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="b755f-116">如果用户特别是活动的, 并且其他应用程序已创建了更新的活动, 则此服务器端筛选可能会导致空页面。</span><span class="sxs-lookup"><span data-stu-id="b755f-116">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="b755f-117">若要获取应用程序的活动, 请使用**nextLink**属性进行分页。</span><span class="sxs-lookup"><span data-stu-id="b755f-117">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="b755f-118">权限</span><span class="sxs-lookup"><span data-stu-id="b755f-118">Permissions</span></span>

<span data-ttu-id="b755f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b755f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b755f-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="b755f-121">Permission type</span></span>      | <span data-ttu-id="b755f-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b755f-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b755f-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b755f-123">Delegated (work or school account)</span></span> | <span data-ttu-id="b755f-124">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="b755f-124">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="b755f-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b755f-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b755f-126">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="b755f-126">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="b755f-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="b755f-127">Application</span></span> | <span data-ttu-id="b755f-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="b755f-128">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b755f-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b755f-129">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b755f-130">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b755f-130">Optional query parameters</span></span>

<span data-ttu-id="b755f-131">此方法支持一些[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b755f-131">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="b755f-132">支持以下查询参数:</span><span class="sxs-lookup"><span data-stu-id="b755f-132">The following query parameters are supported:</span></span>

- <span data-ttu-id="b755f-133">**historyItems**导航属性的 $expand。</span><span class="sxs-lookup"><span data-stu-id="b755f-133">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="b755f-134">$top, 以限制跨页的最大项目数。</span><span class="sxs-lookup"><span data-stu-id="b755f-134">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="b755f-135">在**活动**或**historyItems**的**lastModifiedDateTime**属性上 $filter (如果已展开)。</span><span class="sxs-lookup"><span data-stu-id="b755f-135">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="b755f-136">以下是使用 URL 编码支持的查询的一些示例。</span><span class="sxs-lookup"><span data-stu-id="b755f-136">The following are some examples of supported queries with URL encoding.</span></span>

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="b755f-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="b755f-137">Request headers</span></span>

|<span data-ttu-id="b755f-138">名称</span><span class="sxs-lookup"><span data-stu-id="b755f-138">Name</span></span> | <span data-ttu-id="b755f-139">类型</span><span class="sxs-lookup"><span data-stu-id="b755f-139">Type</span></span> | <span data-ttu-id="b755f-140">说明</span><span class="sxs-lookup"><span data-stu-id="b755f-140">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="b755f-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="b755f-141">Authorization</span></span> | <span data-ttu-id="b755f-142">string</span><span class="sxs-lookup"><span data-stu-id="b755f-142">string</span></span> | <span data-ttu-id="b755f-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b755f-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b755f-145">请求正文</span><span class="sxs-lookup"><span data-stu-id="b755f-145">Request body</span></span>

<span data-ttu-id="b755f-146">请勿指定请求正文。</span><span class="sxs-lookup"><span data-stu-id="b755f-146">Do not specify a request body.</span></span>

## <a name="response"></a><span data-ttu-id="b755f-147">响应</span><span class="sxs-lookup"><span data-stu-id="b755f-147">Response</span></span>

<span data-ttu-id="b755f-148">如果成功, 此方法将返回`200 OK`应用程序的用户最近活动的响应代码。</span><span class="sxs-lookup"><span data-stu-id="b755f-148">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="b755f-149">示例</span><span class="sxs-lookup"><span data-stu-id="b755f-149">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b755f-150">请求</span><span class="sxs-lookup"><span data-stu-id="b755f-150">Request</span></span>

<span data-ttu-id="b755f-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b755f-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities/recent
```

##### <a name="response"></a><span data-ttu-id="b755f-152">响应</span><span class="sxs-lookup"><span data-stu-id="b755f-152">Response</span></span>

<span data-ttu-id="b755f-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b755f-153">The following is an example of the response.</span></span>

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
