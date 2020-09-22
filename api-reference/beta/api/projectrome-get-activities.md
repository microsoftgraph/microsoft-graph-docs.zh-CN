---
title: 获取用户活动
description: 获取给定用户的活动。 与 **最近** 的 OData 函数不同，将返回不含历史记录的活动。 权限 Useractivity.readwrite.createdbyapp Useractivity.readwrite.createdbyapp 将对响应应用额外的筛选，以便仅返回应用程序所创建的活动。 如果用户特别是活动的，并且其他应用程序已创建了更新的活动，则此服务器端筛选可能会导致空页面。 若要获取应用程序的活动，请使用 **nextLink** 属性进行分页。
localization_priority: Normal
ms.prod: project-rome
doc_type: apiPageType
author: ailae
ms.openlocfilehash: c34149a5325e3f7b7087c886a6faab5a9963535a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48014278"
---
# <a name="get-user-activities"></a><span data-ttu-id="a3a6b-107">获取用户活动</span><span class="sxs-lookup"><span data-stu-id="a3a6b-107">Get user activities</span></span>

<span data-ttu-id="a3a6b-108">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3a6b-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3a6b-109">获取给定用户的活动。</span><span class="sxs-lookup"><span data-stu-id="a3a6b-109">Get activities for a given user.</span></span> <span data-ttu-id="a3a6b-110">与 **最近** 的 OData 函数不同，将返回不含历史记录的活动。</span><span class="sxs-lookup"><span data-stu-id="a3a6b-110">Unlike the **recent** OData function, activities without histories will be returned.</span></span> <span data-ttu-id="a3a6b-111">权限 Useractivity.readwrite.createdbyapp Useractivity.readwrite.createdbyapp 将对响应应用额外的筛选，以便仅返回应用程序所创建的活动。</span><span class="sxs-lookup"><span data-stu-id="a3a6b-111">The permission UserActivity.ReadWrite.CreatedByApp will apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="a3a6b-112">如果用户特别是活动的，并且其他应用程序已创建了更新的活动，则此服务器端筛选可能会导致空页面。</span><span class="sxs-lookup"><span data-stu-id="a3a6b-112">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="a3a6b-113">若要获取应用程序的活动，请使用 **nextLink** 属性进行分页。</span><span class="sxs-lookup"><span data-stu-id="a3a6b-113">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3a6b-114">权限</span><span class="sxs-lookup"><span data-stu-id="a3a6b-114">Permissions</span></span>

<span data-ttu-id="a3a6b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a3a6b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3a6b-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3a6b-117">Permission type</span></span>      | <span data-ttu-id="a3a6b-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a3a6b-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3a6b-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3a6b-119">Delegated (work or school account)</span></span> | <span data-ttu-id="a3a6b-120">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="a3a6b-120">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="a3a6b-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3a6b-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3a6b-122">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="a3a6b-122">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="a3a6b-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="a3a6b-123">Application</span></span> | <span data-ttu-id="a3a6b-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3a6b-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3a6b-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3a6b-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a3a6b-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a3a6b-126">Optional query parameters</span></span>

<span data-ttu-id="a3a6b-127">此方法支持一些 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a3a6b-127">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="a3a6b-128">支持以下查询参数：</span><span class="sxs-lookup"><span data-stu-id="a3a6b-128">The following query parameters are supported:</span></span>

- <span data-ttu-id="a3a6b-129">**historyItems**导航属性的 $expand。</span><span class="sxs-lookup"><span data-stu-id="a3a6b-129">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="a3a6b-130">$top，以限制跨页的最大项目数。</span><span class="sxs-lookup"><span data-stu-id="a3a6b-130">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="a3a6b-131">在**活动**或**historyItems**的**lastModifiedDateTime**属性上 $filter （如果已展开）。</span><span class="sxs-lookup"><span data-stu-id="a3a6b-131">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="a3a6b-132">以下是使用 URL 编码支持的查询的一些示例：</span><span class="sxs-lookup"><span data-stu-id="a3a6b-132">The following are some examples of supported queries with URL encoding:</span></span>

```
/me/activities?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="a3a6b-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3a6b-133">Request headers</span></span>

|<span data-ttu-id="a3a6b-134">名称</span><span class="sxs-lookup"><span data-stu-id="a3a6b-134">Name</span></span> | <span data-ttu-id="a3a6b-135">类型</span><span class="sxs-lookup"><span data-stu-id="a3a6b-135">Type</span></span> | <span data-ttu-id="a3a6b-136">说明</span><span class="sxs-lookup"><span data-stu-id="a3a6b-136">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="a3a6b-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3a6b-137">Authorization</span></span> | <span data-ttu-id="a3a6b-138">string</span><span class="sxs-lookup"><span data-stu-id="a3a6b-138">string</span></span> | <span data-ttu-id="a3a6b-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a3a6b-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3a6b-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="a3a6b-141">Request body</span></span>

<span data-ttu-id="a3a6b-142">无请求正文。</span><span class="sxs-lookup"><span data-stu-id="a3a6b-142">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="a3a6b-143">响应</span><span class="sxs-lookup"><span data-stu-id="a3a6b-143">Response</span></span>

<span data-ttu-id="a3a6b-144">如果成功，此方法将返回 `200 OK` 应用程序的用户活动的响应代码。</span><span class="sxs-lookup"><span data-stu-id="a3a6b-144">If successful, this method returns the `200 OK` response code with the user's activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="a3a6b-145">示例</span><span class="sxs-lookup"><span data-stu-id="a3a6b-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a3a6b-146">请求</span><span class="sxs-lookup"><span data-stu-id="a3a6b-146">Request</span></span>

<span data-ttu-id="a3a6b-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a3a6b-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities
```

##### <a name="response"></a><span data-ttu-id="a3a6b-148">响应</span><span class="sxs-lookup"><span data-stu-id="a3a6b-148">Response</span></span>

<span data-ttu-id="a3a6b-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a3a6b-149">The following is an example of the response.</span></span>

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
  "suppressions": []
}
-->


