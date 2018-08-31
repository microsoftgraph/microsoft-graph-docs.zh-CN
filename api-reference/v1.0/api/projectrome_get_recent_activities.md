# <a name="get-recent-user-activities"></a><span data-ttu-id="e8ba7-101">获取最近的用户活动</span><span class="sxs-lookup"><span data-stu-id="e8ba7-101">Get recent activities</span></span>

<span data-ttu-id="e8ba7-102">获得给定用户的最近活动。</span><span class="sxs-lookup"><span data-stu-id="e8ba7-102">Get recent activities for a given user.</span></span> <span data-ttu-id="e8ba7-103">这个 OData 函数具有一些包含以使其类似“最近使用”的 API 操作的默认行为。</span><span class="sxs-lookup"><span data-stu-id="e8ba7-103">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="e8ba7-104">该服务将查询最近的 [historyItems](../resources/projectrome_historyitem.md)，然后提取那些相关的活动。</span><span class="sxs-lookup"><span data-stu-id="e8ba7-104">The service will query for the most recent [historyItems](../resources/projectrome_historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="e8ba7-105">活动将根据 **historyItem** 上最近的 **lastModified** 进行排序。</span><span class="sxs-lookup"><span data-stu-id="e8ba7-105">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="e8ba7-106">这意味着没有 **historyItems** 的活动将不包括在响应中。</span><span class="sxs-lookup"><span data-stu-id="e8ba7-106">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="e8ba7-107">UserActivity.ReadWrite.CreatedByApp 权限还会将额外的筛选应用于响应，以便返回仅由你的应用程序创建的活动。</span><span class="sxs-lookup"><span data-stu-id="e8ba7-107">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="e8ba7-108">如果用户特别活跃并且其他应用程序已创建较新的活动，则将此服务器端筛选可能会导致空白页。</span><span class="sxs-lookup"><span data-stu-id="e8ba7-108">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="e8ba7-109">要获取应用程序的活动，请使用 **nextLink** 属性进行分页。</span><span class="sxs-lookup"><span data-stu-id="e8ba7-109">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8ba7-110">权限</span><span class="sxs-lookup"><span data-stu-id="e8ba7-110">Permissions</span></span>

<span data-ttu-id="e8ba7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e8ba7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e8ba7-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8ba7-113">Permission type</span></span>      | <span data-ttu-id="e8ba7-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e8ba7-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8ba7-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8ba7-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e8ba7-116">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="e8ba7-116">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="e8ba7-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8ba7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8ba7-118">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="e8ba7-118">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="e8ba7-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8ba7-119">Application</span></span> | <span data-ttu-id="e8ba7-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8ba7-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8ba7-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8ba7-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8ba7-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e8ba7-122">Optional query parameters</span></span>

<span data-ttu-id="e8ba7-123">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e8ba7-123">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span> <span data-ttu-id="e8ba7-124">支持以下查询参数：</span><span class="sxs-lookup"><span data-stu-id="e8ba7-124">The following query parameters are supported:</span></span>

- <span data-ttu-id="e8ba7-125">**historyItems** 导航属性的 $expand。</span><span class="sxs-lookup"><span data-stu-id="e8ba7-125">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="e8ba7-126">限制跨页的最大项目数的 $top。</span><span class="sxs-lookup"><span data-stu-id="e8ba7-126">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="e8ba7-127">在**活动**或 **historyItems** 的 **lastModifiedDateTime** 属性上的 $filter（如果扩展）。</span><span class="sxs-lookup"><span data-stu-id="e8ba7-127">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="e8ba7-128">以下是支持 URL 编码查询的一些示例。</span><span class="sxs-lookup"><span data-stu-id="e8ba7-128">The following are some examples of supported queries with URL encoding.</span></span>

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="e8ba7-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8ba7-129">Request headers</span></span>

|<span data-ttu-id="e8ba7-130">名称</span><span class="sxs-lookup"><span data-stu-id="e8ba7-130">Name</span></span> | <span data-ttu-id="e8ba7-131">类型</span><span class="sxs-lookup"><span data-stu-id="e8ba7-131">Type</span></span> | <span data-ttu-id="e8ba7-132">说明</span><span class="sxs-lookup"><span data-stu-id="e8ba7-132">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="e8ba7-133">授权</span><span class="sxs-lookup"><span data-stu-id="e8ba7-133">Authorization</span></span> | <span data-ttu-id="e8ba7-134">字符串</span><span class="sxs-lookup"><span data-stu-id="e8ba7-134">string</span></span> | <span data-ttu-id="e8ba7-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e8ba7-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8ba7-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8ba7-137">Request body</span></span>

<span data-ttu-id="e8ba7-138">请勿指定请求正文。</span><span class="sxs-lookup"><span data-stu-id="e8ba7-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8ba7-139">响应</span><span class="sxs-lookup"><span data-stu-id="e8ba7-139">Response</span></span>

<span data-ttu-id="e8ba7-140">如果成功，此方法返回您的应用程序用户最近活动的 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e8ba7-140">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="e8ba7-141">示例</span><span class="sxs-lookup"><span data-stu-id="e8ba7-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e8ba7-142">请求</span><span class="sxs-lookup"><span data-stu-id="e8ba7-142">Request</span></span>

<span data-ttu-id="e8ba7-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e8ba7-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities/recent
```

##### <a name="response"></a><span data-ttu-id="e8ba7-144">响应</span><span class="sxs-lookup"><span data-stu-id="e8ba7-144">Response</span></span>

<span data-ttu-id="e8ba7-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e8ba7-145">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userActivity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/activities/recent?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
    "value": [{
        "@odata.type": "#microsoft.graph.userActivity",
        "activitySourceHost": "https://www.contoso.com",
        "createdDateTime": "2018-02-26T18:34:29.592Z",
        "lastModifiedDateTime": "2018-02-26T18:34:29.607Z",
        "id": "5347642601316252694",
        "appActivityId": "/article?12345",
        "visualElements": {
            "attribution": {
              "iconUrl": "http://www.contoso.com/icon",
              "alternateText": "Contoso, Ltd.",
              "addImageQuery": false,
              },
            "displayText": "Contoso How-To: How to Tie a Reef Knot",
            "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
            "backgroundColor": "#ff0000",
            "content": {
              "$schema": "http://adaptivecards.io/schemas/adaptive-card.json",
              "type": "AdaptiveCard",
              "body":
              [{
                  "type": "TextBlock",
                  "text": "Contoso MainPage"
              }]
            }
        },
        "activationUrl": "http://www.contoso.com/article?id=12345",
        "appDisplayName": "Contoso, Ltd.",
        "userTimezone": "Africa/Casablanca",
        "fallbackUrl": "http://www.contoso.com/article?id=12345",
        "contentUrl": "http://www.contoso.com/article?id=12345",
        "contentInfo": {
            "@context": "http://schema.org",
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
  "suppressions": [
    "Error: get_recent_activities/container/contentInfo:
      Property 'contentInfo' is of type Custom but has no custom members."
  ],
  "tocPath": ""
}-->
