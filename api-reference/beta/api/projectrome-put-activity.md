---
title: 创建或替换活动
description: 创建一个新或替换现有用户活动应用程序。 如果您想要在一个请求中创建用户活动和其相关的**historyItems** ，您可以使用深层插入。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: f9dfa75f8503e9fcd9bec6f7b36840e310bf629d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520359"
---
# <a name="create-or-replace-an-activity"></a><span data-ttu-id="37f30-104">创建或替换活动</span><span class="sxs-lookup"><span data-stu-id="37f30-104">Create or replace an activity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37f30-105">创建一个新或替换现有用户活动应用程序。</span><span class="sxs-lookup"><span data-stu-id="37f30-105">Create a new or replace an existing user activity for your app.</span></span> <span data-ttu-id="37f30-106">如果您想要在一个请求中创建用户活动和其相关的**historyItems** ，您可以使用[深层插入](projectrome-put-activity.md#example-2---deep-insert)。</span><span class="sxs-lookup"><span data-stu-id="37f30-106">If you'd like to create a user activity and its related **historyItems** in one request, you can use [deep insert](projectrome-put-activity.md#example-2---deep-insert).</span></span>

## <a name="permissions"></a><span data-ttu-id="37f30-107">权限</span><span class="sxs-lookup"><span data-stu-id="37f30-107">Permissions</span></span>

<span data-ttu-id="37f30-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="37f30-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="37f30-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="37f30-110">Permission type</span></span>      | <span data-ttu-id="37f30-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="37f30-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37f30-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="37f30-112">Delegated (work or school account)</span></span> | <span data-ttu-id="37f30-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="37f30-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="37f30-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="37f30-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37f30-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="37f30-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="37f30-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="37f30-116">Application</span></span> | <span data-ttu-id="37f30-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="37f30-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="37f30-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="37f30-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{appActivityId}
```

><span data-ttu-id="37f30-119">**注意：** 在 URL appActivityId 需要 URL 安全 （除 RFC 2396 必须将未保留的字符转换为十六进制表示形式为所有字符），但原始 appActivityId 不必是安全的 URL。</span><span class="sxs-lookup"><span data-stu-id="37f30-119">**Note:** The appActivityId in the URL needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37f30-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="37f30-120">Request headers</span></span>

|<span data-ttu-id="37f30-121">名称</span><span class="sxs-lookup"><span data-stu-id="37f30-121">Name</span></span> | <span data-ttu-id="37f30-122">类型</span><span class="sxs-lookup"><span data-stu-id="37f30-122">Type</span></span> | <span data-ttu-id="37f30-123">说明</span><span class="sxs-lookup"><span data-stu-id="37f30-123">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="37f30-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="37f30-124">Authorization</span></span> | <span data-ttu-id="37f30-125">string</span><span class="sxs-lookup"><span data-stu-id="37f30-125">string</span></span> | <span data-ttu-id="37f30-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="37f30-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="37f30-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="37f30-128">Request body</span></span>

<span data-ttu-id="37f30-129">在请求正文中，提供的[活动](../resources/projectrome-activity.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37f30-129">In the request body, supply a JSON representation of an [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="37f30-130">响应</span><span class="sxs-lookup"><span data-stu-id="37f30-130">Response</span></span>

<span data-ttu-id="37f30-131">如果成功，此方法返回`201 Created`如果创建活动的响应代码或`200 OK`如果活动的正被替换。</span><span class="sxs-lookup"><span data-stu-id="37f30-131">If successful, this method returns the `201 Created` response code if the activity was created or `200 OK` if the activity was replaced.</span></span>

## <a name="example-1"></a><span data-ttu-id="37f30-132">示例 1</span><span class="sxs-lookup"><span data-stu-id="37f30-132">Example 1</span></span>

#### <a name="request"></a><span data-ttu-id="37f30-133">请求</span><span class="sxs-lookup"><span data-stu-id="37f30-133">Request</span></span>

<span data-ttu-id="37f30-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="37f30-134">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/beta/me/activities/%2Farticle%3F12345
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
            "addImageQuery": "false"
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

#### <a name="response"></a><span data-ttu-id="37f30-135">响应</span><span class="sxs-lookup"><span data-stu-id="37f30-135">Response</span></span>

<span data-ttu-id="37f30-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="37f30-136">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.activity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/beta/me/activities/14332800362997268276

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

## <a name="example-2---deep-insert"></a><span data-ttu-id="37f30-137">示例 2-深层插入</span><span class="sxs-lookup"><span data-stu-id="37f30-137">Example 2 - Deep insert</span></span>

#### <a name="request"></a><span data-ttu-id="37f30-138">请求</span><span class="sxs-lookup"><span data-stu-id="37f30-138">Request</span></span>

<span data-ttu-id="37f30-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="37f30-139">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/beta/me/activities/%2Farticle%3F12345
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
            "addImageQuery": "false",
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

#### <a name="response"></a><span data-ttu-id="37f30-140">响应</span><span class="sxs-lookup"><span data-stu-id="37f30-140">Response</span></span>

<span data-ttu-id="37f30-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="37f30-141">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.activity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/beta/me/activities/14332800362997268276

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
<!--
{
  "type": "#page.annotation",
  "description": "Upsert activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/projectrome-put-activity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
