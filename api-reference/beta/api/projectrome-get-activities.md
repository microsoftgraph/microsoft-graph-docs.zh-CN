---
title: 获取用户活动
description: 获取给定用户的活动。 与**最近**的 OData 函数不同, 将返回不含历史记录的活动。 权限 useractivity.readwrite.createdbyapp useractivity.readwrite.createdbyapp 将对响应应用额外的筛选, 以便仅返回应用程序所创建的活动。 如果用户特别是活动的, 并且其他应用程序已创建了更新的活动, 则此服务器端筛选可能会导致空页面。 若要获取应用程序的活动, 请使用**nextLink**属性进行分页。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 96830c2698a079018368ce907ca39d4cda0f63fe
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546330"
---
# <a name="get-user-activities"></a><span data-ttu-id="5c5a7-107">获取用户活动</span><span class="sxs-lookup"><span data-stu-id="5c5a7-107">Get user activities</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c5a7-108">获取给定用户的活动。</span><span class="sxs-lookup"><span data-stu-id="5c5a7-108">Get activities for a given user.</span></span> <span data-ttu-id="5c5a7-109">与**最近**的 OData 函数不同, 将返回不含历史记录的活动。</span><span class="sxs-lookup"><span data-stu-id="5c5a7-109">Unlike the **recent** OData function, activities without histories will be returned.</span></span> <span data-ttu-id="5c5a7-110">权限 useractivity.readwrite.createdbyapp useractivity.readwrite.createdbyapp 将对响应应用额外的筛选, 以便仅返回应用程序所创建的活动。</span><span class="sxs-lookup"><span data-stu-id="5c5a7-110">The permission UserActivity.ReadWrite.CreatedByApp will apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="5c5a7-111">如果用户特别是活动的, 并且其他应用程序已创建了更新的活动, 则此服务器端筛选可能会导致空页面。</span><span class="sxs-lookup"><span data-stu-id="5c5a7-111">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="5c5a7-112">若要获取应用程序的活动, 请使用**nextLink**属性进行分页。</span><span class="sxs-lookup"><span data-stu-id="5c5a7-112">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c5a7-113">权限</span><span class="sxs-lookup"><span data-stu-id="5c5a7-113">Permissions</span></span>

<span data-ttu-id="5c5a7-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5c5a7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c5a7-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c5a7-116">Permission type</span></span>      | <span data-ttu-id="5c5a7-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5c5a7-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c5a7-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c5a7-118">Delegated (work or school account)</span></span> | <span data-ttu-id="5c5a7-119">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="5c5a7-119">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="5c5a7-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c5a7-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c5a7-121">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="5c5a7-121">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="5c5a7-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c5a7-122">Application</span></span> | <span data-ttu-id="5c5a7-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c5a7-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c5a7-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c5a7-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5c5a7-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5c5a7-125">Optional query parameters</span></span>

<span data-ttu-id="5c5a7-126">此方法支持一些[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5c5a7-126">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="5c5a7-127">支持以下查询参数:</span><span class="sxs-lookup"><span data-stu-id="5c5a7-127">The following query parameters are supported:</span></span>

- <span data-ttu-id="5c5a7-128">**historyItems**导航属性的 $expand。</span><span class="sxs-lookup"><span data-stu-id="5c5a7-128">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="5c5a7-129">$top, 以限制跨页的最大项目数。</span><span class="sxs-lookup"><span data-stu-id="5c5a7-129">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="5c5a7-130">在**活动**或**historyItems**的**lastModifiedDateTime**属性上 $filter (如果已展开)。</span><span class="sxs-lookup"><span data-stu-id="5c5a7-130">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="5c5a7-131">以下是使用 URL 编码支持的查询的一些示例:</span><span class="sxs-lookup"><span data-stu-id="5c5a7-131">The following are some examples of supported queries with URL encoding:</span></span>

```
/me/activities?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="5c5a7-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="5c5a7-132">Request headers</span></span>

|<span data-ttu-id="5c5a7-133">名称</span><span class="sxs-lookup"><span data-stu-id="5c5a7-133">Name</span></span> | <span data-ttu-id="5c5a7-134">类型</span><span class="sxs-lookup"><span data-stu-id="5c5a7-134">Type</span></span> | <span data-ttu-id="5c5a7-135">说明</span><span class="sxs-lookup"><span data-stu-id="5c5a7-135">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="5c5a7-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c5a7-136">Authorization</span></span> | <span data-ttu-id="5c5a7-137">string</span><span class="sxs-lookup"><span data-stu-id="5c5a7-137">string</span></span> | <span data-ttu-id="5c5a7-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5c5a7-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c5a7-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c5a7-140">Request body</span></span>

<span data-ttu-id="5c5a7-141">无请求正文。</span><span class="sxs-lookup"><span data-stu-id="5c5a7-141">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="5c5a7-142">响应</span><span class="sxs-lookup"><span data-stu-id="5c5a7-142">Response</span></span>

<span data-ttu-id="5c5a7-143">如果成功, 此方法将返回`200 OK`应用程序的用户活动的响应代码。</span><span class="sxs-lookup"><span data-stu-id="5c5a7-143">If successful, this method returns the `200 OK` response code with the user's activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="5c5a7-144">示例</span><span class="sxs-lookup"><span data-stu-id="5c5a7-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5c5a7-145">请求</span><span class="sxs-lookup"><span data-stu-id="5c5a7-145">Request</span></span>

<span data-ttu-id="5c5a7-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5c5a7-146">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities
```

##### <a name="response"></a><span data-ttu-id="5c5a7-147">响应</span><span class="sxs-lookup"><span data-stu-id="5c5a7-147">Response</span></span>

<span data-ttu-id="5c5a7-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5c5a7-148">The following is an example of the response.</span></span>

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
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/activities?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
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
  "description": "Get activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/projectrome-get-activities.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
