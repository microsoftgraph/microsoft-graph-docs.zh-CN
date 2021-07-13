---
title: 获取最近的用户活动
description: " API。 该服务将查询最新的 historyItems，然后提取这些相关活动。 活动将按照 **historyItem** 上的最新 **lastModified** 进行排序。 这意味着没有 **historyItems** 的活动不会包含在响应中。 UserActivity.ReadWrite.CreatedByApp 权限还将对响应应用额外筛选，以便仅返回由应用程序创建的活动。 如果用户特别活动并且其他应用程序已创建最近的活动，则此服务器端筛选可能会导致空页。 若要获取应用程序的活动，请使用 **nextLink** 属性分页。"
localization_priority: Normal
ms.prod: project-rome
doc_type: apiPageType
author: ailae
ms.openlocfilehash: 27361d56e62e1ea255c2a0e9e3b6d3e0b45ee44e
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401503"
---
# <a name="get-recent-user-activities"></a><span data-ttu-id="b1003-109">获取最近的用户活动</span><span class="sxs-lookup"><span data-stu-id="b1003-109">Get recent user activities</span></span>

<span data-ttu-id="b1003-110">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1003-110">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1003-111">获取给定用户的最近活动。</span><span class="sxs-lookup"><span data-stu-id="b1003-111">Get recent activities for a given user.</span></span> <span data-ttu-id="b1003-112">此 OData 函数包含一些默认行为，可使其像"最近使用的"API 一样运行。</span><span class="sxs-lookup"><span data-stu-id="b1003-112">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="b1003-113">该服务将查询最新的 [historyItems](../resources/projectrome-historyitem.md)，然后拉取这些相关活动。</span><span class="sxs-lookup"><span data-stu-id="b1003-113">The service will query for the most recent [historyItems](../resources/projectrome-historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="b1003-114">活动将按照 **historyItem** 上的最新 **lastModified** 进行排序。</span><span class="sxs-lookup"><span data-stu-id="b1003-114">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="b1003-115">这意味着没有 **historyItems** 的活动不会包含在响应中。</span><span class="sxs-lookup"><span data-stu-id="b1003-115">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="b1003-116">UserActivity.ReadWrite.CreatedByApp 权限还将对响应应用额外筛选，以便仅返回由应用程序创建的活动。</span><span class="sxs-lookup"><span data-stu-id="b1003-116">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="b1003-117">如果用户特别活动并且其他应用程序已创建最近的活动，则此服务器端筛选可能会导致空页。</span><span class="sxs-lookup"><span data-stu-id="b1003-117">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="b1003-118">若要获取应用程序的活动，请使用 **nextLink** 属性分页。</span><span class="sxs-lookup"><span data-stu-id="b1003-118">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1003-119">权限</span><span class="sxs-lookup"><span data-stu-id="b1003-119">Permissions</span></span>

<span data-ttu-id="b1003-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b1003-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1003-122">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1003-122">Permission type</span></span>      | <span data-ttu-id="b1003-123">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b1003-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1003-124">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1003-124">Delegated (work or school account)</span></span> | <span data-ttu-id="b1003-125">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="b1003-125">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="b1003-126">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1003-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1003-127">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="b1003-127">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="b1003-128">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1003-128">Application</span></span> | <span data-ttu-id="b1003-129">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1003-129">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1003-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1003-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b1003-131">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b1003-131">Optional query parameters</span></span>

<span data-ttu-id="b1003-132">此方法支持一些 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b1003-132">This method supports some [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span> <span data-ttu-id="b1003-133">支持以下查询参数：</span><span class="sxs-lookup"><span data-stu-id="b1003-133">The following query parameters are supported:</span></span>

- <span data-ttu-id="b1003-134">$expand **historyItems 导航属性** 。</span><span class="sxs-lookup"><span data-stu-id="b1003-134">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="b1003-135">$top限制页面的最大项目数。</span><span class="sxs-lookup"><span data-stu-id="b1003-135">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="b1003-136">$filter活动或 **historyItems** 的 **lastModifiedDateTime** 属性（如果展开）。 </span><span class="sxs-lookup"><span data-stu-id="b1003-136">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="b1003-137">下面是使用 URL 编码的受支持查询的一些示例。</span><span class="sxs-lookup"><span data-stu-id="b1003-137">The following are some examples of supported queries with URL encoding.</span></span>

```http
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="b1003-138">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1003-138">Request headers</span></span>

|<span data-ttu-id="b1003-139">名称</span><span class="sxs-lookup"><span data-stu-id="b1003-139">Name</span></span> | <span data-ttu-id="b1003-140">类型</span><span class="sxs-lookup"><span data-stu-id="b1003-140">Type</span></span> | <span data-ttu-id="b1003-141">说明</span><span class="sxs-lookup"><span data-stu-id="b1003-141">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="b1003-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1003-142">Authorization</span></span> | <span data-ttu-id="b1003-143">string</span><span class="sxs-lookup"><span data-stu-id="b1003-143">string</span></span> | <span data-ttu-id="b1003-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b1003-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1003-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1003-146">Request body</span></span>

<span data-ttu-id="b1003-147">不指定请求正文。</span><span class="sxs-lookup"><span data-stu-id="b1003-147">Do not specify a request body.</span></span>

## <a name="response"></a><span data-ttu-id="b1003-148">响应</span><span class="sxs-lookup"><span data-stu-id="b1003-148">Response</span></span>

<span data-ttu-id="b1003-149">如果成功，此方法将返回响应代码以及用户 `200 OK` 最近针对您的应用程序的活动。</span><span class="sxs-lookup"><span data-stu-id="b1003-149">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="b1003-150">示例</span><span class="sxs-lookup"><span data-stu-id="b1003-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1003-151">请求</span><span class="sxs-lookup"><span data-stu-id="b1003-151">Request</span></span>

<span data-ttu-id="b1003-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b1003-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities/recent
```

### <a name="response"></a><span data-ttu-id="b1003-153">响应</span><span class="sxs-lookup"><span data-stu-id="b1003-153">Response</span></span>

<span data-ttu-id="b1003-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b1003-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.activity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(userActivity)",
   "@odata.nextLink":"https://graph.microsoft.com/beta/me/activities/recent?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
   "value":[
      {
         "@odata.type":"#microsoft.graph.activity",
         "activitySourceHost":"https://www.contoso.com",
         "createdDateTime":"2018-02-26T18:34:29.592Z",
         "lastModifiedDateTime":"2018-02-26T18:34:29.607Z",
         "id":"5347642601316252694",
         "appActivityId":"/article?12345",
         "visualElements":{
            "attribution":{
               "iconUrl":"https://www.contoso.com/icon",
               "alternateText":"Contoso, Ltd.",
               "addImageQuery":"false"
            },
            "displayText":"Contoso How-To: How to Tie a Reef Knot",
            "description":"How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
            "backgroundColor":"#ff0000",
            "content":{
               "$schema":"https://adaptivecards.io/schemas/adaptive-card.json",
               "type":"AdaptiveCard",
               "body":[
                  {
                     "type":"TextBlock",
                     "text":"Contoso MainPage"
                  }
               ]
            }
         },
         "activationUrl":"https://www.contoso.com/article?id=12345",
         "appDisplayName":"Contoso, Ltd.",
         "userTimezone":"Africa/Casablanca",
         "fallbackUrl":"https://www.contoso.com/article?id=12345",
         "contentUrl":"https://www.contoso.com/article?id=12345",
         "contentInfo":{
            "@context":"https://schema.org",
            "@type":"Article",
            "author":"John Doe",
            "name":"How to Tie a Reef Knot"
         },
         "expirationDateTime":"2018-03-28T18:34:29.607Z",
         "status":"updated"
      }
   ]
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
