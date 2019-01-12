---
title: 获取用户活动
description: 获得给定用户的活动。 与不同**最近**OData 函数，将返回不历史记录的活动。 权限 UserActivity.ReadWrite.CreatedByApp 将额外将筛选应用于响应，以便返回仅由您的应用程序创建的活动。 如果用户是特别活动和其他应用程序已创建较新的活动，则将此服务器端筛选可能会导致空白页。 要获取应用程序的活动，请使用**nextLink**属性进行分页。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: d6b2f4c14e1f33a09ed81aeb2c8d626ed70bcdc5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928183"
---
# <a name="get-user-activities"></a><span data-ttu-id="4a0b9-107">获取用户活动</span><span class="sxs-lookup"><span data-stu-id="4a0b9-107">Get user activities</span></span>

> <span data-ttu-id="4a0b9-108">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4a0b9-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a0b9-109">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4a0b9-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4a0b9-110">获得给定用户的活动。</span><span class="sxs-lookup"><span data-stu-id="4a0b9-110">Get activities for a given user.</span></span> <span data-ttu-id="4a0b9-111">与不同**最近**OData 函数，将返回不历史记录的活动。</span><span class="sxs-lookup"><span data-stu-id="4a0b9-111">Unlike the **recent** OData function, activities without histories will be returned.</span></span> <span data-ttu-id="4a0b9-112">权限 UserActivity.ReadWrite.CreatedByApp 将额外将筛选应用于响应，以便返回仅由您的应用程序创建的活动。</span><span class="sxs-lookup"><span data-stu-id="4a0b9-112">The permission UserActivity.ReadWrite.CreatedByApp will apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="4a0b9-113">如果用户是特别活动和其他应用程序已创建较新的活动，则将此服务器端筛选可能会导致空白页。</span><span class="sxs-lookup"><span data-stu-id="4a0b9-113">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="4a0b9-114">要获取应用程序的活动，请使用**nextLink**属性进行分页。</span><span class="sxs-lookup"><span data-stu-id="4a0b9-114">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a0b9-115">权限</span><span class="sxs-lookup"><span data-stu-id="4a0b9-115">Permissions</span></span>

<span data-ttu-id="4a0b9-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4a0b9-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a0b9-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a0b9-118">Permission type</span></span>      | <span data-ttu-id="4a0b9-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4a0b9-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a0b9-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a0b9-120">Delegated (work or school account)</span></span> | <span data-ttu-id="4a0b9-121">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="4a0b9-121">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="4a0b9-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a0b9-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a0b9-123">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="4a0b9-123">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="4a0b9-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a0b9-124">Application</span></span> | <span data-ttu-id="4a0b9-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a0b9-125">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a0b9-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a0b9-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4a0b9-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4a0b9-127">Optional query parameters</span></span>

<span data-ttu-id="4a0b9-128">此方法支持某些[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)，以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4a0b9-128">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="4a0b9-129">支持以下查询参数：</span><span class="sxs-lookup"><span data-stu-id="4a0b9-129">The following query parameters are supported:</span></span>

- <span data-ttu-id="4a0b9-130">$ expand **historyItems**导航属性。</span><span class="sxs-lookup"><span data-stu-id="4a0b9-130">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="4a0b9-131">$top 跨页限制的最大项目数。</span><span class="sxs-lookup"><span data-stu-id="4a0b9-131">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="4a0b9-132">在**活动**或**historyItems**，如果展开的**lastModifiedDateTime**属性 $filter。</span><span class="sxs-lookup"><span data-stu-id="4a0b9-132">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="4a0b9-133">以下是支持 URL 编码的查询的一些示例：</span><span class="sxs-lookup"><span data-stu-id="4a0b9-133">The following are some examples of supported queries with URL encoding:</span></span>

```
/me/activities?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="4a0b9-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="4a0b9-134">Request headers</span></span>

|<span data-ttu-id="4a0b9-135">名称</span><span class="sxs-lookup"><span data-stu-id="4a0b9-135">Name</span></span> | <span data-ttu-id="4a0b9-136">类型</span><span class="sxs-lookup"><span data-stu-id="4a0b9-136">Type</span></span> | <span data-ttu-id="4a0b9-137">说明</span><span class="sxs-lookup"><span data-stu-id="4a0b9-137">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="4a0b9-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a0b9-138">Authorization</span></span> | <span data-ttu-id="4a0b9-139">string</span><span class="sxs-lookup"><span data-stu-id="4a0b9-139">string</span></span> | <span data-ttu-id="4a0b9-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4a0b9-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a0b9-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="4a0b9-142">Request body</span></span>

<span data-ttu-id="4a0b9-143">没有请求正文中。</span><span class="sxs-lookup"><span data-stu-id="4a0b9-143">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="4a0b9-144">响应</span><span class="sxs-lookup"><span data-stu-id="4a0b9-144">Response</span></span>

<span data-ttu-id="4a0b9-145">如果成功，此方法返回`200 OK`与您的应用程序的用户的活动的响应代码。</span><span class="sxs-lookup"><span data-stu-id="4a0b9-145">If successful, this method returns the `200 OK` response code with the user's activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="4a0b9-146">示例</span><span class="sxs-lookup"><span data-stu-id="4a0b9-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4a0b9-147">请求</span><span class="sxs-lookup"><span data-stu-id="4a0b9-147">Request</span></span>

<span data-ttu-id="4a0b9-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4a0b9-148">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities
```

##### <a name="response"></a><span data-ttu-id="4a0b9-149">响应</span><span class="sxs-lookup"><span data-stu-id="4a0b9-149">Response</span></span>

<span data-ttu-id="4a0b9-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4a0b9-150">The following is an example of the response.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
