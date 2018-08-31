# <a name="get-user-activities"></a><span data-ttu-id="fb46c-101">获取用户活动</span><span class="sxs-lookup"><span data-stu-id="fb46c-101">Get user activities</span></span>

<span data-ttu-id="fb46c-102">获得给定用户的活动。</span><span class="sxs-lookup"><span data-stu-id="fb46c-102">Get activities for a given user.</span></span> <span data-ttu-id="fb46c-103">与**最近**的 OData 函数不同的是，将返回不含历史记录的活动。</span><span class="sxs-lookup"><span data-stu-id="fb46c-103">Unlike the **recent** OData function, activities without histories will be returned.</span></span> <span data-ttu-id="fb46c-104">权限 UserActivity.ReadWrite.CreatedByApp 将额外将筛选应用于响应，以便返回仅由您的应用程序创建的活动。</span><span class="sxs-lookup"><span data-stu-id="fb46c-104">The permission UserActivity.ReadWrite.CreatedByApp will apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="fb46c-105">如果用户是特别活动和其他应用程序已创建较新的活动，则将此服务器端筛选可能会导致空白页。</span><span class="sxs-lookup"><span data-stu-id="fb46c-105">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="fb46c-106">要获取应用程序的活动，请使用 **nextLink** 属性进行分页。</span><span class="sxs-lookup"><span data-stu-id="fb46c-106">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb46c-107">权限</span><span class="sxs-lookup"><span data-stu-id="fb46c-107">Permissions</span></span>

<span data-ttu-id="fb46c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fb46c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fb46c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb46c-110">Permission type</span></span>      | <span data-ttu-id="fb46c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fb46c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb46c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb46c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fb46c-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="fb46c-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="fb46c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb46c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb46c-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="fb46c-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="fb46c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb46c-116">Application</span></span> | <span data-ttu-id="fb46c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb46c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb46c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb46c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fb46c-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fb46c-119">Optional query parameters</span></span>

<span data-ttu-id="fb46c-120">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fb46c-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span> <span data-ttu-id="fb46c-121">支持以下查询参数：</span><span class="sxs-lookup"><span data-stu-id="fb46c-121">The following query parameters are supported:</span></span>

- <span data-ttu-id="fb46c-122">**historyItems** 导航属性的 $expand。</span><span class="sxs-lookup"><span data-stu-id="fb46c-122">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="fb46c-123">限制跨页的最大项目数的 $top。</span><span class="sxs-lookup"><span data-stu-id="fb46c-123">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="fb46c-124">活动的 **lastModifiedDateTime** 属性上的 $filter 或 **historyItems**（如果扩展）。</span><span class="sxs-lookup"><span data-stu-id="fb46c-124">$filter on the **lastModifiedDateTime** property for either activities or **historyItems**, if expanded.</span></span>

<span data-ttu-id="fb46c-125">以下是支持 URL 编码的查询的一些示例：</span><span class="sxs-lookup"><span data-stu-id="fb46c-125">The following are some examples of supported queries with URL encoding:</span></span>

```
/me/activities?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="fb46c-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb46c-126">Request headers</span></span>

|<span data-ttu-id="fb46c-127">名称</span><span class="sxs-lookup"><span data-stu-id="fb46c-127">Name</span></span> | <span data-ttu-id="fb46c-128">类型</span><span class="sxs-lookup"><span data-stu-id="fb46c-128">Type</span></span> | <span data-ttu-id="fb46c-129">说明</span><span class="sxs-lookup"><span data-stu-id="fb46c-129">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="fb46c-130">授权</span><span class="sxs-lookup"><span data-stu-id="fb46c-130">Authorization</span></span> | <span data-ttu-id="fb46c-131">字符串</span><span class="sxs-lookup"><span data-stu-id="fb46c-131">string</span></span> | <span data-ttu-id="fb46c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fb46c-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb46c-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb46c-134">Request body</span></span>

<span data-ttu-id="fb46c-135">无请求正文。</span><span class="sxs-lookup"><span data-stu-id="fb46c-135">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="fb46c-136">响应</span><span class="sxs-lookup"><span data-stu-id="fb46c-136">Response</span></span>

<span data-ttu-id="fb46c-137">如果成功，`200 OK` 此方法为您的应用程序返回用户活动的  响应代码。</span><span class="sxs-lookup"><span data-stu-id="fb46c-137">If successful, this method returns the `200 OK` response code with the user's activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="fb46c-138">示例</span><span class="sxs-lookup"><span data-stu-id="fb46c-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fb46c-139">请求</span><span class="sxs-lookup"><span data-stu-id="fb46c-139">Request</span></span>

<span data-ttu-id="fb46c-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fb46c-140">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities
```

##### <a name="response"></a><span data-ttu-id="fb46c-141">响应</span><span class="sxs-lookup"><span data-stu-id="fb46c-141">Response</span></span>

<span data-ttu-id="fb46c-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fb46c-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.activity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/activities?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
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
  "description": "Get activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
