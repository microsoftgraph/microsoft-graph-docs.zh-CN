# <a name="create-or-replace-an-activity"></a><span data-ttu-id="728e1-101">创建或替换活动</span><span class="sxs-lookup"><span data-stu-id="728e1-101">Create or replace an activity</span></span>

<span data-ttu-id="728e1-102">创建一个新或替换现有用户活动应用程序。</span><span class="sxs-lookup"><span data-stu-id="728e1-102">Create a new or replace an existing user activity for your app.</span></span> <span data-ttu-id="728e1-103">如果您想要在一个请求中创建用户活动和其相关的**historyItems** ，您可以使用[深层插入](projectrome_put_activity.md#example-2---deep-insert)。</span><span class="sxs-lookup"><span data-stu-id="728e1-103">If you'd like to create a user activity and its related **historyItems** in one request, you can use [deep insert](projectrome_put_activity.md#example-2---deep-insert).</span></span>

## <a name="permissions"></a><span data-ttu-id="728e1-104">权限</span><span class="sxs-lookup"><span data-stu-id="728e1-104">Permissions</span></span>

<span data-ttu-id="728e1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="728e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="728e1-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="728e1-107">Permission type</span></span>      | <span data-ttu-id="728e1-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="728e1-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="728e1-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="728e1-109">Delegated (work or school account)</span></span> | <span data-ttu-id="728e1-110">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="728e1-110">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="728e1-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="728e1-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="728e1-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="728e1-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="728e1-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="728e1-113">Application</span></span> | <span data-ttu-id="728e1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="728e1-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="728e1-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="728e1-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{appActivityId}
```

><span data-ttu-id="728e1-116">**注意：** 在 URL appActivityId 需要 URL 安全 （除 RFC 2396 必须将未保留的字符转换为十六进制表示形式为所有字符），但原始 appActivityId 不必是安全的 URL。</span><span class="sxs-lookup"><span data-stu-id="728e1-116">**Note:** The appActivityId in the URL needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span>

## <a name="request-headers"></a><span data-ttu-id="728e1-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="728e1-117">Request headers</span></span>

|<span data-ttu-id="728e1-118">名称</span><span class="sxs-lookup"><span data-stu-id="728e1-118">Name</span></span> | <span data-ttu-id="728e1-119">类型</span><span class="sxs-lookup"><span data-stu-id="728e1-119">Type</span></span> | <span data-ttu-id="728e1-120">说明</span><span class="sxs-lookup"><span data-stu-id="728e1-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="728e1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="728e1-121">Authorization</span></span> | <span data-ttu-id="728e1-122">string</span><span class="sxs-lookup"><span data-stu-id="728e1-122">string</span></span> | <span data-ttu-id="728e1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="728e1-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="728e1-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="728e1-125">Request body</span></span>

<span data-ttu-id="728e1-126">在请求正文中，提供的[活动](../resources/projectrome_activity.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="728e1-126">In the request body, supply a JSON representation of an [activity](../resources/projectrome_activity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="728e1-127">响应</span><span class="sxs-lookup"><span data-stu-id="728e1-127">Response</span></span>

<span data-ttu-id="728e1-128">如果成功，此方法返回`201 Created`如果创建活动的响应代码或`200 OK`如果活动的正被替换。</span><span class="sxs-lookup"><span data-stu-id="728e1-128">If successful, this method returns the `201 Created` response code if the activity was created or `200 OK` if the activity was replaced.</span></span>

## <a name="example-1"></a><span data-ttu-id="728e1-129">示例 1</span><span class="sxs-lookup"><span data-stu-id="728e1-129">Example 1</span></span>

#### <a name="request"></a><span data-ttu-id="728e1-130">请求</span><span class="sxs-lookup"><span data-stu-id="728e1-130">Request</span></span>

<span data-ttu-id="728e1-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="728e1-131">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/%2Farticle%3F12345
Content-type: application/json
Content-length: 364

{
    "appActivityId": "/article?12345",
    "activitySourceHost": "https://www.contoso.com",
    "userTimezone": "Africa/Casablanca",
    "appDisplayName": "Contoso, Ltd.",
    "activationUrl": "https://www.contoso.com/article?id=12345",
    "contentUrl": "https://www.contoso.com/article?id=12345",
    "fallbackUrl": "https://www.contoso.com/article?id=12345",
    "contentInfo": {
        "@context": "https://schema.org",
        "@type": "Article",
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
    "visualElements": {
        "attribution": {
            "iconUrl": "https://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": false,
        },
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "backgroundColor": "#ff0000",
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
        "content": {
            "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
            "type": "AdaptiveCard",
            "body":
            [{
                "type": "TextBlock",
                "text": "Contoso MainPage"
            }]
        }
    }
}
```

#### <a name="response"></a><span data-ttu-id="728e1-132">响应</span><span class="sxs-lookup"><span data-stu-id="728e1-132">Response</span></span>

<span data-ttu-id="728e1-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="728e1-133">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.userActivity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/v1.0/me/activities/14332800362997268276

{
    "activitySourceHost": "https://contoso.com",
    "createdDateTime": "2017-06-09T20:54:43.969Z",
    "lastModifiedDateTime": "2017-06-09T20:54:43.969Z",
    "id": "14332800362997268276",
    "appActivityId": "/article?12345",
    "status":"updated",
    "expirationDateTime": "2017-02-26T20:20:48.114Z",
    "id": "14332800362997268276",
    "visualElements": {
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "attribution": {
            "iconUrl": "https://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": false
        },
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
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
}
```

## <a name="example-2---deep-insert"></a><span data-ttu-id="728e1-134">示例 2-深层插入</span><span class="sxs-lookup"><span data-stu-id="728e1-134">Example 2 - Deep insert</span></span>

#### <a name="request"></a><span data-ttu-id="728e1-135">请求</span><span class="sxs-lookup"><span data-stu-id="728e1-135">Request</span></span>

<span data-ttu-id="728e1-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="728e1-136">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/%2Farticle%3F12345
Content-type: application/json
Content-length: 364

{
    "appActivityId": "/article?12345",
    "activitySourceHost": "https://www.contoso.com",
    "userTimezone": "Africa/Casablanca",
    "appDisplayName": "Contoso, Ltd.",
    "activationUrl": "https://www.contoso.com/article?id=12345",
    "contentUrl": "https://www.contoso.com/article?id=12345",
    "fallbackUrl": "https://www.contoso.com/article?id=12345",
    "contentInfo": {
        "@context": "https://schema.org",
        "@type": "Article",
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
    "visualElements": {
        "attribution": {
            "iconUrl": "https://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": false,
        },
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "backgroundColor": "#ff0000",
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
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
    "historyItems":[
        {
            "userTimezone": "Africa/Casablanca",
            "startedDateTime": "2018-02-26T20:54:04.345Z",
            "lastActiveDateTime": "2018-02-26T20:54:24.345Z",
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="728e1-137">响应</span><span class="sxs-lookup"><span data-stu-id="728e1-137">Response</span></span>

<span data-ttu-id="728e1-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="728e1-138">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.userActivity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/v1.0/me/activities/14332800362997268276

{
    "activitySourceHost": "https://contoso.com",
    "createdDateTime": "2017-06-09T20:54:43.969Z",
    "lastModifiedDateTime": "2017-06-09T20:54:43.969Z",
    "id": "14332800362997268276",
    "appActivityId": "/article?12345",
    "status":"updated",
    "expirationDateTime": "2017-02-26T20:20:48.114Z",
    "id": "14332800362997268276",
    "visualElements": {
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "attribution": {
            "iconUrl": "https://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": false
        },
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
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
    "historyItems":[
        {
            "status": "updated",
            "userTimezone": "Africa/Casablanca",
            "createdDateTime": "2018-04-12T21:42:42.495Z",
            "lastModifiedDateTime": "2018-04-12T21:42:42.495Z",
            "id": "61fc8f36-919f-4b73-89d4-1cb7b159d912",
            "startedDateTime": "2018-02-26T20:54:04.345Z",
            "lastActiveDateTime": "2018-02-26T20:54:24.345Z",
            "expirationDateTime": "2018-05-12T21:42:42.495Z",
            "activeDurationSeconds": 20
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upsert activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
