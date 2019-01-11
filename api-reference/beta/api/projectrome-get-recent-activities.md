---
title: 获取最新的用户活动
description: " API。 该服务将最近 historyItems，查询，然后提取这些相关的活动。 活动将根据最近**lastModified** **historyItem**上进行排序。 这意味着不**historyItems**活动将不包含在响应中。 UserActivity.ReadWrite.CreatedByApp 权限也将应用到响应，额外筛选，以便返回仅由您的应用程序创建的活动。 如果用户是特别活动和其他应用程序已创建较新的活动，则将此服务器端筛选可能会导致空白页。 要获取应用程序的活动，请使用**nextLink**属性进行分页。"
localization_priority: Normal
ms.openlocfilehash: 36df29d2000934da417b473235575f5741078dc8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819787"
---
# <a name="get-recent-user-activities"></a><span data-ttu-id="48f29-109">获取最新的用户活动</span><span class="sxs-lookup"><span data-stu-id="48f29-109">Get recent user activities</span></span>

> <span data-ttu-id="48f29-110">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="48f29-110">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48f29-111">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="48f29-111">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="48f29-112">获得给定用户的近期活动。</span><span class="sxs-lookup"><span data-stu-id="48f29-112">Get recent activities for a given user.</span></span> <span data-ttu-id="48f29-113">此 OData 函数具有一些包含以使其类似"最近使用"的 API 操作的默认行为。</span><span class="sxs-lookup"><span data-stu-id="48f29-113">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="48f29-114">该服务将最近[historyItems](../resources/projectrome-historyitem.md)，查询，然后提取这些相关的活动。</span><span class="sxs-lookup"><span data-stu-id="48f29-114">The service will query for the most recent [historyItems](../resources/projectrome-historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="48f29-115">活动将根据最近**lastModified** **historyItem**上进行排序。</span><span class="sxs-lookup"><span data-stu-id="48f29-115">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="48f29-116">这意味着不**historyItems**活动将不包含在响应中。</span><span class="sxs-lookup"><span data-stu-id="48f29-116">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="48f29-117">UserActivity.ReadWrite.CreatedByApp 权限也将应用到响应，额外筛选，以便返回仅由您的应用程序创建的活动。</span><span class="sxs-lookup"><span data-stu-id="48f29-117">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="48f29-118">如果用户是特别活动和其他应用程序已创建较新的活动，则将此服务器端筛选可能会导致空白页。</span><span class="sxs-lookup"><span data-stu-id="48f29-118">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="48f29-119">要获取应用程序的活动，请使用**nextLink**属性进行分页。</span><span class="sxs-lookup"><span data-stu-id="48f29-119">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="48f29-120">权限</span><span class="sxs-lookup"><span data-stu-id="48f29-120">Permissions</span></span>

<span data-ttu-id="48f29-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="48f29-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48f29-123">权限类型</span><span class="sxs-lookup"><span data-stu-id="48f29-123">Permission type</span></span>      | <span data-ttu-id="48f29-124">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="48f29-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48f29-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="48f29-125">Delegated (work or school account)</span></span> | <span data-ttu-id="48f29-126">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="48f29-126">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="48f29-127">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="48f29-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48f29-128">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="48f29-128">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="48f29-129">应用程序</span><span class="sxs-lookup"><span data-stu-id="48f29-129">Application</span></span> | <span data-ttu-id="48f29-130">不支持。</span><span class="sxs-lookup"><span data-stu-id="48f29-130">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="48f29-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="48f29-131">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="48f29-132">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="48f29-132">Optional query parameters</span></span>

<span data-ttu-id="48f29-133">此方法支持某些[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)，以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="48f29-133">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="48f29-134">支持以下查询参数：</span><span class="sxs-lookup"><span data-stu-id="48f29-134">The following query parameters are supported:</span></span>

- <span data-ttu-id="48f29-135">$ expand **historyItems**导航属性。</span><span class="sxs-lookup"><span data-stu-id="48f29-135">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="48f29-136">$top 跨页限制的最大项目数。</span><span class="sxs-lookup"><span data-stu-id="48f29-136">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="48f29-137">在**活动**或**historyItems**，如果展开的**lastModifiedDateTime**属性 $filter。</span><span class="sxs-lookup"><span data-stu-id="48f29-137">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="48f29-138">以下是支持 URL 编码的查询的一些示例。</span><span class="sxs-lookup"><span data-stu-id="48f29-138">The following are some examples of supported queries with URL encoding.</span></span>

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="48f29-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="48f29-139">Request headers</span></span>

|<span data-ttu-id="48f29-140">名称</span><span class="sxs-lookup"><span data-stu-id="48f29-140">Name</span></span> | <span data-ttu-id="48f29-141">类型</span><span class="sxs-lookup"><span data-stu-id="48f29-141">Type</span></span> | <span data-ttu-id="48f29-142">说明</span><span class="sxs-lookup"><span data-stu-id="48f29-142">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="48f29-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="48f29-143">Authorization</span></span> | <span data-ttu-id="48f29-144">string</span><span class="sxs-lookup"><span data-stu-id="48f29-144">string</span></span> | <span data-ttu-id="48f29-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="48f29-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="48f29-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="48f29-147">Request body</span></span>

<span data-ttu-id="48f29-148">不指定请求正文。</span><span class="sxs-lookup"><span data-stu-id="48f29-148">Do not specify a request body.</span></span>

## <a name="response"></a><span data-ttu-id="48f29-149">响应</span><span class="sxs-lookup"><span data-stu-id="48f29-149">Response</span></span>

<span data-ttu-id="48f29-150">如果成功，此方法返回`200 OK`与您的应用程序的用户的近期活动的响应代码。</span><span class="sxs-lookup"><span data-stu-id="48f29-150">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="48f29-151">示例</span><span class="sxs-lookup"><span data-stu-id="48f29-151">Example</span></span>

##### <a name="request"></a><span data-ttu-id="48f29-152">请求</span><span class="sxs-lookup"><span data-stu-id="48f29-152">Request</span></span>

<span data-ttu-id="48f29-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="48f29-153">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities/recent
```

##### <a name="response"></a><span data-ttu-id="48f29-154">响应</span><span class="sxs-lookup"><span data-stu-id="48f29-154">Response</span></span>

<span data-ttu-id="48f29-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="48f29-155">The following is an example of the response.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get recent activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
