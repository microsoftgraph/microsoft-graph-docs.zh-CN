# <a name="get-recent-user-activities"></a><span data-ttu-id="4b71e-101">获取最新的用户活动</span><span class="sxs-lookup"><span data-stu-id="4b71e-101">Get recent user activities</span></span>

<span data-ttu-id="4b71e-102">获得给定用户的近期活动。</span><span class="sxs-lookup"><span data-stu-id="4b71e-102">Get recent activities for a given user.</span></span> <span data-ttu-id="4b71e-103">此 OData 函数具有一些包含以使其类似"最近使用"的 API 操作的默认行为。</span><span class="sxs-lookup"><span data-stu-id="4b71e-103">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="4b71e-104">该服务将最近[historyItems](../resources/projectrome_historyitem.md)，查询，然后提取这些相关的活动。</span><span class="sxs-lookup"><span data-stu-id="4b71e-104">The service will query for the most recent [historyItems](../resources/projectrome_historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="4b71e-105">活动将根据最近**lastModified** **historyItem**上进行排序。</span><span class="sxs-lookup"><span data-stu-id="4b71e-105">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="4b71e-106">这意味着不**historyItems**活动将不包含在响应中。</span><span class="sxs-lookup"><span data-stu-id="4b71e-106">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="4b71e-107">UserActivity.ReadWrite.CreatedByApp 权限也将应用到响应，额外筛选，以便返回仅由您的应用程序创建的活动。</span><span class="sxs-lookup"><span data-stu-id="4b71e-107">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="4b71e-108">如果用户是特别活动和其他应用程序已创建较新的活动，则将此服务器端筛选可能会导致空白页。</span><span class="sxs-lookup"><span data-stu-id="4b71e-108">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="4b71e-109">要获取应用程序的活动，请使用**nextLink**属性进行分页。</span><span class="sxs-lookup"><span data-stu-id="4b71e-109">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b71e-110">权限</span><span class="sxs-lookup"><span data-stu-id="4b71e-110">Permissions</span></span>

<span data-ttu-id="4b71e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4b71e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4b71e-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b71e-113">Permission type</span></span>      | <span data-ttu-id="4b71e-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4b71e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b71e-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b71e-115">Delegated (work or school account)</span></span> | <span data-ttu-id="4b71e-116">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="4b71e-116">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="4b71e-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b71e-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b71e-118">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="4b71e-118">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="4b71e-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="4b71e-119">Application</span></span> | <span data-ttu-id="4b71e-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b71e-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b71e-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b71e-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4b71e-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4b71e-122">Optional query parameters</span></span>

<span data-ttu-id="4b71e-123">此方法支持某些[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)，以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4b71e-123">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="4b71e-124">支持以下查询参数：</span><span class="sxs-lookup"><span data-stu-id="4b71e-124">The following query parameters are supported:</span></span>

- <span data-ttu-id="4b71e-125">$ expand **historyItems**导航属性。</span><span class="sxs-lookup"><span data-stu-id="4b71e-125">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="4b71e-126">$top 跨页限制的最大项目数。</span><span class="sxs-lookup"><span data-stu-id="4b71e-126">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="4b71e-127">在**活动**或**historyItems**，如果展开的**lastModifiedDateTime**属性 $filter。</span><span class="sxs-lookup"><span data-stu-id="4b71e-127">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="4b71e-128">以下是支持 URL 编码的查询的一些示例。</span><span class="sxs-lookup"><span data-stu-id="4b71e-128">The following are some examples of supported queries with URL encoding.</span></span>

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="4b71e-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b71e-129">Request headers</span></span>

|<span data-ttu-id="4b71e-130">名称</span><span class="sxs-lookup"><span data-stu-id="4b71e-130">Name</span></span> | <span data-ttu-id="4b71e-131">类型</span><span class="sxs-lookup"><span data-stu-id="4b71e-131">Type</span></span> | <span data-ttu-id="4b71e-132">说明</span><span class="sxs-lookup"><span data-stu-id="4b71e-132">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="4b71e-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b71e-133">Authorization</span></span> | <span data-ttu-id="4b71e-134">string</span><span class="sxs-lookup"><span data-stu-id="4b71e-134">string</span></span> | <span data-ttu-id="4b71e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4b71e-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b71e-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b71e-137">Request body</span></span>

<span data-ttu-id="4b71e-138">不指定请求正文。</span><span class="sxs-lookup"><span data-stu-id="4b71e-138">Do not specify a request body.</span></span>

## <a name="response"></a><span data-ttu-id="4b71e-139">响应</span><span class="sxs-lookup"><span data-stu-id="4b71e-139">Response</span></span>

<span data-ttu-id="4b71e-140">如果成功，此方法返回`200 OK`与您的应用程序的用户的近期活动的响应代码。</span><span class="sxs-lookup"><span data-stu-id="4b71e-140">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="4b71e-141">示例</span><span class="sxs-lookup"><span data-stu-id="4b71e-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4b71e-142">请求</span><span class="sxs-lookup"><span data-stu-id="4b71e-142">Request</span></span>

<span data-ttu-id="4b71e-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4b71e-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities/recent
```

##### <a name="response"></a><span data-ttu-id="4b71e-144">响应</span><span class="sxs-lookup"><span data-stu-id="4b71e-144">Response</span></span>

<span data-ttu-id="4b71e-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4b71e-145">The following is an example of the response.</span></span>

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
              "iconUrl": "https://www.contoso.com/icon",
              "alternateText": "Contoso, Ltd.",
              "addImageQuery": false,
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
  "suppressions": [
    "Error: get_recent_activities/container/contentInfo:
      Property 'contentInfo' is of type Custom but has no custom members.",

    "Warning: get_recent_activities/container/visualElements:
      Schema validation failed on property 'visualElements' ['microsoft.graph.visualInfo']",

    "Warning: get_recent_activities/container/visualElements/content:
      Schema validation failed on property 'content' ['microsoft.graph.Json']",

    "Warning: get_recent_activities/container/visualElements/content/$schema:
      Undocumented property '$schema' [String] was not expected on resource microsoft.graph.Json.",

    "Warning: get_recent_activities/container/visualElements/content/body:
      Undocumented property 'body' [Collection(Object)] was not expected on resource microsoft.graph.Json.",

    "Warning: get_recent_activities/container/visualElements/content/type:
      Undocumented property 'type' [String] was not expected on resource microsoft.graph.Json."

  ],
  "tocPath": ""
}-->
