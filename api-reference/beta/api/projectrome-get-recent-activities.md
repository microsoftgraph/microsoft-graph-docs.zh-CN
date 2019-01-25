---
title: 获取最新的用户活动
description: " API 该服务将最近 historyItems，查询，然后提取这些相关的活动。 活动将根据最近**lastModified** **historyItem**上进行排序。 这意味着不**historyItems**活动将不包含在响应中。 UserActivity.ReadWrite.CreatedByApp 权限也将应用到响应，额外筛选，以便返回仅由您的应用程序创建的活动。 如果用户是特别活动和其他应用程序已创建较新的活动，则将此服务器端筛选可能会导致空白页。 要获取应用程序的活动，请使用**nextLink**属性进行分页。"
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 5ac5522472404e70f07b5b658e404cd4e77bbf88
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528961"
---
# <a name="get-recent-user-activities"></a><span data-ttu-id="47bfb-109">获取最新的用户活动</span><span class="sxs-lookup"><span data-stu-id="47bfb-109">Get recent user activities</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47bfb-110">获得给定用户的近期活动。</span><span class="sxs-lookup"><span data-stu-id="47bfb-110">Get recent activities for a given user.</span></span> <span data-ttu-id="47bfb-111">此 OData 函数具有一些包含以使其类似"最近使用"的 API 操作的默认行为。</span><span class="sxs-lookup"><span data-stu-id="47bfb-111">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="47bfb-112">该服务将最近[historyItems](../resources/projectrome-historyitem.md)，查询，然后提取这些相关的活动。</span><span class="sxs-lookup"><span data-stu-id="47bfb-112">The service will query for the most recent [historyItems](../resources/projectrome-historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="47bfb-113">活动将根据最近**lastModified** **historyItem**上进行排序。</span><span class="sxs-lookup"><span data-stu-id="47bfb-113">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="47bfb-114">这意味着不**historyItems**活动将不包含在响应中。</span><span class="sxs-lookup"><span data-stu-id="47bfb-114">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="47bfb-115">UserActivity.ReadWrite.CreatedByApp 权限也将应用到响应，额外筛选，以便返回仅由您的应用程序创建的活动。</span><span class="sxs-lookup"><span data-stu-id="47bfb-115">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="47bfb-116">如果用户是特别活动和其他应用程序已创建较新的活动，则将此服务器端筛选可能会导致空白页。</span><span class="sxs-lookup"><span data-stu-id="47bfb-116">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="47bfb-117">要获取应用程序的活动，请使用**nextLink**属性进行分页。</span><span class="sxs-lookup"><span data-stu-id="47bfb-117">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="47bfb-118">权限</span><span class="sxs-lookup"><span data-stu-id="47bfb-118">Permissions</span></span>

<span data-ttu-id="47bfb-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="47bfb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47bfb-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="47bfb-121">Permission type</span></span>      | <span data-ttu-id="47bfb-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="47bfb-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47bfb-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="47bfb-123">Delegated (work or school account)</span></span> | <span data-ttu-id="47bfb-124">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="47bfb-124">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="47bfb-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="47bfb-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47bfb-126">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="47bfb-126">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="47bfb-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="47bfb-127">Application</span></span> | <span data-ttu-id="47bfb-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="47bfb-128">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="47bfb-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="47bfb-129">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47bfb-130">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="47bfb-130">Optional query parameters</span></span>

<span data-ttu-id="47bfb-131">此方法支持某些[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)，以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="47bfb-131">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="47bfb-132">支持以下查询参数：</span><span class="sxs-lookup"><span data-stu-id="47bfb-132">The following query parameters are supported:</span></span>

- <span data-ttu-id="47bfb-133">$ expand **historyItems**导航属性。</span><span class="sxs-lookup"><span data-stu-id="47bfb-133">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="47bfb-134">$top 跨页限制的最大项目数。</span><span class="sxs-lookup"><span data-stu-id="47bfb-134">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="47bfb-135">在**活动**或**historyItems**，如果展开的**lastModifiedDateTime**属性 $filter。</span><span class="sxs-lookup"><span data-stu-id="47bfb-135">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="47bfb-136">以下是支持 URL 编码的查询的一些示例。</span><span class="sxs-lookup"><span data-stu-id="47bfb-136">The following are some examples of supported queries with URL encoding.</span></span>

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="47bfb-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="47bfb-137">Request headers</span></span>

|<span data-ttu-id="47bfb-138">名称</span><span class="sxs-lookup"><span data-stu-id="47bfb-138">Name</span></span> | <span data-ttu-id="47bfb-139">类型</span><span class="sxs-lookup"><span data-stu-id="47bfb-139">Type</span></span> | <span data-ttu-id="47bfb-140">说明</span><span class="sxs-lookup"><span data-stu-id="47bfb-140">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="47bfb-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="47bfb-141">Authorization</span></span> | <span data-ttu-id="47bfb-142">string</span><span class="sxs-lookup"><span data-stu-id="47bfb-142">string</span></span> | <span data-ttu-id="47bfb-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="47bfb-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="47bfb-145">请求正文</span><span class="sxs-lookup"><span data-stu-id="47bfb-145">Request body</span></span>

<span data-ttu-id="47bfb-146">不指定请求正文。</span><span class="sxs-lookup"><span data-stu-id="47bfb-146">Do not specify a request body.</span></span>

## <a name="response"></a><span data-ttu-id="47bfb-147">响应</span><span class="sxs-lookup"><span data-stu-id="47bfb-147">Response</span></span>

<span data-ttu-id="47bfb-148">如果成功，此方法返回`200 OK`与您的应用程序的用户的近期活动的响应代码。</span><span class="sxs-lookup"><span data-stu-id="47bfb-148">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="47bfb-149">示例</span><span class="sxs-lookup"><span data-stu-id="47bfb-149">Example</span></span>

##### <a name="request"></a><span data-ttu-id="47bfb-150">请求</span><span class="sxs-lookup"><span data-stu-id="47bfb-150">Request</span></span>

<span data-ttu-id="47bfb-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="47bfb-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities/recent
```

##### <a name="response"></a><span data-ttu-id="47bfb-152">响应</span><span class="sxs-lookup"><span data-stu-id="47bfb-152">Response</span></span>

<span data-ttu-id="47bfb-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="47bfb-153">The following is an example of the response.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/projectrome-get-recent-activities.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
