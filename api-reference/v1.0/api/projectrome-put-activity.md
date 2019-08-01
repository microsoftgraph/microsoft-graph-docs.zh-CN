---
title: 创建或替换活动
description: 为您的应用程序创建新的或替换现有的用户活动。 如果您想要在一个请求中创建用户活动及其相关的**historyItems** , 则可以使用深层插入。
localization_priority: Normal
ms.prod: project-rome
author: ''
doc_type: apiPageType
ms.openlocfilehash: 8f80d17f64b4f04816670d8e007ca7db82755c0c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025370"
---
# <a name="create-or-replace-an-activity"></a><span data-ttu-id="036e7-104">创建或替换活动</span><span class="sxs-lookup"><span data-stu-id="036e7-104">Create or replace an activity</span></span>

<span data-ttu-id="036e7-105">为您的应用程序创建新的或替换现有的用户活动。</span><span class="sxs-lookup"><span data-stu-id="036e7-105">Create a new or replace an existing user activity for your app.</span></span> <span data-ttu-id="036e7-106">如果您想要在一个请求中创建用户活动及其相关的**historyItems** , 则可以使用[深层插入](#example-2-deep-insert)。</span><span class="sxs-lookup"><span data-stu-id="036e7-106">If you'd like to create a user activity and its related **historyItems** in one request, you can use [deep insert](#example-2-deep-insert).</span></span>

## <a name="permissions"></a><span data-ttu-id="036e7-107">权限</span><span class="sxs-lookup"><span data-stu-id="036e7-107">Permissions</span></span>

<span data-ttu-id="036e7-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="036e7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="036e7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="036e7-110">Permission type</span></span>                        | <span data-ttu-id="036e7-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="036e7-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="036e7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="036e7-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="036e7-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="036e7-113">UserActivity.ReadWrite.CreatedByApp</span></span> |
| <span data-ttu-id="036e7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="036e7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="036e7-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="036e7-115">UserActivity.ReadWrite.CreatedByApp</span></span> |
| <span data-ttu-id="036e7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="036e7-116">Application</span></span>                            | <span data-ttu-id="036e7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="036e7-117">Not supported.</span></span>                      |

## <a name="http-request"></a><span data-ttu-id="036e7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="036e7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{appActivityId}
```

> <span data-ttu-id="036e7-119">**注意:** URL 中的 appActivityId 需要是 URL 安全的 (除 RFC 2396 非保留字符之外的所有字符都必须转换为十六进制表示形式), 但原始 appActivityId 不必是 URL 安全的。</span><span class="sxs-lookup"><span data-stu-id="036e7-119">**Note:** The appActivityId in the URL needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span>

## <a name="request-headers"></a><span data-ttu-id="036e7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="036e7-120">Request headers</span></span>

| <span data-ttu-id="036e7-121">名称</span><span class="sxs-lookup"><span data-stu-id="036e7-121">Name</span></span>          | <span data-ttu-id="036e7-122">类型</span><span class="sxs-lookup"><span data-stu-id="036e7-122">Type</span></span>   | <span data-ttu-id="036e7-123">说明</span><span class="sxs-lookup"><span data-stu-id="036e7-123">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="036e7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="036e7-124">Authorization</span></span> | <span data-ttu-id="036e7-125">string</span><span class="sxs-lookup"><span data-stu-id="036e7-125">string</span></span> | <span data-ttu-id="036e7-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="036e7-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="036e7-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="036e7-128">Request body</span></span>

<span data-ttu-id="036e7-129">在请求正文中, 提供[活动](../resources/projectrome-activity.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="036e7-129">In the request body, supply a JSON representation of an [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="036e7-130">响应</span><span class="sxs-lookup"><span data-stu-id="036e7-130">Response</span></span>

<span data-ttu-id="036e7-131">如果成功, 此方法将在`201 Created`创建活动或`200 OK`替换活动时返回响应代码。</span><span class="sxs-lookup"><span data-stu-id="036e7-131">If successful, this method returns the `201 Created` response code if the activity was created or `200 OK` if the activity was replaced.</span></span>

## <a name="examples"></a><span data-ttu-id="036e7-132">示例</span><span class="sxs-lookup"><span data-stu-id="036e7-132">Examples</span></span>

### <a name="example-1-create-an-activity"></a><span data-ttu-id="036e7-133">示例 1: 创建活动</span><span class="sxs-lookup"><span data-stu-id="036e7-133">Example 1: Create an activity</span></span>

#### <a name="request"></a><span data-ttu-id="036e7-134">请求</span><span class="sxs-lookup"><span data-stu-id="036e7-134">Request</span></span>

<span data-ttu-id="036e7-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="036e7-135">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/%2Farticle%3F12345
Content-type: application/json

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
      "addImageQuery": false
    },
    "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
    "backgroundColor": "#ff0000",
    "displayText": "Contoso How-To: How to Tie a Reef Knot",
    "content": {
      "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
      "type": "AdaptiveCard",
      "body": [
        {
          "type": "TextBlock",
          "text": "Contoso MainPage"
        }
      ]
    }
  }
}
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="036e7-136">响应</span><span class="sxs-lookup"><span data-stu-id="036e7-136">Response</span></span>

<span data-ttu-id="036e7-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="036e7-137">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.userActivity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "activitySourceHost": "https://contoso.com",
  "createdDateTime": "2017-06-09T20:54:43.969Z",
  "lastModifiedDateTime": "2017-06-09T20:54:43.969Z",
  "id": "14332800362997268276",
  "appActivityId": "/article?12345",
  "status": "updated",
  "expirationDateTime": "2017-02-26T20:20:48.114Z",
  "visualElements": {
    "displayText": "Contoso How-To: How to Tie a Reef Knot",
    "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
    "attribution": {
      "iconUrl": "https://www.contoso.com/icon",
      "alternateText": "Contoso, Ltd.",
      "addImageQuery": "false"
    },
    "backgroundColor": "#ff0000",
    "content": {
      "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
      "type": "AdaptiveCard",
      "body": [
        {
          "type": "TextBlock",
          "text": "Contoso MainPage"
        }
      ]
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
  }
}
```

### <a name="example-2-deep-insert"></a><span data-ttu-id="036e7-138">示例 2: 深层插入</span><span class="sxs-lookup"><span data-stu-id="036e7-138">Example 2: Deep insert</span></span>

<span data-ttu-id="036e7-139">本示例在一个请求中为该活动创建一个新活动和一个历史记录项。</span><span class="sxs-lookup"><span data-stu-id="036e7-139">This example creates a new activity and a history item for that activity in one request.</span></span>

#### <a name="request"></a><span data-ttu-id="036e7-140">请求</span><span class="sxs-lookup"><span data-stu-id="036e7-140">Request</span></span>

<span data-ttu-id="036e7-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="036e7-141">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/%2Farticle%3F12345
Content-type: application/json

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
      "body": [
        {
          "type": "TextBlock",
          "text": "Contoso MainPage"
        }
      ]
    }
  },
  "historyItems": [
    {
      "userTimezone": "Africa/Casablanca",
      "startedDateTime": "2018-02-26T20:54:04.345Z",
      "lastActiveDateTime": "2018-02-26T20:54:24.345Z"
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="036e7-142">响应</span><span class="sxs-lookup"><span data-stu-id="036e7-142">Response</span></span>

<span data-ttu-id="036e7-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="036e7-143">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.userActivity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "activitySourceHost": "https://contoso.com",
  "createdDateTime": "2017-06-09T20:54:43.969Z",
  "lastModifiedDateTime": "2017-06-09T20:54:43.969Z",
  "id": "14332800362997268276",
  "appActivityId": "/article?12345",
  "status": "updated",
  "expirationDateTime": "2017-02-26T20:20:48.114Z",
  "visualElements": {
    "displayText": "Contoso How-To: How to Tie a Reef Knot",
    "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
    "attribution": {
      "iconUrl": "https://www.contoso.com/icon",
      "alternateText": "Contoso, Ltd.",
      "addImageQuery": "false"
    },
    "backgroundColor": "#ff0000",
    "content": {
      "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
      "type": "AdaptiveCard",
      "body": [
        {
          "type": "TextBlock",
          "text": "Contoso MainPage"
        }
      ]
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
  "historyItems": [
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
